## TWRP device tree for Micromax Canvas Hue (AQ5000)

Add to `.repo/local_manifests/AQ5000.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/micromax/AQ5000" name="android_device_micromax_AQ5000" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_AQ5000-eng
make -j5 recoveryimage
```