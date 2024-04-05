# CYBER FORENSICS EXPERIMENT
### K P Uday Krishna
### CB.SC.P2CYS23012

## Investigating a suspicious USB pendrive found at a crime scene. The forensic team needs to acquire evidence from the pendrive while ensuring the integrity of the data. Using the dd and dc3dd commands, create a forensic image (.img) file of the pendrive. Additionally, generate a SHA-256 hashfile for the image file to verify its integrity. Finally, wipe the pendrive using the disk wipe pattern 00011 to prevent any potential data leakage. 

> **Run the commands and take a snapshot and submit it in a word document**

![Screenshot 2024-04-05 191317](https://github.com/udayk01/Cyber-Forensics/assets/52235763/fb45ec9f-536a-4e38-8678-72f9de4830cf)

- **We would insert our usb drive and enter the command ```fdisk –l```**
  
![image](https://github.com/udayk01/Cyber-Forensics/assets/52235763/da95ee8e-fa79-4d1c-b2eb-5313c8027bd4)

- **We create a disk image of inserted usb drive**

  ```dd if=/dev/sdb1 of=disk.img```

![image](https://github.com/udayk01/Cyber-Forensics/assets/52235763/45b87b1a-3810-401a-8e45-059776d1e791)

- **We verify the created disk image file and delete it.**

![image](https://github.com/udayk01/Cyber-Forensics/assets/52235763/ea5ff204-1dd2-448d-b4eb-87f522263a52)

- **We can also create disk image by explicitly specifying block size and adding error handling to it**



## DC3DD

### Now install dc3dd

![image](https://github.com/udayk01/Cyber-Forensics/assets/52235763/36a56a84-ba7d-418c-9c26-e934bd8e7f4b)

- man dc3dd
  
![image](https://github.com/udayk01/Cyber-Forensics/assets/52235763/ff9be93c-3573-4fef-9e9b-7d8fa0c051c4)

- Again we have to enter fdisk –l command and insert usb drive

![image](https://github.com/udayk01/Cyber-Forensics/assets/52235763/59088eda-5453-41e7-bdba-5e30aa00d5bb)

- We have to split usb with the help of dc3dd tool

  ```dc3dd if=/dev/sdb hash=sha256 log=split_usb ofs=test.img.000 ofsz=500M```

