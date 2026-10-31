# SigmaOS Boot Configuration

A Rust library for modeling boot-menu settings, kernel parameters, and boot entries. `BootConfigManager` stores these values, builds a kernel command line, generates GRUB-style configuration text, and reports validation messages.

This crate generates and validates configuration data in memory. It does not install a bootloader, write system boot files, or prove that the generated configuration boots on a target machine.

## Build

The manifest uses the sibling [`SigmaOS-kernel`](../SigmaOS-kernel) path dependency. From the SigmaOS checkout:

```sh
cargo check --manifest-path SigmaOS-boot-config/Cargo.toml --lib
```

## License

GPL-3.0-or-later. See [`Cargo.toml`](Cargo.toml).
