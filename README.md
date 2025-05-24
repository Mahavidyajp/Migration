# EX 6: MOVING FILES BETWEEN VIRTUAL MACHINES
## NAME: Maha Vidya J P
## REG NO: 212223220054
## Aim:
To move the files between virtual machine.
 You can move files between virtual machines in several ways:
•	You can copy files using network utilities as you would between physical computers on your network. To do this between two virtual machine:
•	Both virtual machines must be configured to allow access to your network.
•	Any of the networking methods (host-only, bridged and NAT) are appropriate. 
•	With host-only networking, you copy files from the virtual machines to the host and vice-versa, since host-only networking only allows the virtual machines see your host computer.
•	With bridged networking or NAT enabled, you can copy files across your network between the virtual machines.
•	You can create a shared drive, either a virtual disk or a raw partition, and mount the drive in each of the virtual machines.
## Procedure:
### How to Enable File sharing in VirtualBox. 
### Step 1: Install Guest Additions on the Guest machine. 

### Step 2: Configure File Sharing on VirtualBox. 
 

1. Start the Virtuabox Guest Machine (OS). 
2. From Oracle's VM VirtualBox main menu, select Devices > Install Guest Additions *

a. Open Windows Explorer

b. Double click at the "CD Drive (X:) VirtualBox Guest additions" to explore its contents.
		  
![image](https://github.com/user-attachments/assets/28840336-2711-43b4-96b0-acb77e141a22)


C.Right click at "VBoxWindowsAdditions" application and from the pop-up menu, choose "Run as administrator".
 
![image](https://github.com/user-attachments/assets/22ae6463-535d-4f4c-bce7-25b27de3dd38)


3.Press Next and then follow the on screen instructions to complete the Guest Additions installation.
	 
![image](https://github.com/user-attachments/assets/879e4ad7-8ccf-4c38-8886-cd1489cad274)


4. When the setup is completed, choose Finish and restart the Virtuabox guest machine.
   
### Step 3: Setup File Sharing on VirtualBox Guest Machine.

1. From VirtualBox menu click Devices and choose Shared Folders -> Shared Folder Settings.

![image](https://github.com/user-attachments/assets/fee92d3c-64e0-4577-95f6-a03eb5903cdc)


2. Click the Add new shared folder icon.

 ![image](https://github.com/user-attachments/assets/81ffd2a3-ddc3-4aeb-9167-d4f41cdc335f)


3. Click the drop-down arrow and select Other.
 

![image](https://github.com/user-attachments/assets/244a1979-7cbd-4436-8b33-358f59f05f0e)


3. Locate and highlight (from the Host OS) the folder that you want to share between the VirtualBox Guest machine and the Host and click Select Folder. *
* Note: To make your life easier, create a new folder for the file sharing, on the Host OS and give it with a recognizable name. (e.g. "Public")

![image](https://github.com/user-attachments/assets/aec08039-9ef6-41a6-b78e-2d3bf6a6f907)

4. Now, in the 'Add Share' options, type a name (if you want) at the 'Folder Name box, click the Auto Mount and the Make Permanent checkboxes and click OK twice to close the Shared Folder Settings.
 

![image](https://github.com/user-attachments/assets/e435f625-d1df-415f-9349-0969b4680509)


5. You 're done! To access the shared folder from the Guest OS, open Windows Explorer and under the 'Network locations' you should see a new network drive that corresponds to the shared folder on the Host OS.

## Result:

Thus the virtual machine files are moved to another VM.

