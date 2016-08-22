# Install Snap
All of these packages are hosted at http://snap-telemetry.io

### Ubuntu

```
curl -s https://packagecloud.io/install/repositories/intelsdi-x/snap/script.deb.sh > installer.sh
# cat installer.sh
sudo bash installer.sh
sudo apt-get install -y snap-telemetry
```


### RedHat

```
curl -s https://packagecloud.io/install/repositories/intelsdi-x/snap/script.rpm.sh> installer.sh
# cat installer.sh
sudo bash installer.sh
sudo yum install -y snap-telemetry
```

### MacOS

```
curl -O https://github.com/intelsdi-x/snap/releases/download/v0.15.0-beta/snap-telemetry-0.15.0.pkg
sudo installer -allowUntrusted -verboseR -pkg ./snap-telemetry-0.15.0.pkg -target /
```

### man pages

Snap has manuals available on each of these builds:
```
$ man snapd
$ man snapctl
```
