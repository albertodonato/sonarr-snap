# Snap for the Sonarr smart PVR

[![Snap Status](https://build.snapcraft.io/badge/albertodonato/sonarr-snap.svg)](https://build.snapcraft.io/user/albertodonato/sonarr-snap)

This snap contains the [Sonarr](https://sonarr.tv) smart PVR.

It can be installed from the store via:

```bash
    sudo snap install sonarr
```

After installing the snap the service web interface will be accessible at
<http:/localhost:8989> by default.

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-black.svg)](https://snapcraft.io/sonarr)


## Setting storage path for downloads

Since the application runs as a confined stap, by default the applicaion will only be able to access files under `/var/snap/sonarr`.
It is also possible to access storage under `/media` by manually connecting the `removable-media` interface with

```bash
    sudo snap connect sonarr:removable-media
```

It's suggested to create a directory owned by `root` either under
`/var/snap/sonarr/common` or under `/media`, after connecting the interface.


## Building the snap

The snap can be built by simply running:

```bash
    snapcraft
```

Once, built, install the snap with:

```bash
    sudo snap install --dangerous sonarr_*.snap
```
