# example-install-helm

To install Helm 3 on Ubuntu 22.04, while ensuring that we always get the latest stable Helm version directly from the official source
 Here's a breakdown of the steps:

### 1. Download the Helm Install Script
```
curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3
```
This fetches the official Helm installation script.

### 2. Set Execute Permissions
```
chmod 700 get_helm.sh
```
This ensures the script has the correct execution rights.

### 3. Run the Installation Script

```
./get_helm.sh
```

This installs the latest stable version of Helm 3.

### 4. Verify Installation
```
helm version
```
Expected output:
```
version.BuildInfo{Version:"v3.x.x", GitCommit:"xxxxx", ...}
```
### 5.Clean Up the Script

We run this optional command if we do not need the install script:

```
rm get_helm.sh
```






