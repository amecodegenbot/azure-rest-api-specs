## Azure CLI

These settings apply only when `--az` is specified on the command line.

``` yaml $(az)
az:
  extensions: mixedreality
  package-name: azure-mgmt-mixedreality
  namespace: azure.mgmt.mixedreality
az-output-folder: $(azure-cli-extension-folder)/src/mixedreality
python-sdk-output-folder: "$(az-output-folder)/azext_mixedreality/vendored_sdks/mixedreality"

directive:
    - where:
          group: mixedreality spatial-anchor-account
      set:
          group: spatial-anchors-account
    - where:
          group: mixedreality remote-rendering-account
      set:
          group: remote-rendering-account