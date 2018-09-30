# macOS-Sierra-VM
Tutorial on how to setup a macOS Sierra Virtual Machine

For my projects I make use of macOS Sierra Virtual Machine, as I like to devide security research, development and personal use.
I can imagine more people would like to organize their environments like that, therefore I will help you setting up a VM.

## Requirements
- At least 4GB of ram (bare minimum), 8GB would be way better
- A intel core i3, i5, i7 or Xeon Quad or Eightcore processor (Any Intel processor will do, but these are the best).
- Around 80GB of free harddisk space.
- VMWare Workstation (not player, as that will not have VMWare tools).
- Windows 7 or Higher (x64), Linux 64-bit.

## Setup
- For the best VM usage, disable unnecessary Windows animations, C:\Windows\System32\SystemPropertiesPerformance.exe
- You will need to have a license key for VMWare Workstation.
- Here are some licenses that can be used.
  YA3JU-AWY9P-M882Z-2PX79-WCRE8  
  5A02H-AU243-TZJ49-GTC7K-3C61N  
  VZ1XR-66GEM-H899Q-35P59-P688A  
  FZ59H-2QDE5-M8EZP-DNPZ9-N6AC8  
  CY740-8MG55-H8ELQ-VQN7E-MP0C4  
  AZ3M0-4UG92-481PQ-EEPEZ-NGUA4  
  CY7J0-6EW85-089RZ-EMNXZ-QGAUA  
  UG548-4TDD6-4818Y-LPQQX-QA0GF  
  YU712-DRGDQ-H884Z-J7MZE-MCATF  
  GC1ER-21W4K-H80HY-REWQX-ZCUE4  
  YV7TR-8EF95-085MP-WWXQG-MC8R0  
  UZ7ER-89D0L-M85CZ-L7MQT-MY0CF  
  GV1H2-D4F95-089EP-ZNM7C-WCKR2  
  VC7R8-DZE9K-4819Y-M4WXG-Z6UYA  
  GZ1H2-6FD80-0843Z-4GMQC-PVUR2  
  UY14A-88E1P-M88AZ-5YQE9-YLHG0  
  VG5XK-DTYEM-M887P-DYZXE-Q72V6  
  CZ3WA-AXZ8Q-489VP-A6Z7V-P20Z4  
  VV31H-A8Z1J-H84PZ-57NEG-XFRF4  
  CY5M8-FGF42-M8DUQ-AMY7G-NAH92  
  UA1HR-FFZEQ-489HY-YGQ5C-NZHZ8  
  AG5DH-8HF42-081UZ-XDM5C-X3UD6  
  UY7JA-0HY85-M81VZ-DGZ7E-YUUR2  
  AZ5EA-A2Y45-H893Y-ZYZZT-Z6RYD  
  CA118-A0Y1M-089YQ-Y4XE9-PQAG0  
  GY1NR-A5XD4-0815Y-GGQQT-ZA8ED  
  CA5H2-64Z1J-489PQ-UWNQZ-ZZ2A0  
  CC5RR-46D43-080PY-TXWGX-QAKW6  
  UG11H-F8G11-M885Y-CFY5Z-Q3H9D  
  GZ3N2-02WE2-489ZZ-UEYXG-PG8V2  
  VC31K-DZYD3-089LY-HYQEX-W3RV6  
  UC3R8-A2X14-H80WP-Q5YET-QGAU8  
  UV70U-A6E17-H8DGP-5XNE9-WCAD4  
  CV3T0-DYGDK-480RY-LNZ7T-YU2F4  
  MU20T-8X15J-RZYY9-QH07M-1270P  
  NG63J-4KLD1-HZP49-P8CQM-12Q2J  
  NV6EA-21K8L-NZ6M8-P19Q0-CCL0Q  
  4F4W7-6624N-CZVN0-03AQ0-03TPR  
  
- Download the vmdk of Sierra at https://goo.gl/pBVDXz
- Download the VMWare Patch tools at https://goo.gl/bZsv5f
- Extract the vmdk rar file using WinRar or any other rar extraction software.
- Make sure you have VMWare workstation installed.
- Extract the patch tools
- Rightclick win-install.cmd and choose "Run as Administrator"
- Open VMWare workstation and create a new VM.
- Choose "I will install the operating system later"
- Choose macOS from the list of Operating systems in the next step.
- Edit the VM settings to your likings, preferably half of your computer memory should be allocated to the VM and all processor cores.
- Remove the harddisk and re-add a new harddisk
- In the next step, Browse to the extracted vmdk.
- Go to C:\Users\yourusernamehere\Documents\Virtual Machines
- Go into the macOS Sierra folder
- Open the .vmx file in your favorite text editor
- Add the following after the last line: smc.version = "0"
- Save the file and boot the virtual machine
- Follow the macOS installation steps
- Install VMWare tools
- Reboot
- Congratulations, you successfully set up a macOS Sierra VM.
