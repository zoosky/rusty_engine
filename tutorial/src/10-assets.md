# Asset Pack

Rusty Engine assumes the asset pack is present, so you MUST download the asset pack.

Here are three different ways to download the assets (pick any of them--it should end up the same in the end):
- RECOMMENDED: On a posix compatible shells run this command inside your project directory:
```shell
curl -L https://github.com/CleanCut/rusty_engine/archive/refs/heads/main.tar.gz | tar -zxv --strip-components=1 rusty_engine-main/assets
```
- OR, clone the `rusty_engine` repository and copy/move the `assets/` directory over to your own project
- OR, download a [zip file](https://github.com/CleanCut/rusty_engine/archive/refs/heads/main.zip) or [tarball](https://github.com/CleanCut/rusty_engine/archive/refs/heads/main.tar.gz) of the `rusty_engine` repository, extract it, and copy/move the `assets/` directory over to your own project.

## Asset Directory Structure

All assets reside inside an `assets/` directory at the top folder of your Rust project (in the same directory as `Cargo.toml`).

The structure looks like this:

```text
assets
├── audio
│   ├── music
│   └── sfx
├── fonts
└── sprite
    ├── racing
    └── rolling
```

All audio files should be stored in `assets/audio`*. The asset pack divides sounds into `music` and `sfx` subdirectories.

All font files should be stored in `assets/font`*.

All sprites should be stored in `assets/sprite`*.

*Additional subdirectories may be used for organization inside of these directories, as the asset pack does in some cases.
