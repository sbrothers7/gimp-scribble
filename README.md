# gimp-scribble

Prebuilt Arch Linux packages of GIMP with **scribble to erase**: scribble quickly back and forth
over paintbrush or pencil strokes to erase them (like GoodNotes). Later strokes on top are
repainted, and the whole thing is one "Scribble Erase" undo step. Tune it under
**Edit > Scribble Settings…**.

The packages are in [Releases](../../releases), tagged `<gimp version>.1-<patch hash>`. Each is
Arch's own `gimp` recipe for that version plus the attached `gimp-scribble-<hash>.patch`, built
with `makepkg`.

```sh
sudo pacman -U gimp-<version>.1-x86_64.pkg.tar.zst
```

The patch and the script that builds, installs and publishes these live in
[sbrothers7/dotfiles](https://github.com/sbrothers7/dotfiles) under `arch/.config/gimp-scribble/`.
A GIMP update from the Arch repos replaces the patched package; install the matching release
again (or build it if there isn't one yet).

GIMP is GPL-3.0-or-later; the patch is under the same license. Source for each release: the
upstream GIMP tag, Arch's packaging at the matching tag, and the patch attached to the release.
