# Packages for electronic design automation (EDA)

This repository is an index for several projects providing *great prepackaged/prebuilt and easy-to-set-up* bleeding-edge packages/environments of [electronic design automation (EDA)](https://en.wikipedia.org/wiki/Electronic_design_automation) tools/projects. Find a discussion about the different approaches in [CONTEXT.md](CONTEXT.md).

---

- OCI container images (aka [Docker](https://www.docker.com/)/[Podman](https://podman.io/)): see [hdl/containers](https://github.com/hdl/containers) and [hdl.github.io/containers](https://hdl.github.io/containers).
- System package managers
  - `pacman` (PKGBUILD)
    - Arch Linux: see [archlinux.org/packages](https://archlinux.org/packages/), [aur.archlinux.org/packages](https://aur.archlinux.org/packages) and [SymbiFlow/symbiflow-arch-pkgs](https://github.com/SymbiFlow/symbiflow-arch-pkgs).
    - MSYS2 (Windows): see [hdl/MINGW-packages](https://github.com/hdl/MINGW-packages) and [hdl.github.io/MINGW-packages](https://hdl.github.io/MINGW-packages).
  - `apt` | `apt-get` (DEB)
    - Termux (Android): see [hdl/Termux-packages](https://github.com/hdl/Termux-packages).
  - `dnf` | `yum` (RPM)
  - `brew` (macOS)
    - See [ktemkin/homebrew-oss-fpga](https://github.com/ktemkin/homebrew-oss-fpga).
- Multiplatform package managers
  - [Bazel](https://bazel.build/) rules: see [hdl/bazel_rules_hdl](https://github.com/hdl/bazel_rules_hdl).
  - [Conda](https://conda.io) packages: see [litex-hub/litex-conda-packages](https://github.com/litex-hub/litex-conda-packages) ([litex-hub/litex-conda-eda](https://github.com/litex-hub/litex-conda-eda), [litex-hub/litex-conda-compilers](https://github.com/litex-hub/litex-conda-compilers), [litex-hub/litex-conda-prog](https://github.com/litex-hub/litex-conda-prog), [litex-hub/litex-conda-misc](https://github.com/litex-hub/litex-conda-misc), etc.).
- Statically built packages
  - See [open-tool-forge/fpga-toolchain](https://github.com/open-tool-forge/fpga-toolchain) (GNU/Linux, Windows and macOS).
- [WebAssembly](https://webassembly.org/) packages
  - See [YoWASP](http://yowasp.org/).
- CIPD (Chrome Infrastructure Package Deployment)

---

Apart from projects providing pre-built packages, the following projects are also used in the ecosystem:

- [hdl/awesome](https://github.com/hdl/awesome): index of tools/projects; there is a markdown file for each tool/project, with a frontmatter including metadata (repos, site, useful references, etc.). Those are used in the documentation of packaging projects.
- [hdl/smoke-tests](https://github.com/hdl/smoke-tests): fine grained tests that cover the most important functionalities of the tools. Those are used in packaging projects, along with more specific tests.
- [hdl/constraints](https://github.com/hdl/constraints): constraints and useful metadata about development boards, devices, and external memories. Some of the test examples in packaging projects use it.
