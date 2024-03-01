# UTM | Apple Silicone | Linux Virtualization
<h1>Hector M. Reyes  | SOC Analysts </h1>
</h1> Group 17: Script K™</h1>
<h1>  Comprehensive Guide: <br />
Setting up Linux Virtual Machines using <br />
UTM for M1 & M2 Apple Silicone </h1>

 ### [Fullstack Academy - Capstone Project](https://docs.google.com/document/d/1mizcEhlYScNc8-_g/edit)


<h2>Purpose</h2> 
Our team faced some challenges when setting up our SIEM lab environment. Team members using Apple silicon-based computers encountered difficulties creating virtual machines on their personal computers. We were able to resolve this issue by using UTM, a virtualized environment that is designed for M1 and M2 Macs. This allowed our team members to have Linux distributions on their computers that they could use on the go. We created a tutorial to help other information security professionals and students facing similar issues. 
 
<h2>Tools & Environments Used </h2>
- <b> UTM (Universal Type Manager) | QEMU | Virtualization
</b>  <br />
- <b> Kali Linux | Architecture: ARM64
- <b> Memory: 4 GiB | Disk: 64 GiB </b>
<br /> <br />

<img src="https://i.imgur.com/8Wic9mu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <br />

<h2> Description </h2> 
Accessing type 2 hypervisors can be daunting for security professionals and students when deploying Linux distributions on their Apple Mac computers. To add to the complexity, the affordable versions of hypervisors like VMware and VirtualBox can be incompatible, further complicating the access of Linux distributions on Apple Computers. However, there is a solution to this problem - UTM. By leveraging virtualization, UTM can act as a front end to Apple's built-in hypervisor, a macOS feature, allowing us to access Kali Linux - a Debian-based distribution. It's worth noting that these steps can be used to virtualize other Linux distributions, such as Ubuntu or RedHat distributions like CentOS.
<br />  <br />  
<img src="https://i.imgur.com/ap10O7K.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  <br />

<br />
 
<img src="https://i.imgur.com/gfOvXDn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />  

<h3> What is Kali Linux? <h3>
Kali Linux is a free and open-source Debian-based Linux distribution. It comes with a comprehensive set of pre-installed tools and utilities specifically designed to perform various cybersecurity testing such as penetration testing, digital forensics, and security audits. 
 
<br /> 

<img src="https://i.imgur.com/pGFHB6D.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <br />

1. Penetration Testing Tools: <br />
Kali Linux includes many penetration testing tools for assessing the security of networks, systems, and applications. These tools range from network scanners and vulnerability assessment frameworks to exploitation tools and password crackers. 

2. Digital Forensics Utilities: <br />
Kali Linux provides robust digital forensics capabilities, allowing users to conduct investigations, analyze digital evidence, and recover data from various storage media. It includes tools for disk imaging, file carving, memory analysis, and forensic analysis of network traffic.

3. Security Assessment Frameworks: <br />
Kali Linux incorporates popular security assessment frameworks such as Metasploit and Burp Suite, which enable professionals to identify vulnerabilities, exploit security flaws, and simulate real-world cyber attacks. These frameworks streamline the process of security testing and help organizations improve defenses.

4. Wireless Network Testing: <br />
Kali Linux offers specialized wireless network testing and exploitation tools. Users can perform wireless network reconnaissance, capture and analyze network traffic, and assess the security of Wi-Fi networks using tools like Aircrack-ng and Wireshark.

5. Web Application Security: <br />
Kali Linux includes tools for testing the security of web applications, APIs, and web servers. It provides scanners for identifying common web vulnerabilities such as SQL injection, cross-site scripting (XSS), command injection, and web application fuzzing and exploitation tools. 

6. Exploitation Frameworks:  <br />
Kali Linux features comprehensive exploitation frameworks like Metasploit, allowing users to develop and execute custom exploits against vulnerable systems and applications. These frameworks facilitate the discovery and exploitation of security weaknesses in target environments.

<img src="https://i.imgur.com/ZaJJJ4n.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />  <br />  

