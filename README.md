<p align="center">
  <a title="hdl/community on gitter.im" href="https://gitter.im/hdl/community"><img src="https://img.shields.io/gitter/room/hdl/community.svg?longCache=true&style=flat-square&logo=gitter&logoColor=fff&color=4db797"></a><!--
  -->
</p>

# Packages for electronic design automation (EDA)

This repository is an index for several projects providing *great prepackaged/prebuilt and easy-to-set-up* bleeding-edge packages/environments of [electronic design automation (EDA)](https://en.wikipedia.org/wiki/Electronic_design_automation) tools/projects. Find a discussion about the different approaches in [CONTEXT.md](CONTEXT.md).

**NOTE** Shield/badges below indicate which projects (packaging strategies) do have a corresponding repository in this organisation, for coordination and discussion. If you want to contribute to any of those packaging solutions, go ahead and jump to the corresponding repository. Should you be willing to contribute to any other packaging project, please [open an issue](https://github.com/hdl/packages/issues/new) or [ask in the chat](https://gitter.im/hdl/community).

---

- OCI container images (aka [Docker](https://www.docker.com/)/[Podman](https://podman.io/)) [![](https://img.shields.io/badge/hdl-containers-f2f1ef.svg?longCache=true&style=flat-square&logo=GitHub&logoColor=f2f1ef)](https://github.com/hdl/containers) [![](https://img.shields.io/website.svg?label=hdl.github.io%2Fcontainers&longCache=true&style=flat-square&url=http%3A%2F%2Fhdl.github.io%2Fcontainers%2Findex.html&logo=Asciidoctor&logoColor=fff)](https://hdl.github.io/containers)
- Multiplatform package managers
  - [Bazel](https://bazel.build/) rules [![](https://img.shields.io/badge/hdl-bazel__rules__hdl-f2f1ef.svg?longCache=true&style=flat-square&logo=GitHub&logoColor=f2f1ef)](https://github.com/hdl/bazel_rules_hdl)
  - [Conda](https://conda.io) packages
    - [![](https://img.shields.io/badge/hdl-conda--eda-f2f1ef.svg?longCache=true&style=flat-square&logo=GitHub&logoColor=f2f1ef)](https://github.com/hdl/conda-eda) [![](https://img.shields.io/badge/hdl-conda--compilers-f2f1ef.svg?longCache=true&style=flat-square&logo=GitHub&logoColor=f2f1ef)](https://github.com/hdl/conda-compilers) [![](https://img.shields.io/badge/hdl-conda--prog-f2f1ef.svg?longCache=true&style=flat-square&logo=GitHub&logoColor=f2f1ef)](https://github.com/hdl/conda-prog) [![](https://img.shields.io/badge/hdl-conda--misc-f2f1ef.svg?longCache=true&style=flat-square&logo=GitHub&logoColor=f2f1ef)](https://github.com/hdl/conda-misc)
    - [litex-hub/litex-conda-packages](https://github.com/litex-hub/litex-conda-packages)
- Statically built packages
  - [YosysHQ/fpga-toolchain](https://github.com/YosysHQ/fpga-toolchain) (GNU/Linux, Windows and macOS).
- System package managers
  - PKGBUILD (`pacman`)
    - [Arch Linux](https://archlinux.org)
      - [archlinux.org/packages](https://archlinux.org/packages/)
      - [aur.archlinux.org/packages](https://aur.archlinux.org/packages)
      - [SymbiFlow/symbiflow-arch-pkgs](https://github.com/SymbiFlow/symbiflow-arch-pkgs).
    - [MSYS2](https://www.msys2.org/) (Windows) [![](https://img.shields.io/badge/hdl-MINGW--packages-f2f1ef.svg?longCache=true&style=flat-square&logo=GitHub&logoColor=f2f1ef)](https://github.com/hdl/MINGW-packages) [![](https://img.shields.io/website.svg?label=hdl.github.io%2FMINGW-packages&longCache=true&style=flat-square&url=http%3A%2F%2Fhdl.github.io%2FMINGW-packages%2Findex.html&logo=Asciidoctor&logoColor=fff)](https://hdl.github.io/MINGW-packages)
      - [sylefeb/fpga-binutils](https://github.com/sylefeb/fpga-binutils)
  - ebuild (`portage` | `layman`, [gentoo](https://www.gentoo.org/))
    - [packages.gentoo.org](https://packages.gentoo.org/)
    - [overlays.gentoo.org](https://overlays.gentoo.org/)
  - DEB (`apt` | `apt-get`)
    - [Debian](https://www.debian.org/)
      - [packages.debian.org: buster/debian-electronics](https://packages.debian.org/source/buster/debian-electronics)
      - [salsa.debian.org/electronics-team](https://salsa.debian.org/electronics-team)
    - [Termux](https://termux.com/) ([Android](https://www.android.com/)) [![](https://img.shields.io/badge/hdl-Termux--packages-f2f1ef.svg?longCache=true&style=flat-square&logo=GitHub&logoColor=f2f1ef)](https://github.com/hdl/Termux-packages)
  - RPM
    - `dnf` | `yum` ([Fedora](https://getfedora.org))
      - [src.fedoraproject.org](https://src.fedoraproject.org/)
      - [fedoraproject.org/wiki: Electronic Lab](https://fedoraproject.org/wiki/Electronic_Lab) a [lab/spin](https://labs.fedoraproject.org) not available anymore
    - `zypper` | `yast` ([OpenSUSE](https://www.opensuse.org/))
      - [build.opensuse.org | hardware:FPGA](https://build.opensuse.org/project/show/hardware:FPGA)
      - [SymbiFlow/ideas#59](https://github.com/SymbiFlow/ideas/issues/59)
  - NIX ([NixOS](https://nixos.org/))
    - [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  - `brew` (macOS)
    - [ktemkin/homebrew-oss-fpga](https://github.com/ktemkin/homebrew-oss-fpga)
- [WebAssembly](https://webassembly.org/) packages
  - [YoWASP](http://yowasp.org/).
- CIPD (Chrome Infrastructure Package Deployment)

---

Apart from projects providing pre-built packages, the following projects are also used in the ecosystem:

- [![](https://img.shields.io/badge/hdl-awesome-f2f1ef.svg?longCache=true&style=flat-square&logo=GitHub&logoColor=f2f1ef)](https://github.com/hdl/awesome) [![](https://img.shields.io/website.svg?label=hdl.github.io%2Fawesome&longCache=true&style=flat-square&url=http%3A%2F%2Fhdl.github.io%2Fawesome%2Findex.html&logo=Asciidoctor&logoColor=fff)](https://hdl.github.io/awesome): index of tools/projects; there is a markdown file for each tool/project, with a frontmatter including metadata (repos, site, useful references, etc.). Those are used in the documentation of packaging projects.
- [![](https://img.shields.io/badge/hdl-smoke--tests-f2f1ef.svg?longCache=true&style=flat-square&logo=GitHub&logoColor=f2f1ef)](https://github.com/hdl/smoke-tests): fine grained tests that cover the most important functionalities of the tools. Those are used in packaging projects, along with more specific tests.
- [![](https://img.shields.io/badge/hdl-constraints-f2f1ef.svg?longCache=true&style=flat-square&logo=GitHub&logoColor=f2f1ef)](https://github.com/hdl/constraints) [![](https://img.shields.io/website.svg?label=hdl.github.io%2Fconstraints&longCache=true&style=flat-square&url=http%3A%2F%2Fhdl.github.io%2Fconstraints%2Findex.html&logo=Asciidoctor&logoColor=fff)](https://hdl.github.io/constraints): constraints and useful metadata about development boards, devices, and external memories. Some of the test examples in packaging projects use it.
