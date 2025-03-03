
# MD5
40a931da749b77e13674b8d12fc765a6

# Release Note
| Category | Specification |
|----------|--------------|
| SOM | ORIN NX 64G |
| Jetpack version | 6.1.0 |
| L4T version | 35.4.1 |
| Kernel version | 5.10.104 |

# BSP build feature
- CUDA XXXX
- 

# Flash Command
## Run Command on Host PC
- Extracted BSP image file
``` bash
$  sudo tar -zxvf XXXX.tgz
```
- Switch Directory
``` bash
$  cd Linux_for_Tegra
```
- To flash QSPI + NVME SSD:
``` bash
$ sudo ./tools/kernel_flash/l4t_initrd_flash.sh --external-device nvme0n1p1 -c tools/kernel_flash/flash_l4t_external.xml -p "-c bootloader/t186ref/cfg/flash_t234_qspi.xml" --showlogs --network usb0 jetson-orin-epcr7300-a1 internal
```