# Red Hat CodeReady Workspaces Installer for RHPDS
![screenshot](../assets/screenshot.png)

## Pre-requisites
- [helm 3](https://helm.sh/) is available.
- bash available.
- RHPDS instance configured with `Use let's encrypt certificates`

## Configuration
Edit `crw-workshop/values.yaml` file

Namespace used to install Red Hat CodeReady Workspaces:
```yaml
installTargetNamespace: crw
```

Namespace used to install OpenShift Template Service Broker (used to install mongodb service with OpenShift connector plug-in) Workspaces:
```yaml
installTargetNamespace: crw
```

Enable OpenShift oAuth: Allows to log-in into Red Hat CodeReady Workspaces with Openshift login
```yaml
openShiftoAuth: true
```

Usage of self signed certificates
```yaml
selfSignedCert: false
```

## Run installer
Clone this repository

```bash
$ git clone https://github.com/benoitf/wrkshp-helm
$ cd wrkshp-helm
$ ./setup-workshop.sh
```

### Demo
![installer](../assets/installer.gif)
