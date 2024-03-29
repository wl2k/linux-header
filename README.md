# linux-image-cloud-bbr

linux-image-cloud with [TCP BBR v3](https://github.com/google/bbr/tree/v3) support.

The config file is based on this Debian kernel config file: [4.19.0-26-amd64](configs/4.19.0-26-cloud-amd64.config).

## Installation

Download the `linux-headers-*.deb` and `linux-image-*.deb` files from [Releases](../../releases).
Then install them with:

```sh
sudo dpkg -i linux-headers-*.deb linux-image-*.deb
```

## Getting started

BBR and FQ are enabled by default.

## Acknowledgments

### BBR

- [Zxilly/bbr-v3-pkg: Compile bbrv3 kernel into deb/rpm format.](https://github.com/Zxilly/bbr-v3-pkg)
- [Debian 11 手动编译 Google BBR v3 内核 - Sitao](https://sitao.org/Linux/bbrv3.html)
- [编译 Linux 内核启用 TCP BBR3-腾讯云开发者社区-腾讯云](https://cloud.tencent.com/developer/article/2345894)
- [编译 Google TCP BBR v3-荒岛](https://lala.im/8742.html)

### Kernel

- [Chapter 4. Common kernel-related tasks](https://kernel-team.pages.debian.net/kernel-handbook/ch-common-tasks.html#s-common-building)
- [BuildADebianKernelPackage - Debian Wiki](https://wiki.debian.org/BuildADebianKernelPackage)
- [How to quickly build a trimmed Linux kernel — The Linux Kernel documentation](https://docs.kernel.org/admin-guide/quickly-build-trimmed-linux.html#distro-specific-adjustments)

### Certificate

- [8.10. Compiling a Kernel](https://debian-handbook.info/browse/stable/sect.kernel-compilation.html#sidebar.kernel-config-keyring)
