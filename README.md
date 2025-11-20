Historical development kit for the original Motorola Droid phone (model A855, codename "Sholes").
Archaeological sources (last accessed 19 Nov. 2025):
```bash
#!/bin/bash
sources=(
	'web.archive.org/web/20110812051811if_/http://wonderly.com:80/bb/DROID/OEM/VZW_A855_QSC6085BP_CWRECOVERY_UPDATE.sbf'
	'kimete.com/droid/dosbf.zip'
	'xdaforums.com/attachments/flash_image-zip.482080/'
	'codeload.github.com/kfazz/android_kernel_motorola_sholes/zip/refs/heads/jellybean'
	'codeload.github.com/koush/android_device_motorola_sholes/zip/refs/heads/froyo'
	'codeload.github.com/CyanogenMod/android_bootable_recovery/zip/refs/heads/froyo-stable'
	'codeload.github.com/lg-e400/arm-eabi-4.4.3/zip/refs/heads/master'
)
for source in "${sources[@]}"; do
	wget --method=HEAD "$source" 2>&1 | tail -n 7
done
```

