## TWRP device tree for Lenovo A328 (A328)

Add to `.repo/local_manifests/A328.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/lenovo/A328" name="android_device_lenovo_A328" remote="hejsekvojtech" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_A328-userdebug
make -j5 recoveryimage
```
