OBS Studio Overlay
------------------

`USE=pulseaudio` is highly recommended (if you would like to capture audio).
PulseAudio is the only available method to capture audio in OBS Studio.

QT5 is required for OBS Studio. QT5 is currently only available on ~arch. If
you would like to use OBS Studio on stable you need to add QT5 to
package.keywords.

If you would prefer to use the live ebuild instead of the release. You will
need to add obs-studio to your package.keywords. A file you can symlink is
provided in the Documentation directory.

```
ln -s <path to overlay>/Documentation/package.keywords/obs-studio-live \
    /etc/portage/package.keywords/obs-studio-live
```
