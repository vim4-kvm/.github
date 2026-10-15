# VIM4 KVM

Turn a [Khadas VIM4](https://www.khadas.com/vim4) (Amlogic A311D2) into a dedicated IP-KVM:
HDMI-in capture, hardware H.264/H.265/MJPEG encoding, USB keyboard/mouse and virtual media
over USB-C, running on Ubuntu 24.04.

Four web KVM front ends run on the same board, one at a time:

| Project | Fork | Branch |
|---|---|---|
| Sipeed NanoKVM | [NanoKVM](https://github.com/vim4-kvm/NanoKVM) | `vim4` |
| JetKVM | [kvm](https://github.com/vim4-kvm/kvm) | `vim4` |
| One-KVM (Rust) | [One-KVM](https://github.com/vim4-kvm/One-KVM) | `vim4` |
| PiKVM | [kvmd](https://github.com/vim4-kvm/kvmd), [ustreamer](https://github.com/vim4-kvm/ustreamer) | `vim4` |

Platform layers:

| Layer | Repository | Branch |
|---|---|---|
| Kernel | [linux](https://github.com/vim4-kvm/linux) | `vim4-kvm-5.15` |
| Drivers and device trees | [common_drivers](https://github.com/vim4-kvm/common_drivers) | `vim4-kvm-5.15` |
| Hardware encoders | [gst-plugin-venc](https://github.com/vim4-kvm/gst-plugin-venc) | `vim4` |

Each fork keeps upstream history and license; VIM4 changes live on the branch listed above.
Original VIM4 code is released under GPL-3.0 (LGPL-2.1-or-later for the GStreamer capture plugin).
