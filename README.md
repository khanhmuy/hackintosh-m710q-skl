# hackintosh-ideapad-3-14ABA7
## Intro

|          | Version                 |
|----------|-------------------------|
| OpenCore | 0.9.3                   |
| macOS    | Monterey |

- Supported macOS versions: In theory this should work with any version supported by NootedRed, however only Ventura has been tested.

## Info / Disclaimer
### Info
- `boot-args` used: `debug=0x100 keepsyms=1`
- `alcid`: `11`
- SMBIOS: `iMac18,1`
- `ShowPicker`, `ScanPolicy` and `HideAuxilary` are set up in a way that automatically boots to a APFS partition with macOS installed without user confirmation. Adjust accordingly for installation (that's why you should read the guide).
### Usage
- You can use it however you like, except for commercial purposes (such as work enviroments and reselling your Hackintosh), refer to the [Psystar case](https://en.wikipedia.org/wiki/Psystar_Corporation). TLDR, you'll get your ass sued if you do so.
- Reminder that this is only a base for your OpenCore setup and should always be viewed as incomplete, and it is strongly recommended that you follow the entire OpenCore guide [here](https://dortania.github.io/OpenCore-Install-Guide/). 
- **DO NOT USE ANY INSTALLER NOT FROM APPLE**, no one knows if/how they've been tampered with, and they *always* break the APFS system volume seal, which breaks OTA updates, and are generally not trustworthy at all.
### Issues
- Sleep does not work.
- To get display output, it is required to unplug the DP cable after selecting macOS to boot, then reconnecting when the system has finished booting.
### Notes
- Don't use case-sensitive APFS if you want to use Steam or Adobe tools.
## Hardware

|                                           | Specifications                                                                | macOS Compatibility                                                                                                                   |
| ----------------------------------------- | ----------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| ``CPU``                                   | Intel(R) Core(TM) i5-6500T, 4 Cores / 4 Threads, 2.5GHz / 3.1GHz, 6MB L3 Cache | With native power management|
| ``Memory``                                | 16GB DDR4-2133MHz                                  |                                                                                                                                               |
| ``GPU``                                   | Intel HD 530                                                       | With full QE/CI (Graphics accleration)|
| ``Storage``                               | IM2P33F3A NVMe ADATA 256GB                                              |                                                                                                                                              |             
| ``WiFi``                                  | Intel AC-8265                                                        | Works with `AirPortitlwm`                                                                |
| ``Bluetooth``                             | Intel                                                                         | Works. |
| ``Audio``                            | Realtek ALC294                                                      |                                                                                                                                               |

Special thanks to:
- [acidanthera](https://github.com/acidanthera) - the maker of OpenCore and your favourite kexts, for making this Hackintosh possible in the first place
- [dortania people](https://github.com/orgs/dortania/people) for the OpenCore Install Guide
- [quynkk5](https://github.com/quynkk5) for helping me fix display outputs

readme prouldly ~~stolen from~~ inspired by [beerpiss](https://github.com/beerpiss/dell-vostro-15-3568-hackintosh)'s

