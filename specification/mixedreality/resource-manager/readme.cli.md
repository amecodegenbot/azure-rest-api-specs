## CLI

These settings apply only when `--cli` is specified on the command line.

``` yaml $(cli)
cli:
  cli-name: mixedreality
  package-name: azure-mgmt-mixedreality
  namespace: azure.mgmt.mixedreality
  cli-directive:
    - where:
        operation: CheckNameAvailabilityLocal
      hidden: true
  test-scenario:
    - name: Create spatial anchor account
    - name: Create remote rendering account
    - name: Get remote rendering account key
    - name: Get spatial anchor account key
    - name: List spatial anchor accounts by resource group
    - name: List remote rendering accounts by resource group
    - name: Get spatial anchors account
    - name: Get remote rendering account
    - name: List remote rendering accounts by subscription
    - name: List spatial anchors accounts by subscription
    - name: List available operations
      disabled: true
    - name: Regenerate remote rendering account keys
    - name: Regenerate spatial anchors account keys
    - name: Update remote rendering account
    - name: Update spatial anchors account
    - name: CheckLocalNameAvailability
      disabled: true
    - name: Delete spatial anchors account
    - name: Delete remote rendering account
```
