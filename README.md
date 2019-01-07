# Snap for the Sonarr smart PVR

[![Snap Status](https://build.snapcraft.io/badge/albertodonato/sonarr-snap.svg)](https://build.snapcraft.io/user/albertodonato/sonarr-snap)

This snap contains the [Sonarr](https://sonarr.tv) smart PVR.

It can be installed from the store via:

```bash
    sudo snap install sonarr
```

After installing the snap the service web interface will be accessible at
<http:/localhost:8989> by default.


## Building the snap

The snap can be built by simply running:

```bash
    snapcraft
```

Once, built, install the snap with:

```bash
    sudo snap install --dangerous sonarr_*.snap
```
