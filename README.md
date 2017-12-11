## TWRP device tree for Infinix Zero 2 X509 (Infinix_X509)

Add to `.repo/local_manifests/Infinix_X509.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/infinix/Infinix_X509" name="android_device_infinix_Infinix_X509" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_Infinix_X509-eng
make -j5 recoveryimage
```
