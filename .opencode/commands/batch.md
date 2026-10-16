
---
description: Work on a selected Spring Batch job
agent: spring-batch
---

The first argument identifies the active batch.

Batch ID: $1

Complete request:
$ARGUMENTS

Before doing any other work:

1. Validate the batch ID.
   Accept only lowercase letters, numbers and hyphens.

2. Read the batch profile:
   .opencode/batches/$1.md

3. If the profile does not exist, stop and
   report the missing profile.

4. Extract editable paths, read-only dependencies
   and the XML entry point.

5. Apply these scope restrictions to the request.

6. Start the investigation from the selected
   XML configuration when relevant.

Never inspect other batch implementations
unless the user explicitly approves it.
