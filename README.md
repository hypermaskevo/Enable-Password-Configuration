# Enable-Password-Configuration
This lab is designed to guide users through the process of configuring and securing privileged EXEC access on Cisco devices (Router and Switch) using Cisco Packet Tracer.
![image](https://github.com/user-attachments/assets/1b0f110a-1646-40c1-a064-053f0bbdd9dc)

🛠️ Lab Objectives
Change Hostnames
Rename the router and switch to R1 and SW1 respectively using global configuration mode.
Command example:

nginx
Копіювати
Редагувати
hostname R1
Configure an Unencrypted Enable Password
Set the enable password to CCNA on both devices.

Test the Password
Exit to user EXEC mode and test access with the password.

View Configuration
Use show running-config to view the unencrypted password.

Encrypt All Passwords
Ensure all passwords (current and future) are encrypted.
Command:

nginx
Копіювати
Редагувати
service password-encryption
Check Encryption
Use show running-config again to verify encryption.

Configure an Encrypted Enable Secret Password
Set a more secure password using the enable secret command.
Command:

bash
Копіювати
Редагувати
enable secret Cisco
Test Access with Enable Secret
Return to privileged EXEC mode and test the new password.

Analyze Encryption Types
Compare encryption types used for enable password and enable secret.

🖥️ Network Topology
Router: R1

Switch: SW1

End Devices: PC1, PC2, PC3

All devices are connected through the switch.

🔧 Technologies Used
Cisco Packet Tracer

Cisco IOS CLI

📁 How to Use
Open the .pkt file in Cisco Packet Tracer.

Follow the steps listed above or shown in the task area.

Use the CLI tab on each device to enter configuration commands.

📚 Useful Commands
bash
Копіювати
Редагувати
enable
configure terminal
hostname R1
enable password CCNA
service password-encryption
enable secret Cisco
exit
show running-config
📌 Notes
The enable secret password overrides the enable password.

Password encryption helps secure your device configurations from unauthorized access.

