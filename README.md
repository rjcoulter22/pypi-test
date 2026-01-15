# urllib3 False Positive Test

Test case for false positive vulnerability detection.

## Setup

- `urllib3==2.6.3` (direct dependency)
- `opensearch-py==3.0.0` (depends on urllib3>=1.26.20)

## Expected

Only `urllib3@2.6.3` should be installed and scanned.

## Actual Behavior to Test

Does SCA report vulnerabilities for both `urllib3@2.6.3` AND `urllib3@1.26.20`?

If yes, that's a false positive - urllib3@1.26.20 never exists in the actual Python environment.
# pypi-test

Adding stuff, scan again
