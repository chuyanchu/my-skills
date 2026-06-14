# Handoff QA

## Secret Scan

Before packaging or publishing, check for:

- API keys and tokens;
- cookies;
- private hostnames and IPs;
- passwords;
- personal data;
- raw client data;
- `.env` files;
- cloud credentials;
- internal-only URLs.

Replace with placeholders and document how the recipient should configure them.

## Run Verification

Prefer lightweight checks:

- install command;
- lint or import smoke test;
- unit tests if fast;
- sample CLI command;
- API health check;
- one sample request/response.

If a check cannot run locally, document the missing dependency.

## Acceptance Readiness

- The package states what "done" means.
- Sample input/output is enough for a recipient to verify behavior.
- Version/date is visible.
- Known limitations are listed.
- Deployment and rollback or restart notes exist for services.
- Database migrations or schema assumptions are documented.

## Public Sharing

For public repos or external sharing:

- remove client names unless approved;
- remove raw datasets;
- use synthetic examples;
- generalize business-specific prompts;
- keep architecture and workflow knowledge, not confidential facts.
