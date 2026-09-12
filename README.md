# cosmic-files (fork ReCosmicLabs)

> **This is a fork of [pop-os/cosmic-files](https://github.com/pop-os/cosmic-files)**, the file manager of
> the COSMIC desktop by [System76](https://system76.com). All credit for the app itself goes to System76
> and the upstream contributors. The license is unchanged: **GPL-3.0-only**.

## Changes in this fork

Maintained by [ReCosmicLabs](https://github.com/ReCosmicLabs) for the
[dotfiles](https://github.com/eualexandrerrr/dotfiles) setup. Everything below is a modification of the
original work, as required by section 5 of the GPL. The `recosmic` branch holds these patches rebased on
top of upstream; `master` is an untouched mirror.

- **Home entry named after the user** (`src/lib.rs`). The sidebar and the breadcrumb show the home
  folder by its real name (the user name) instead of the generic "Home" / "Pasta pessoal".
- **Resizable sidebar** (`src/app.rs`, `src/config.rs`). The navigation bar has a 6 px drag handle on its
  right edge; dragging it changes the width (160 to 640 px) and the value is saved as `nav_bar_width` in
  the app config, so it survives restarts. Upstream fixes it at 280 px.

---

Original README follows.

# cosmic-files
File manager for the COSMIC desktop environment

## Build the project from source

```sh
# Clone the project using `git`
git clone https://github.com/pop-os/cosmic-files
# Change to the directory that was created by `git`
cd cosmic-files
# Build an optimized version using `cargo`, this may take a while
cargo build --release
# Run the optimized version using `cargo`
cargo run --release
```

## Community and Contributing

The COSMIC desktop environment is maintained by System76 for use in Pop!_OS. A list of all COSMIC projects can be found in the
[cosmic-epoch](https://github.com/pop-os/cosmic-epoch) project's README. If you would like to discuss COSMIC and Pop!_OS, please
consider joining the [Pop!_OS Chat](https://chat.pop-os.org/). More information and links can be found on the
[Pop!_OS Website](https://pop.system76.com).

## License

This project is licensed under [GPLv3](LICENSE)
