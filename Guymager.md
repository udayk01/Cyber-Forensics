## K P Uday Krishna 
## CB.SC.P2CYS23012
## Imagine you're a digital forensic analyst working on a case involving a USB pendrive suspected to contain crucial evidence. Detail the steps you would take to acquire the evidence and recover files from the pendrive using the following tools: Guymager for creating a dd file, and Foremost for file recovery. Explain each step of the process, from connecting the pendrive to your forensic workstation to generating a dd file using Guymager, and then recovering files using foremost.

> First we would insert our usb drive.

![image](https://github.com/udayk01/Cyber-Forensics/assets/52235763/04b6b24b-4026-49fc-9b0f-e59f38ab00b8)

> Then i am going to delete the image from this usb.

![image](https://github.com/udayk01/Cyber-Forensics/assets/52235763/183da45e-3293-4ebd-b094-36e39022fadc)

> Press Delete

![image](https://github.com/udayk01/Cyber-Forensics/assets/52235763/f6a1cf70-1f70-4373-a77a-2312a07636fe)

> Now i am going to create a disk image using Guymager.

### Guymager for creating a dd file

> Now we run guymager in our Kali Linux system. To run this tool we simply use ```guymager``` command in our terminal window.

```sudo guymager```

> Providing command will open it's window as following:

> In that will specify all the disk connected to the device.

![image](https://github.com/udayk01/Cyber-Forensics/assets/52235763/29dc189b-6354-4f74-92c0-2db18113f618)

![image](https://github.com/udayk01/Cyber-Forensics/assets/52235763/4cfc9a2c-dcb7-4a7a-abf6-eff7d7504942)

> Here we can see that we can clone the pen drive on our hard disks or any other flash drives. To acquire image we need to right click on the disk and select the acquire option.

![image](https://github.com/udayk01/Cyber-Forensics/assets/52235763/03759cb5-c4c4-4a41-8f36-0758deef3402)

> And a new window will pop up.

![image](https://github.com/udayk01/Cyber-Forensics/assets/52235763/0c860901-f5af-4e4d-93c4-9c68376f216d)

> Here we can choose the file format and provide the case number and evidence number, examiner, descriptions and notes. Here we can also choose the image directory. We can also split the size of disk. We can calculate MD% and SHA1 and SHA-256. Then we must check the verification process, because if the image acquisition was not valid then it can't be an evidence. So verification is a good habit. Here we have done everything, and set the acquired image directory in our desktop, and we did not used the split image because we are not acquiring large image. Following screenshot shows the process.

![image](https://github.com/udayk01/Cyber-Forensics/assets/52235763/c99fd012-0e33-4d12-a15c-936aa664ca2a)

> Then we just click on start option and the process will started.

![image](https://github.com/udayk01/Cyber-Forensics/assets/52235763/b372b54b-72b8-47d5-9fd6-579da0435a4b)

> After finishing this process we will get a dd image file in our specified folder.

![image](https://github.com/udayk01/Cyber-Forensics/assets/52235763/e2b4a93c-1c38-4618-beb9-96bc776bdf6c)

> now we will use dd image to recover the image by using ```Foremost``` tool

