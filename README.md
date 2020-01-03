This is a little project I did to help me mass archive all my CDs and DVDs. The Digital Dark Age is coming and I hope this tool can help in preparation of that.

This tool is designed to manage multiple disk drives in a way that doesn't confuse you and lets you work on disks concurrently.

To run, just type `cargo run` and it will build and run like any other Rust application.
It is however dependent on some external packages:

- `libdvdcss`: driver to decode encrypted DVDs (optional). **Ubuntu users**: follow [this guide](https://help.ubuntu.com/community/RestrictedFormats/PlayingDVDs).
- `eject`: open and close drives (optional but very recommended).
- `lsscsi`: discover disk drives.
- `blkid`: discover if disks are in drives.

The following command should install all of the other dependencies on Ubuntu 18:

```
sudo apt install eject util-linux lsscis
```

Do not use this tool to violate laws of any kind.