Pre-installed Tools: <br />
Some pre-installed tools and utilities available in Kali Linux include: 
- <b> Nmap: Network scanner and reconnaissance tool. 
- <b> Wireshark: Network protocol analyzer. 
- <b> John the Ripper: Password cracking tool. 
- <b> Burp Suite: Web application security testing framework. 
- <b> Metasploit Framework: Exploitation framework for developing and executing exploits.
- <b> Aircrack-ng: Wireless network assessment tool. 
- <b> Volatility: Memory forensics framework. 
- <b> Hydra: Password brute-forcing tool. 
- <b> Nikto: Web server vulnerability scanner.  <br />

<img src="https://i.imgur.com/kAqGa69.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br /><br />  

Usage and Community:  <br />
Kali Linux is widely used by cybersecurity professionals, penetration testers, ethical hackers, and security enthusiasts worldwide. Its extensive documentation, community forums, and online resources make it accessible to users of all skill levels. The active community of contributors and developers ensures regular updates, bug fixes, and improvements to the distribution, keeping it at the forefront of cybersecurity testing and research. 
 

Summary<br />
Kali Linux is a versatile and powerful platform for conducting cybersecurity assessments, digital forensics investigations, and security research. Its comprehensive set of pre-installed tools, user-friendly interface, and active community support make it an indispensable resource for professionals and enthusiasts in information security. 

<br />  

<h2>What is UTM?</h2> 
UTM (Universal Type Manager):  <br />
UTM (Universal Type Manager) is a virtualization platform designed explicitly for macOS, developed by Felix Schwarz. It enables users to run virtual machines (VMs) on their Mac computers, allowing them to use multiple operating systems simultaneously without additional hardware. UTM offers a user-friendly interface and robust functionality, making it an ideal choice for users seeking to leverage virtualization for various purposes, including software testing, development, education, and more. 

<br /> 

Key Features: <br />
1. Versatile Virtualization: <br />
UTM supports various guest operating systems, including Windows, Linux, macOS, and BSD distributions. Users can create and manage multiple virtual machines with different configurations to suit their needs.

2. Performance Optimization: <br />
UTM utilizes QEMU (Quick Emulator) as its virtualization backend, providing efficient performance and compatibility with various hardware platforms, including Apple Silicon (ARM64) chips found in Mac M1 and M2 computers. 

3. User-Friendly Interface: <br />
UTM offers an intuitive graphical user interface (GUI) that simplifies creating, configuring, and managing virtual machines. Users can easily customize VM settings, allocate resources, and install guest operating systems with minimal effort. 

4. Hardware Acceleration: <br />
UTM supports hardware acceleration features like OpenGL acceleration to enhance virtualized environments' performance and graphical capabilities. This ensures smooth operation and optimal user experience, particularly when running resource-intensive applications and graphical workloads. 

5. Integration with macOS: <br />
UTM seamlessly integrates with macOS, allowing users to leverage native system features and resources within virtualized environments. This includes support for peripherals, file sharing, networking, and other macOS functionalities, enhancing the interoperability and usability of virtual machines on Mac computers. 

6. Open-Source Foundation: <br />
UTM is built upon open-source technologies, with its source code available on GitHub for community contribution and collaboration. This open development model fosters innovation, transparency, and continuous improvement, ensuring that UTM remains a reliable and cutting-edge virtualization solution for macOS users.

<img src="https://i.imgur.com/azTPDJR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br /> <br />  

</h3> Usage and Applications: </h3> <br />
UTM is utilized by a diverse user base, including software developers, system administrators, educators, and hobbyists, for various purposes: <br />

1. Software Development and Testing: UTM enables developers to create isolated development environments, test software compatibility across different operating systems, and evaluate application performance under various configurations.
 
2. Education and Training: UTM is a valuable tool for educational institutions and training providers, allowing students to explore different operating systems, practice system administration tasks, and learn about virtualization concepts hands-on. <br />

3. System Administration and Maintenance: System administrators use UTM to simulate network environments, troubleshoot system issues, and perform maintenance tasks without affecting their primary macOS environment. 
Security Research and Testing: UTM supports the creation of virtualized security testing environments, facilitating the evaluation of cybersecurity tools, techniques, and procedures in a controlled and isolated environment.<br />

<br /> 

<img src="https://i.imgur.com/WSK2lK0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />  <br />  

Summary <br />
UTM is a versatile and powerful virtualization platform for macOS, offering various features and capabilities to meet users' needs across various industries and disciplines. Its intuitive interface, robust performance, and integration with macOS make it an indispensable tool for running virtual machines on Mac computers and exploring different operating systems and software environments. 

