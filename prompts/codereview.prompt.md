---
name: codereview
description: After making changes to code, request a code review from CodeRabbit for your uncommitted changes.
---

Request a code review from CodeRabbit by running `coderabbit --prompt-only --type uncommitted` in the background. Allow it to take as long as it needs and check on it periodically. When it finishes, it will output `Review Completed`. If there are no issues found, consider the review passed.

If there are issues found, evaluate the fixes and considerations. Fix major and critical issues only and ignore the nits.

Once those changes are implemented, run CodeRabbit CLI one more time to make sure we addressed all the critical issues and didn't introduce any additional bugs.

Only run the loop twice. If on the second run you don't find any critical issues, ignore the nits and you're complete. Give me a summary of everything that was completed and why.