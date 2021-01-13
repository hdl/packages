# Context

**NOTE** Find a more detailed document at [docs.google.com: Building, packaging and installing Open Source EDA tooling for mixed HDL designs](https://docs.google.com/document/d/10_MqFjTIYVVuOJlusJydsp4KOcmrrHk03__7ME5thOI/).

Each GNU/Linux distribution has a default package manager: `apt-get`/`apt` on Debian/Ubuntu/LinuxMint, `yum/dnf` on RedHat/CentOS/Fedora, `pacman` on ArchLinux, etc. Therefore, the most natural procedure is to install tooling through the system package manager, since that ensures the best compatibility and stability. However, on the one hand, it is a huge effort to develop and maintain multiple recipes for each tool and for each officially supported architecture on each distribution. On the other hand, the release schedule and packaging guidelines of some distributions make it unfeasible to keep bleeding-edge projects up to date. That is the case of e.g. Debian or CentOS, which are known to be stable and slowly updating environments. Therefore, some projects provide non-official recipes for users to build their own `deb`/`rpm`/`tar.xz` packages. On Windows, it is easier to upstream recipes because `pacman` is the only supported Unix alike package manager.

Several alternatives arised in the open source EDA community for making it easier to get latest working toolchains involving several projects. The following solutions trade either features and/or platform/architecture portability for achieving working bleeding-edge environments:

## Statically pre-built packages

This provides the easiest setup approach and it allows having multiple versions of the toolchains, without running into conflicts. However, some features are limited when tools are built statically. See [YosysHQ/fpga-toolchain: DEVELOPMENT.md > General guidelines](https://github.com/YosysHQ/fpga-toolchain/blob/main/DEVELOPMENT.md#general-guidelines).

## OCI container images

This provides the less invasive solution, because no tools are installed on the host, besides the container runtime. Moreover, the behaviour of the tools is exactly the same, regardless of the host OS. However, on Windows, accessing USB devices from containers is not straightforward. See [ ghdl/docker: usbip/README.md > USB/IP protocol support for Docker Desktop](https://github.com/ghdl/docker/tree/master/usbip).

## Conda packages

Conda is an *open source package management system and environment management system that runs on Windows, macOS and Linux*. However, for Conda packages to install/configure tools, those need to be previously compiled or available as pre-built packages. Therefore, Conda packages can indeed be wrappers around some of the previous solutions.

## CIPD (Chrome Infrastructure Package Deployment)

[github.com/luci/luci-go/tree/master/cipd](https://github.com/luci/luci-go/tree/master/cipd)

## Bazel rules

Bazel is an open-source build and test tool similar to Make, Maven, and Gradle, which supports projects in multiple languages and builds outputs for multiple platforms.

## Termux recipes (Android)

"*Termux is an Android terminal emulator and Linux environment app that works directly with no rooting or setup required. A minimal base system is installed automatically - additional packages are available using the APT package manager*".

## WebAssembly packages

[YoWASP](http://yowasp.org/) aims to distribute tools from [YosysHQ](https://github.com/YosysHQ/) compiled to [WebAssembly](https://webassembly.org/) via language package managers like Python’s [PyPI](https://pypi.org/).

---

Apart from building and distributing tools using any of the solutions above, those need to be then used somehow. As discussed in [eine/vhdl-cfg](https://github.com/eine/vhdl-cfg), there are currently about a dozen projects for managing the execution of EDA tools. Any of those might rely on any of the distribution solutions explained above. In this regard, [SymbiFlow/make-env](https://github.com/SymbiFlow/make-env) is an *environment provider* meant for bootstraping the tools along with tool management projects.