<br /> 

<h2> Why does Kali and UTM work so well? </h2> 
Key Features: <br />

1. ARM64 Compatibility: <br />
Kali Linux provides official builds optimized explicitly for the ARM64 architecture used in Apple's M1 and M2 chips. This compatibility ensures that Kali Linux can run smoothly on Mac computers equipped with these processors when virtualized using UTM. 

2. QEMU Virtualization Backend: <br />
UTM utilizes QEMU (Quick Emulator) as its virtualization backend, which is a versatile and powerful emulator that supports a wide range of hardware platforms and architectures, including ARM64. This allows UTM to emulate the ARM64 architecture required to run Kali Linux on Mac M1 and M2 systems. 

3. Hardware Acceleration Support: <br />
UTM supports hardware acceleration features, such as OpenGL acceleration, which can enhance virtualized environments' performance and graphical capabilities. This ensures that Kali Linux, running within a UTM virtual machine, can leverage hardware acceleration for responsiveness and visual fidelity.  

4. Integration with macOS: <br />
UTM seamlessly integrates with macOS, providing native support for peripherals, file sharing, networking, and other macOS functionalities within virtualized environments. This integration ensures smooth interoperability between Kali Linux and macOS, allowing users to access and utilize macOS resources seamlessly while running Kali Linux in a virtual machine. 

5. Ease of Use: <br />
UTM offers an intuitive user interface that simplifies creating, configuring, and managing virtual machines. Users can easily set up a Kali Linux virtual machine within UTM without complex configurations or technical expertise, making it accessible to users of all skill levels. 

6. Community Support: <br />
Kali Linux and UTM benefit from an active and vibrant community of users, developers, and contributors who provide support, feedback, and resources. This collaborative ecosystem ensures that users can find assistance, troubleshooting tips, and guidance when running Kali Linux on UTM, enhancing the virtualization setup's overall user experience and reliability. 

<br /> 
</h3>Summary </h3> <br />
Kali Linux works well with UTM due to its ARM64 compatibility, hardware acceleration support, macOS integration, ease of use, and strong community support. Together, these factors contribute to a seamless and reliable experience for users seeking to run Kali Linux on Mac M1 and M2 systems using UTM as the virtualization platform. <br />  

<img src="https://i.imgur.com/6ZvyGJm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />  

<h2> How to install and use Kali Linux and UTM: </h2>
1. Download UTM and Kali Linux: <br />
- <b> Navigate to the UTM Website: Open your web browser and go to https://mac.getutm.app to access the UTM website.
 
 <br />  
 
<img src="https://i.imgur.com/GF6X6LG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
 
Download UTM:  <br />
On the UTM website, locate the download button and click on it to initiate the download process. 

<img src="https://i.imgur.com/yps0uW1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

Install UTM:  <br />
Navigate to your "Downloads" folder once the download is complete.
Locate the downloaded UTM file (usually in .dmg format) and double-click to open it.
Drag the UTM icon to your "Applications" folder to install UTM on your Mac. 

<img src="https://i.imgur.com/LoZPARL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 


Download Kali Linux: <br />
Visit the Kali Linux website at https://www.kali.org/get-kali/#kali-platforms. 

<img src="https://i.imgur.com/AgItYjq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

Find the image: <br />
Click the download icon and select the latest Kali Linux version compatible with Apple Silicon (ARM64).

<img src="https://i.imgur.com/eTtLgxj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

<img src="https://i.imgur.com/SN1eJbP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

<br /> 

2. Verify Kali Linux Download: <br />
Navigate to your "Downloads" folder once the download is complete. 
Verify that the downloaded Kali Linux file is intact and complete.

<br />  

3. Creating a Virtual Machine in UTM: <br />
Open the UTM application from your "Applications" folder.
 
<img src="https://i.imgur.com/DydQBuC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Create a New Virtual Machine: <br />
Create a New Virtual Machine: In UTM, select"Create a New Virtual Machine" to begin the setup process. Create a New Virtual Machine

<img src="https://i.imgur.com/te0olrC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

Select Virtualize Option: <br />
Choose the "Virtualize" option and select"Linux" as the operating system for the virtual machine. 

