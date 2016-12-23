# Black Duck Hub


#### How to build

Set env var of your auth token received from Blackduck hub and version

```bash
export BD_HUB_VERSION=<version>
export BD_AUTH_TOKEN=<token>
```

Download the zip from Blackduck website
```bash
cd build
wget https://updates.suite.blackducksoftware.com/appmgr.artifacts/bds-release/com/blackducksoftware/hub/appmgr.hubinstall.full/$BD_HUB_VERSION/appmgr.hubinstall.full-$BD_HUB_VERSION.zip?authToken=$BD_AUTH_TOKEN
```

Start automated build
```
./autobuild.sh -i|--image <image name> -l|--license $BD_AUTH_TOKEN
```
