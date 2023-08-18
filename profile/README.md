# Manifest for Galaxy S21 Devices running Exynos 2100
currently only Base S21 (o1s) and Galaxy S21 Ultra (p3s) 
### Getting the manifest in place
> Create ``.repo/local_manifests/roomservice.xml`` and add this inside it:
> ```xml
> <?xml version="1.0" encoding="UTF-8"?>
> <manifest>
>	  <default revision="lineage-20">
>	  <project path="device/samsung/o1s" name="Exy2100-LOS/android_device_samsung_o1s" remote="github" revision="lineage-20"/>
>	  <project path="device/samsung/p3s" name="Exy2100-LOS/android_device_android_device_samsung_p3s" remote="github" revision="lineage-20"/>
>	  <project path="device/samsung/universal2100-common" name="Exy2100-LOS/android_device_samsung_universal2100-common" remote="github" revision="lineage-20"/>
>	  <project path="kernel/samsung/o1s" name="Exy2100-LOS/android_kernel_samsung_o1s" remote="github" revision="lineage-20"/>
>	  <project path="kernel/samsung/p3s" name="Exy2100-LOS/android_kernel_samsung_p3s" remote="github" revision="lineage-20"/>
>	  <project path="vendor/samsung/o1s" name="Exy2100-LOS/android_vendor_samsung_o1s" remote="github" revision="lineage-20"/>
>	  <project path="vendor/samsung/p3s" name="Exy2100-LOS/android_vendor_samsung_p3s" remote="github" revision="lineage-20"/>
>	  <project path="vendor/samsung/universal2100-common" name="Exy2100-LOS/android_vendor_samsung_universal2100-common" remote="github" revision="lineage-20"/>
> </manifest>
> ```
> And then sync the repos by
>```console
> repo sync --force-sync -j8
>```
