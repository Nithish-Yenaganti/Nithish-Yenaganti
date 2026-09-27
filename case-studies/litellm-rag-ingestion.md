# Fixing false-success RAG ingestion in LiteLLM

[Merged PR #30628](https://github.com/BerriAI/litellm/pull/30628) · Python · June 18, 2026

## User-visible problem

A caller supplied an existing OpenAI `file_id` and a `vector_store_id` to LiteLLM's RAG ingestion API. The request could return a completed response without attaching that file to the vector store. A successful API response therefore did not guarantee that the requested ingestion happened.

## My contribution

I traced the existing-file path through the shared ingestion layer and the OpenAI provider implementation, then:

- added an explicit provider capability for reusing an existing file ID;
- attached the file through `vector_store_file_acreate` on the OpenAI path;
- required a vector store ID for the attachment;
- made providers without existing-file support fail clearly;
- added regression tests for the successful attachment and the two failure cases.

## Validation and review

The PR reports three focused regression tests passing. After feedback, I updated typing syntax and investigated CI failures, distinguishing a setup cancellation from failures caused by the change. The final commit passed all 73 checks, received maintainer approval, and was merged into LiteLLM's `litellm_oss_staging` branch.

The [PR conversation](https://github.com/BerriAI/litellm/pull/30628) contains the test commands, CI follow-up, review, and merge record. These are historical validation results for that PR, not a claim that the current repository was retested here.

## Outcome and limits

The merged change makes an existing-file ingest perform the requested attachment or report a failure for unsupported or incomplete inputs. I do not have public production adoption, latency, or revenue measurements for this fix.

## Engineering lesson

Test the side effect that a successful response promises. A status field alone cannot prove that a file was attached, persisted, or made available to retrieval.
