# Delivery Structure

For a standalone package:

```text
delivery_package/
  README.md
  docs/
    deployment.md
    api.md
    data_contract.md
    database.md
    test_commands.md
    troubleshooting.md
  examples/
    sample_input/
    sample_output/
  scripts/
  tests/
  delivery_inventory.md
  acceptance_checklist.md
```

For an existing repo:

- keep the current code layout;
- add missing docs under `docs/`;
- add sample input/output under `examples/`;
- add acceptance docs at the repo root or under `docs/`;
- do not move large code folders unless the user asks.

## Minimum Handoff Set

- README with quick start.
- Environment/configuration notes.
- One known-good run command.
- API or CLI usage docs.
- Sample input and expected output.
- Test or smoke-check commands.
- Known limitations.
- Delivery inventory.
