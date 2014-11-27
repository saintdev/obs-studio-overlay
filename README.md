OBS Studio Overlay
------------------

`USE=pulseaudio` is highly recommended (if you would like to capture audio).
PulseAudio is the only available method to capture audio in OBS Studio.

QT 5 is required for OBS Studio. It is currently masked in the portage tree.

To unmask the required QT 5 packages, symlink Documentation/package.unmask/obs-studio
into /etc/portage/package.unmask/.

```
ln -s <path to overlay>/Documentation/package.unmask/obs-studio \
/etc/portage/package.unmask/obs-studio
```

If you would prefer to use the live ebuild instead of the release. You will
need to add obs-studio to your ACCEPT_KEYWORDS. A file you can symlink is
provided.

```
ln -s <path to overlay>/Documentation/package.keywords/obs-studio-live \
/etc/portage/package.keywords/obs-studio-live
```
