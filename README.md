This is just a noobs attempt to get som use out of his old Huawei Matebook. Use the information on this reposotory at your own risk.
90% of the EFI is from the hard work over at https://github.com/tlefko/Huawei-Matebook-X-Pro-Ventura/tree/main

I have mainly just brute forced my way into getting it to work.
Followed the intructions on https://dortania.github.io/OpenCore-Install-Guide/ to make an booteble usb with my wanted OS then triel and error to get it working. 

As of today the wifi is working with Heliport but the audio is something i cant fix.

To get Imessage and Facetime working i had to use Opencore configurator to set up Serial nr.

To get a clean boot add <data></data> after line 1419 <data>hwcAAA==</data> don't know what it does but i get a clean boot no materix. You have to remove line <data></data> to be able to use opencore config. OPS sync the file before you save or opencore deletes it and you have to pull it again.

if anyone has the tecnical knowhow to fix the audio or im able to stumble into it then ill update this.

I'm making this seperate reposotory because i don't want to poisen the good work telfko and the othes have been doing the EFI thats here is not optimal but its working and after my testing it seems to be stable.

The Specs on my Huawei Matebook x Pro 2018 is

Processor	Intel Core i7-8550U
Memory	16 GB LPDDR4 2133 MHz
SSD	LiteON SSD PCIe NVMe 512 GB [CA3-8D512]
Graphics	NVIDIA GeForce MX150 (Disabled) / Intel(R) UHD Graphics 620
Display	3K Display @ 3000 x 2000 (13.9 inch) @ 60hz
Sound Controller	Realtek ALC256
Wireless Card	Intel Dual Band Wireless-AC 8265
Bluetooth Card	Intel Bluetooth 8265