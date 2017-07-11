# Tp-link-W8960NV5-firmware-source-code


download link https://drive.google.com/file/d/0B3jG8LulloMTTjVjYThyTlU4b28/view?usp=sharing


### step 1 

+ Decompress the archive with your favorite tool.
+ Use the ./prepare script to install and decompress uclibc and source or do this manually moving the toolchain to / opt.


### step 2      
      
+ cd TD-W8960Nv5.0_consumer 
+ make PROFILE=W8960NV5

                                                     
### step 3
      
+ Flash the firmware using Broadcom CFE bootloader https://wiki.openwrt.org/doc/techref/bootloader/cfe
      
   
### NOTE
      
The image produced is fully functional , some nodes have been modified for the correct startup and the interface of the     uhttpd webserver has been modified. You can add new binary and more .To restore the original image , download the right firmware version and then do 
     

## dd if=original_firmware.bin bs=1 of=stripped_firmware.bin skip=512
      
      
![Preview](https://raw.githubusercontent.com/Sputkin/Tp-link-W8960NV5-firmware-source-code/master/img/wbs.png)


