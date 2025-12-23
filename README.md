# iDescriptor flake

A simple flake for idescriptor. Will become simpler when iDescriptor actually gets NixOS support.

Probably will break or smth so use at your own risk.

Make sure to have these lines in your `configuration.nix`:
```nix

services.avahi.enable = true;
services.usbmuxd.enable = true;

environment.systemPackages = with pkgs; [
  ifuse
  libimobiledevice
];

```
