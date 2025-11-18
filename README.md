# OC-XPS-7590-Precision-5540-Sequoia

**OpenCore EFI for Dell XPS 7590 and Precision 5540 Sequoia**

This EFI supports both the Dell XPS 7590 and the Dell Precision 5540.
Both machines share the same architecture, making one configuration suitable for macOS Sequoia.

| Component              | Details                                                      |
| ---------------------- | ------------------------------------------------------------ |
| Processor              | Intel Core i7 9750H                                          |
| Graphics               | Intel UHD Graphics 630 / NVIDIA card disabled (unsupported)  |
| Display                | 15.6 inch Full HD 1920 × 1080 IPS                            |
| Memory                 | DDR4 SO DIMM up to 64 GB                                     |
| Storage                | M dot 2 PCIe NVMe SSD                                        |
| Wireless and Bluetooth | Intel wireless card. Requires HeliPort for Wi Fi. iServices like handoff and iMessage may not work or are unsupported|

**Important setup steps**
| Task                            | Description                                                                                                       |
| ------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| Generate serial and identifiers | Open the config plist with OCAT and let it generate unique platform info. Never use identifiers from someone else |
| Configure Wi Fi                 | Intel based Wi Fi needs the HeliPort app for network connections                                                  |
| Adjust BIOS settings            | Disable Secure Boot. Enable AHCI. Load defaults before applying changes                                           |
| Create a backup                 | Make a copy of your existing EFI before replacing anything                                                        |



**Special thanks**
@gorquan. EFI Based on the OC XPS 7590 project.
