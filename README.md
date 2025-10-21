# DO NOT USE!

Unless you really want to use the squashfs uruntime, there is no real reason to use this appimagetool, it only supports squashfs.

Use the DWARFS uruntime, **it is a lot better in every single measurable way**, you can use this [script instead](https://github.com/pkgforge-dev/Anylinux-AppImages/blob/main/useful-tools/uruntime2appimage.sh) for that.

---


This is a fork of [AppImage/appimagetool](https://github.com/AppImage/appimagetool) that uses the squashfs [uruntime](https://github.com/VHSgunzo/uruntime) instead of the [type2-runtime](https://github.com/AppImage/type2-runtime) by default.

The uruntime is fully compatible to with the type2-runtime and offers advatnages such as:

* [Automatically extract and run](https://github.com/psadi/ghostty-appimage/pull/50#issuecomment-2686587362) when fuse is not available.

* [Keep the filesystem mounted](https://github.com/psadi/ghostty-appimage/pull/54) for even faster launch times.

* Easily set extra env variables by making a `$0.env` file with the variables to be set, similar to the existing portable `$0.home` and `$0.config` feature of the type2-runtime. 

* Have a portable `~/.local/share` dir by making a `$0.share` directory.
