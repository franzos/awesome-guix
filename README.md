# Awesome Guix [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Package manager and distribution of the GNU system with reproducible, transactional upgrades.

[<img src="https://codeberg.org/guix/artwork/raw/branch/master/logo/head-only/Guix-head.svg" align="right" width="120" alt="Guix">](https://guix.gnu.org/)

GNU Guix is a functional package manager and a distribution of the GNU operating system. Every package is built in an isolated environment and stored under a hash of all its inputs, so the same definition produces the same result on any machine, and pre-built substitutes can stand in for local builds. Packages, services, home environments and whole operating systems are declared in Guile Scheme. Every change is a transaction: an upgrade either completes or leaves the system untouched, and each generation can be rolled back, down to the boot menu. Guix runs as a standalone package manager on top of any GNU/Linux distribution, or as Guix System, where the entire machine is configured from a single file. The distribution ships only free software and is bootstrapped from a small, auditable binary seed.

## Contents

- [Docs and Videos](#docs-and-videos)
- [Tools](#tools)
- [Channels](#channels)
- [Distributions](#distributions)
- [Build Servers](#build-servers)
- [Config Examples](#config-examples)
- [Misc](#misc)
- [Communities](#communities)
- [Guix on Other Distros](#guix-on-other-distros)

## Docs and Videos

- [Guix Manual](https://guix.gnu.org/manual/en/html_node/) - The reference manual.
- [Guix Cookbook](https://guix.gnu.org/cookbook/en/) - Tutorials and worked examples: packaging, Scheme crash course, system config.
- [Guix Reference Card](https://guix.gnu.org/guix-refcard.pdf) - Must-have cheat sheet.
- [Guix Help](https://guix.gnu.org/en/help/) - Videos, tutorials and where to ask.
- [Guix Blog](https://guix.gnu.org/en/blog/) - Announcements, packaging guides and things like [Music Production on Guix System](https://guix.gnu.org/en/blog/2020/music-production-on-guix-system/).
- [PantherX Wiki](https://wiki.pantherx.org/Table-of-contents/) - Guides for PantherX, most of which apply to Guix System.

### Articles and Videos

- [pjotrp/guix-notes](https://gitlab.com/pjotrp/guix-notes) - Notes on using and packaging with Guix.
- [The Guix System Image API](https://othacehe.org/the-guix-system-image-api.html) - Building disk images with Guix.
- [The Guile Hacker Handbook](https://jeko.frama.io/) - Learning Guile by building things.
- [5 Reasons to Try GNU Guix in 2022](https://systemcrafters.net/craft-your-system-with-guix/5-reasons-to-try-guix/) - The case for Guix, by System Crafters.
- [Installing the GNU Guix Package Manager](https://systemcrafters.net/craft-your-system-with-guix/installing-the-package-manager/) - On Debian, Arch, Fedora and others.
- [Guix Gaming Desktop](https://boilingsteam.com/how-i-built-my-new-linux-gaming-desktop-in-2021-with-amd-cpugpu-and-gnu-guix/) - Building a Linux gaming desktop on Guix.
- [A Home Router with GNU Guix](https://timmydouglas.com/2021/02/07/guix-router.html) - Running a home router on Guix System.
- [YouTube Playlist: GNU Guix](https://www.youtube.com/playlist?list=PLZmotIJq3yOI0cPPQ07urjm6VMnb8GDSQ) - By Andrew Tropin.
- [YouTube Playlist: Craft Your System with GNU Guix](https://www.youtube.com/playlist?list=PLEoMzSkcN8oNxnj7jm5V2ZcGc52002pQU) - By System Crafters.
- [YouTube: How to Install GNU Guix System (2027 Edition)](https://www.youtube.com/watch?v=3mbCH7sBLeI) - Installation walkthrough.
- [Shell Examples](https://codeberg.org/nutcase/guix-shell-examples) - Run software that's not available on Guix.
- [Build React Native Android Apps on Guix](https://gofranz.com/blog/react-native-android-on-guix-without-docker/) - Android builds without Docker.

## Tools

- [Guix Packager](https://guix-hpc.gitlabpages.inria.fr/guix-packager/) - Write a package definition in a breeze.
- [System Config Generator](https://www.pantherx.org/configs/) - Config generator for PantherX OS (similar to Guix).
- [guix-install](https://github.com/franzos/guix-install) - Guix System installer: libre, nonguix, panther, or enterprise.
- [guix-rs](https://github.com/franzos/guix-rs) - Unofficial GUI for day-to-day Guix usage.
- [esquema](https://github.com/cristiancmoises/esquema) - Rootless, daemon-free container runtime written in Scheme, integrating with Guix and Shepherd.
- [Guix Data Service](https://data.guix.gnu.org/) - Query packages, derivations and lint warnings for any revision of Guix.
- [Guix QA](https://qa.guix.gnu.org/) - Build status of the team branches queued for merge into master.

## Channels

- [guix](https://codeberg.org/guix/guix) - The primary channel. Legacy repository on [GNU Savannah](https://git.savannah.gnu.org/cgit/guix.git).
- [nonguix](https://gitlab.com/nonguix/nonguix) - Packages that can't be included upstream.
- [pantherx](https://codeberg.org/gofranz/panther) - System and packages for PantherX.
- [games](https://gitlab.com/guix-gaming-channels/games) - Collection of non-free game packages.
- [guix-android](https://framagit.org/tyreunom/guix-android) - Experimental packages for Android development.
- [guix-past](https://codeberg.org/guix-science/guix-past) - Packages from the past.
- [guix-hpc](https://gitlab.inria.fr/guix-hpc/guix-hpc) - Extensions for high-performance computing.
- [guix-hpc-non-free](https://gitlab.inria.fr/guix-hpc/guix-hpc-non-free) - Non-free HPC software, or free software with non-free dependencies.
- [guix-science](https://codeberg.org/guix-science/guix-science) - Free scientific packages.
- [guix-science-nonfree](https://codeberg.org/guix-science/guix-science-nonfree) - Non-free scientific packages.
- [guix-ost](https://gitlab.ost.ch/scl/guix-ost) - Software recipes for the HPC-RJ Cluster.
- [sops-guix](https://github.com/fishinthecalculator/sops-guix) - Secure secret management with Guix.
- [gocix](https://github.com/fishinthecalculator/gocix) - Community managed library of Guix services.
- [small-guix](https://codeberg.org/fishinthecalculator/small-guix.git) - Small Guix.
- [guix-cn](https://github.com/guixcn/guix-channel) - Channel of the Guix China community.
- [bin-guix](https://github.com/ieugen/bin-guix) - Binary packages.
- [rosenthal](https://codeberg.org/hako/Rosenthal) - Experiments.
- [giuliano108/guix-packages](https://github.com/giuliano108/guix-packages) - Guix on WSL2, packages and notes.
- [guix-wigust](https://github.com/kitnil/guix-wigust) - Extra packages.
- [guix-rustup](https://github.com/declantsien/guix-rustup) - Rustup toolchains on Guix.
- [guix-tailscale](https://github.com/umanwizard/guix-tailscale) - Provides tailscale, tailscaled, and tailscale-service-type.
- [guixrus](https://git.sr.ht/~whereiseveryone/guixrus) - Channel maintained by the whereiseveryone community.
- [guix-crypto](https://codeberg.org/attila.lendvai/guix-crypto) - Crypto and Blockchain related packages and services.
- [gundroid](https://github.com/shegeley/gundroid) - Android tools packages.
- [divya-lambda](https://codeberg.org/divyaranjan/divya-lambda) - Haskell, Rust packages and toolchain, libre audio software, emacs-next, among others.
- [guix-cran](https://github.com/guix-science/guix-cran) - All R packages not available in Guix yet.
- [guix-bioc](https://github.com/guix-science/guix-bioc) - The entire Bioconductor collection, generated like guix-cran.
- [saayix](https://codeberg.org/look/saayix) - Personal channel for developing and sharing services and packages.
- [radix](https://codeberg.org/anemofilia/radix) - Personal channel, which contains Free Software only.
- [abbe](https://codeberg.org/group/guix-modules) - Many up-to-date Rust and Go apps built with custom nix-like build systems, and more.
- [emacs-master](https://github.com/gs-101/emacs-master) - The latest Emacs from the master branch.
- [guix-telegram-desktop](https://github.com/johnlepikhin/guix-telegram-desktop) - Latest version of telegram-desktop.
- [asahi-guix/channel](https://codeberg.org/asahi-guix/channel) - Run the GNU operating system with the Asahi Linux kernel on Apple Silicon devices.
- [dariqq/guix-surface](https://codeberg.org/Dariqq/guix-surface) - Implementation of linux-surface for GNU Guix.
- [kolev/guix-channel](https://codeberg.org/kolev/guix-channel) - Chromebook audio configuration and SUPDUP.
- [ROCKTAKEY/roquix](https://github.com/ROCKTAKEY/roquix) - Roquix Guix channel.
- [minkieyume/chiko-guix-channel](https://codeberg.org/minkieyume/chiko-guix-channel) - Minkie Chiko's Guix channel.
- [Jonabron](https://github.com/librepup/jonabron) - Provides osu!lazer, Vicinae, Discord, and more.
- [guix-eda](https://codeberg.org/fsi/guix-eda) - Electronic design automation, with pinned versions for specific purposes.
- [guix-bitcoin](https://codeberg.org/trevarj/guix-bitcoin) - Bitcoin ecosystem: nodes, wallets, Lightning, indexers and block explorers.
- [guix-astro](https://codeberg.org/vleugelcomplement/guix-astro) - Astrophysics-adjacent codes which are not yet included upstream.
- [guix-discord](https://github.com/jack-faller/guix-discord) - Discord, and some Discord related packages.
- [aagl-guix](https://codeberg.org/ch4og/aagl-guix) - Run an-anime-team launchers on Guix.
- [Jasmine](https://codeberg.org/SameExpert/guix-jasmine) - Application and desktop themes.

### Package Indexes

- [toys.whereis.social](https://toys.whereis.social/) - JSON API for exploring Guix channels on the internets.
- [packages.guix.gnu.org](https://packages.guix.gnu.org/) - Packages in guix.
- [pantherx.org/packages](https://www.pantherx.org/packages/) - Packages in guix, nonguix and pantherx.
- [hpc.guix.info/browse](https://hpc.guix.info/browse) - Packages in guix, guix-hpc, guix-past, guix-science and guix-cran.

### Wishlist

- [Guix/Wishlist](https://libreplanet.org/wiki/Group:Guix/Wishlist) - Software that users of GNU Guix would like to see packaged.
- [Codeberg/Wishlist](https://codeberg.org/guix/guix/issues?labels=422988) - Feature and update requests users would like to see implemented in GNU Guix.

### Issue Trackers

- [guix](https://codeberg.org/guix/guix/issues) - Issues for Guix itself.
- [nonguix](https://gitlab.com/nonguix/nonguix/-/work_items) - Issues for the nonguix channel.
- [pantherx](https://github.com/franzos/panther/issues) - Issues for the PantherX channel.

## Distributions

- [Guix System](https://guix.gnu.org/en/download/) - The GNU operating system built on Guix.
- [PantherX](https://www.pantherx.org/) - Guix-based distribution with its own channel and tooling.
- [rde](https://sr.ht/~abcdw/rde/) - Developer and power-user environment built on Guix.

## Build Servers

Substitutes (aka pre-built software) come from here:

- [ci.guix.gnu.org](http://ci.guix.gnu.org/) - Official Cuirass build farm.
- [bordeaux.guix.gnu.org](https://bordeaux.guix.gnu.org/) - Official substitute server.
- [berlin.guix.gnu.org](https://berlin.guix.gnu.org/) - Official substitute server.
- [substitutes.nonguix.org](https://substitutes.nonguix.org/) - Substitutes for the nonguix channel.
- [substitutes.guix.gofranz.com](https://substitutes.guix.gofranz.com/) - Substitutes for the PantherX channel.
- [guix.tobias.gr](https://guix.tobias.gr/substitutes/) - Third-party substitute server.
- [cuirass.genenetwork.org](https://cuirass.genenetwork.org/) - GeneNetwork build farm ([public key](https://git.genenetwork.org/guix-north-america/about/)).

Love the quote, from the last one; though it seems Firefox has fallen into this category too.

> Only malware, such as Chromium, will never be distributed.

Want to run your own substitute server? Check out [Cuirass](https://guix.gnu.org/cuirass/).

## Config Examples

When you're stuck, it's super helpful to see what others are doing.

- [tyreunom/system-configuration](https://framagit.org/tyreunom/system-configuration) - Personal system configuration.
- [aurtzy/guix-config](https://github.com/aurtzy/guix-config) - System and Home configuration modularized with "mods", an extension to Guix records.
- [hiecaq/guix-config](https://github.com/hiecaq/guix-config) - Literate Org configuration covering system, home and channels.
- [podiki/dot.me](https://github.com/podiki/dot.me/tree/master/guix/.config/guix) - Guix configuration in literate dotfiles, tangled from Org and linked with GNU Stow.
- [anemofilia/zero](https://codeberg.org/anemofilia/zero) - Modular system and home environments that keep desktop concerns out of the operating system.
- [hako/Testament](https://codeberg.org/hako/Testament) - Literate Guix System configurations, dotfiles and live CD images, built with BLUE.
- [look/misako](https://codeberg.org/look/misako) - Modular system and home configurations, companion to the saayix channel.
- [VnPower/rkgk](https://codeberg.org/VnPower/rkgk) - Lisp-machine-style desktop on Guix System.
- [mrh/dotfiles](https://codeberg.org/mrh/dotfiles) - Per-machine Guix System configurations alongside an Emacs setup.
- [franzos/dotfiles](https://github.com/franzos/dotfiles) - Two-host Guix System configuration with a shared module and system hardening.
- [berkeley/guix-config](https://codeberg.org/berkeley/guix-config) - Hardened, minimal System and Home configuration with XMonad, River and Sway desktops.
- [fishinthecalculator/guix-deployments](https://codeberg.org/fishinthecalculator/guix-deployments) - Opinionated operating-system definitions, distributed as a signed channel.
- [aartaka/guix-config](https://github.com/aartaka/guix-config) - System configuration and a large development manifest.

## Misc

- [guix-vm](https://github.com/palfrey/guix-vm) - Scripts and support necessary to make a GuixSD VirtualBox image.
- [DistroWatch](https://distrowatch.com/table.php?distribution=guixsd) - Release history and package versions of Guix System.
- [flathub.org/setup](https://flathub.org/en/setup/GNU%20Guix) - Flatpak on Guix.
- [metacall/guix](https://github.com/metacall/guix) - Docker image for using Guix in a CI/CD environment.
- [kristianlm/hetzner.scm](https://gist.github.com/kristianlm/089a6759a74dcd2e6f702847cf919ed2) - Guix on Hetzner Cloud.

## Communities

- [Mailing Lists](https://guix.gnu.org/contact/) - Official Guix mailing lists, plus IRC on Libera: `#guix`, `#info-guix`, `#guixcn`, `#nonguix`.
- [#guix:matrix.org](https://matrix.to/#/%23guix:matrix.org) - Matrix room.
- [r/GUIX](https://www.reddit.com/r/GUIX) - Subreddit.
- [gnu_guix_en](https://t.me/gnu_guix_en) - Telegram group, also in [Russian](https://t.me/gnu_guix_ru), [Portuguese](https://t.me/gnu_guix_br) and [Chinese](https://t.me/guixcn).

## Guix on Other Distros

- [Guix Binary Installation](https://guix.gnu.org/manual/en/html_node/Binary-Installation.html) - Install almost anywhere.
- [Guix Desktop-Environment Integration](https://gist.github.com/peanutbutterandcrackers/844c211a91137c19607ae75b59fa116f) - Make Guix-installed applications show up in the host desktop.
- [Nix](https://search.nixos.org/packages?query=guix&show=guix) - Guix in nixpkgs.
- [Arch](https://aur.archlinux.org/packages/guix) - Guix in the AUR.
- [Debian](https://packages.debian.org/search?keywords=guix) - Guix in the Debian archive.
- [Ubuntu](https://packages.ubuntu.com/search?keywords=guix) - Guix in the Ubuntu archive.
- [Fedora](https://copr.fedorainfracloud.org/coprs/lantw44/guix/) - Guix via Copr.
- [Alpine](https://pkgs.alpinelinux.org/packages?name=guix&branch=edge&arch=) - Guix in Alpine edge.

## Related Lists

- [tieong/awesome-guix](https://github.com/tieong/awesome-guix) - Another Guix list.

## Footnotes

Unmaintained and archived entries, still useful as references, are listed in [unmaintained.md](unmaintained.md).