<img src="https://i.imgur.com/ALiII9F.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

<img src="https://i.imgur.com/PuzxN82.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

Choose the Kali Linux ISO: <br />
Opt not to use Apple Virtualization and proceed with QEMU. 
Browse and select the Kali Linux ISO image downloaded earlier. 

<img src="https://i.imgur.com/9WHJozr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

Specify RAM Allocation: <br />
Specify the desired amount of RAM allocation for the virtual machine (e.g., 6GB) for optimal performance. 
Enable hardware OpenGL acceleration for smooth graphical performance. 

<img src="https://i.imgur.com/hEUaFst.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

Allocate Storage Space: <br />
Allocate default storage space (e.g., 64GB) for the virtual machine's storage. 

<img src="https://i.imgur.com/gO3Vf4E.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

<br /> 

4. Virtual Machine Configuration: <br />
Rename Virtual Machine:  <br />
Rename the virtual machine to a descriptive name (e.g.," Kali Linux") for easy identification.

Add Serial Device: <br />
Navigate to the "Settings" tab and add a new serial device in the devices section. 

<img src="https://i.imgur.com/cnXH5O1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

<img src="https://i.imgur.com/zpPaZtK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 


Grant Disk Access: <br />
Ensure that UTM has full disk access by granting permissions in your Mac's system settings under "Privacy and Security." 

<img src="https://i.imgur.com/ztKhWgm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

<img src="https://i.imgur.com/alxZMxx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

Reboot UTM: <br />
If necessary, reboot UTM to apply the changes made to disk access permissions. 

<br /> 

5. Installation of Kali Linux: <br />
Initiate Installation Process: 
Reopen UTM and initiate the installation process by selecting the start I

<img src="https://i.imgur.com/5hhUTlY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

<img src="https://i.imgur.com/aTr2gX2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

Follow On-Screen Prompts: <br />
Follow the on-screen prompts to select the Kali Linux system's language, location, keyboard configuration, hostname, domain, username, and password. 

<img src="https://i.imgur.com/bBa0cMu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

<img src="https://i.imgur.com/rmCD90I.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

<img src="https://i.imgur.com/hV2Qw7M.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

<img src="https://i.imgur.com/LrYMBTX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

Guided Partitioning: <br />
Select the timezone and proceed with guided partitioning (use the entire disk) for the installation.

<img src="https://i.imgur.com/I6PPe45.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

<img src="https://i.imgur.com/gwpku5V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

Software Selection: <br />
Choose software selection options based on your requirements. 

<img src="https://i.imgur.com/Ct3yepQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

Wait for Installation: <br />
Wait for the installation process to complete

<img src="https://i.imgur.com/588rHmM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

<img src="https://i.imgur.com/ImNlGf1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br />

6. Post-Installation Configuration: <br />
Reboot UTM: <br />
Upon receiving the "Finish the Installation" prompt, continue and reboot UTM to apply the changes. 

<img src="https://i.imgur.com/LsC4NYS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

Clear CD/DVD Option: <br />
Re-launch UTM and clear the CD/DVD option in the settings. 

<img src="https://i.imgur.com/B0uYAad.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

Start your Virtual Machine: <br />
Start the virtual machine and select the Kali Linux option. 

<img src="https://i.imgur.com/iJJcaBU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

<br /> 

7. Terminal Setup and Update: Open Terminal: <br />
Open Terminal: <br />
Open the terminal within Kali Linux.

<img src="https://i.imgur.com/Cb4hVoi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

Execute Commands: <br />
Execute the following commands to install necessary packages, update repositories, and upgrade existing software within the virtual machine.


<img src="https://i.imgur.com/if43yBG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

<br /> 

<img src="https://i.imgur.com/vyvufdZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br /><br />

</h2>Conclusion </h2> <br />
This comprehensive run book offers a detailed and easy-to-follow guide for setting up Kali Linux on UTM for Mac M1 and M2 computers. With this step-by-step instruction manual, you can ensure a smooth and hassle-free installation process. Not only that but the same set of instructions can be used to install other operating systems as well, making it an indispensable reference for anyone looking to install an OS on their Mac.

<br /> <br />

<img src="https://i.imgur.com/pw4NvMC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />

<img src="https://i.imgur.com/AggZzny.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>










