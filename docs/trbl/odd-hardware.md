---
title: 'Hardware with unique requirements'
taxonomy:
    category:
        - docs
visible: true
---
### Tongfang-GK5C6Z

boot param: acpi_osi=! acpi_osi=‘Windows 2009’   
Custom kernel compiled with pinctrl-cannonlake module enabled is needed.    
(This will fix the Touchpad and give you better performance overall.)    
Neither, Optimus, Bumblebee nor the next-gpu.sh work as solutions currently a solution is to disable discrete GPU via acpi_call    

 All three HDMI ports are wired to the GTX1060 which means no extra screens. For best performance  have the core and cache undervolted to -130mV.    
    
 Written by 99-0    

&nbsp;

[Using Parrot](https://docs.parrotlinux.org/info/start/) | [Troubleshooting](https://docs.parrotlinux.org/trbl/start/) | [Linux Beginner Guide](https://docs.parrotlinux.org/library/lbg-basics/) | [Home](https://docs.parrotlinux.org/)