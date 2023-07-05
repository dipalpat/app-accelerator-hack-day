## Local Authoring and Publishing Application Accelerators
For local authoring and faster feedback Tanzu CLI and Accelerator Plugin can be leveraged. The instructions for publishing the accelerator to Azure Spring Apps Enterprise are provided below.
* [Tanzu CLI Installation Instructions](https://docs.vmware.com/en/VMware-Tanzu-Application-Platform/1.5/tap/install-tanzu-cli.html#install-or-update-the-tanzu-cli-and-plugins-3)
* [Publish Accelerator using Azure CLI](https://learn.microsoft.com/en-us/azure/spring-apps/how-to-use-accelerator?tabs=Azure-CLI#manage-your-own-accelerators)
* [Publish Accelerator using Azure Portal](https://learn.microsoft.com/en-us/azure/spring-apps/how-to-use-accelerator?tabs=Portal#manage-your-own-accelerators)

For local authoring and testing, use the ```tanzu accelerator generate-from-local``` command.

```tanzu acc generate-from-local --accelerator-path test-gen-local=./ --options-file=./options.json --server-url=https://ASAE_DEV_PORTAL_URL -o=./test --force```

```tanzu accelerator generate-from-local --accelerator-path java-rest=workspace/java-rest --fragment-paths java-version=workspace/version --fragment-names tap-workload --options '{"projectName":"test"}'```

```      --accelerator-name string             name of the registered accelerator to use
      --accelerator-path "key=value" pair   key value pair of the name and path to the directory containing the accelerator
  -f, --force                               force clean and rewrite of output-dir
      --fragment-names strings              names of the registered fragments to use
      --fragment-paths stringToString       key value pairs of the name and path to the directory containing each fragment (default [])
  -h, --help                                help for generate-from-local
      --options string                      options JSON string (default "{}")
      --options-file string                 path to file containing options JSON string
  -o, --output-dir string                   the directory that the project will be created in (defaults to the project name)
      --server-url string                   the URL for the Application Accelerator server
```

## Installing VS Code Tanzu Extension
Use the following steps to install the Application Accelerator Visual Studio extension:

1. Sign in to VMware Tanzu Network and download the “Tanzu App Accelerator Extension for Visual Studio Code” file from the product page for [VMware Tanzu Application Platform](https://network.tanzu.vmware.com/products/tanzu-application-platform).

2. Open VS Code.

* **Option 1:**

1. From the Command Palette (cmd + shift + P), run “Extensions: Install from VSIX…”.

2. Select the extension file **tanzu-app-accelerator-<EXTENSION_VERSION>.vsix.**


* **Option 2:**

1. Select the **Extensions** tab

2. Select **Install from VSIX…** from the overflow menu.



