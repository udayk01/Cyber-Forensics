# CYBER FORENSICS EXPERIMENT
### K P Uday Krishna
### CB.SC.P2CYS23012

## Investigating a suspicious USB pendrive found at a crime scene. The forensic team needs to acquire evidence from the pendrive while ensuring the integrity of the data. Using the dd and dc3dd commands, create a forensic image (.img) file of the pendrive. Additionally, generate a SHA-256 hashfile for the image file to verify its integrity. Finally, wipe the pendrive using the disk wipe pattern 00011 to prevent any potential data leakage. 

> **Run the commands and take a snapshot and submit it in a word document**

![Screenshot 2024-04-05 191317](https://github.com/udayk01/Cyber-Forensics/assets/52235763/fb45ec9f-536a-4e38-8678-72f9de4830cf)

- We would insert our usb drive and enter the command ```fdisk –l```
  
![Screenshot 2024-04-05 191530](https://github.com/udayk01/Cyber-Forensics/assets/52235763/13d4adc5-c9fc-44d3-a955-34c0ccd3858a)

- We create a disk image of inserted usb drive

  ```dd if=/dev/sdb1 of=disk.img```
  
