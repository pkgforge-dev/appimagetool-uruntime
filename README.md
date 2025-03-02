This is a fork of [AppImage/appimagetool](https://github.com/AppImage/appimagetool) that uses the squashfs [uruntime](https://github.com/VHSgunzo/uruntime) instead of the [type2-runtime](https://github.com/AppImage/type2-runtime) by default.

The uruntime is fully compatible to with the type2-runtime and offers advatnages such as:

* [faster launch times](https://github.com/AppImage/type2-runtime/issues/116) 

* [Automatically extract and run](https://github.com/psadi/ghostty-appimage/pull/50#issuecomment-2686587362) when fuse is not available.

* [Keep the filesystem mounted](https://github.com/psadi/ghostty-appimage/pull/54) for even faster launch times.
