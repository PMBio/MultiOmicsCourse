# MultiOmicsCourse

## Description:
This course provides insights into the foundations and principles of multi-omics data analysis and modeling,. The course is aimed specifically for students with experience in Python programming, eager to apply and broaden their skills in single-cell genomics and multi-omics  setting. This is a four day course, consisting of lectures in the morning and practicals in the afternoon.

- [Day 1](day1/):  will provide foundations in multi omics technologies and analysis
- [Day 2](day2/):  will focus on basics of machine and supervised analysis of single-cell data,
- [Day 3](day3/):  will focus on unsupervised exploration of multi-omics bulk and single-cell assay
- [Day 4](day4/):  will introduce spatial multi-omics analytics and integration.



## Slides & Material:


## Prerequisites:

* Experience in Python programming, and the use of bash.
* Access to a Linux/Mac/Windows OS machine for practicals

## Downloads
* Day 1: Please [download](https://drive.google.com/drive/folders/17sufCcvtCAbaBn5MfKr5ZxWdz2ilXL51?usp=drive_link) the folder and run the first notebook to download the datasets.  (this is cloned from [here](https://github.com/NBISweden/workshop-scRNAseq).)
* Day 2: [data](https://hub.dkfz.de/s/JWBprGiT6MELiDN)
* Day 3: TBD
* Day 4: [data](https://hub.dkfz.de/s/WxptQkKEb36EnAP)

# Environments
* Day 1: [environment-day1](environments/day1.yml)
* Day 2: [environment-day2](environments/day2.yml)
* Day 3: [environment-day3](environments/day3.yml)
* Day 4: 

## Optional
### VM
In case you don't manage to set everything up on your own computer, we have prepared a Linux virtual machine that has all the packages you need.
This is intended purely as a last resort, since it adds quite a bit of RAM and CPU overhead.
You can download it [here](https://drive.google.com/file/d/1-9iBqS1XzWvGqPUxMfsoi4Gk-f-fE4GB/view?usp=sharing).
The image is in VirtualBox format, but you can also use it with QEMU.

To run QEMU on an Intel/AMD host, use `qemu-system-x86_64 -enable-kvm -m 8G -cpu host -vga qxl -hda vm.vdi` which runs the VM with 8 GB RAM and 1 CPU.
Add `-smp 2` to give it 2 cores.
On a Windows host, replace `-enable-kvm` with `-enable-hax`.

QEMU can also emulate x86 hardware on Apple Silicon, but in that case no hardware virtualization is available, so it will be very slow. Try something like:
`qemu-system-x86_64 -m 8G -cpu max -hda vm.vdi -vga qxl`
