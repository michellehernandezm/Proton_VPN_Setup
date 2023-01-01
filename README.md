<p align="center">
<img src="https://i.imgur.com/Grb44gD.png" height="70%" width="70%" alt="ProtonVPN logo"/>
</p>

<h1>Proton VPN - Setup and Usage</h1>
This tutorial outlines the process of retrieving and observing IP addresses of computers in different locations. We will observe our own desktop IP address, then the IP addresses within a Azure virtual machine. We will use Proton VPN to change our IP address and observe the changes. <br />


<h2>Video Demonstration</h2>

- ### [How To Install Proton VPN with Prerequisites](https://clipchamp.com/watch/owUcTrGNUxf)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)


<h2>Installation Steps</h2>

<p> Step 1 : On your desktop, go to (https://whatismyipaddress.com/) and locate your IPv4 adress and location.
<img src="https://i.imgur.com/37yHrFL.png" height="80%" width="80%" alt="Proton_VPN_Setup"/>

 Once you open the website, it will have the current location of your device and the IPv4 address. Take note of these details.
</p>
<br />


<p> Step 2 : Create Virtual Machine (VM) in Azure.
 <img src="https://i.imgur.com/65vRsY7.png" height="80%" width="80%" alt="Proton_VPN_Setup"/>

In your Azure portal, "create" a new Virtual Machine and fill in with the following:
 
- VM Name: VPNPractice
 
- Region: Europe France Central
 
- Image: Windows 10
 
- Size: 2vcpus
 
- Username: labuser
 
- Password: (create something you will remember)
 
 Once all information is filled click "Review + Create"
 
</p>
<br />

<p> Step 3 : Connect to VM through Remote Desktop.
<img src="https://i.imgur.com/JHkENa8.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>

 Once VM is created copy the "Public IP Address"

 

<img src="https://i.imgur.com/vhO3b4K.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>


<p>
Open up "Remote Desktop" in a Windows computer or "Microsoft Remote Desktop" in a Mac. Paste the Public IP address and "Add" the PC. Once added, continue with the username and password you created back in Step 2.
</p>
<br />

<p> Step 4 : Inside the VM open (https://whatismyipaddress.com/) again and locate your VM's IPv4 address and location. 
<img src="https://i.imgur.com/XVa490G.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The location for your Virtual Machine should say Paris, France.  Take note of the IPv4 addresss and location for future reference.
</p>
<br />

<p> Step 5 : Create an account with Proton VPN. 
<img src="https://i.imgur.com/0cqZPPT.png" height="80%" width="80%" alt="create"/>
 
 
 In your regular browser (not VM browser) search the web for https://protonvpn.com/ and click on "Create a free account" 
</p>
<br />
 
<img src="https://i.imgur.com/XnQFxbS.png" height="80%" width="80%" alt="get free account"/>
 
  You will then be directed to a new page with pricing options, be sure to scroll down and click "Get VPN Free"
 </p>
<br />
 <img src="https://i.imgur.com/T2Sdz1j.png" height="80%" width="80%" alt="create user"/>

  Proceed to create your personal account.
</p>
<br />

<p> Step 6 : Download Proton VPN. 
<img src="https://i.imgur.com/hTC0mJk.png" height="80%" width="80%" alt="Download proton vpn"/>
</p>
<p>
Go back to VM and log into your newly created Proton VPN account. From your dashboard, locate the "downloads" tab from the left hand side of the page. Locate the Windows option and click "download"
</p>
<br />
<img src="https://i.imgur.com/fS1f0w1.png" height="80%" width="80%" alt="Download proton vpn"/>
</p>
<p>
 
 Click "Download Proton VPN" for Windows and follow instructions to complete installation.
</p>
<br />

<p> Step 7 : Connect to Japan Virtual Private Network.
<img src="https://i.imgur.com/88VzKS8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

 Open your new Proton VPN app to see this screen. Observing the IP Address, it should match the IP address from Step 4.
 </p>
<br />
 
 <img src="https://i.imgur.com/yIuPcQV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 Hover mouse over "Japan" and click "Connect"

 </p>
<br />
 
 
 <img src="https://i.imgur.com/l87Tpj4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
As you connect to the Japan VPN your remote desktop connection may freeze. Reload remote desktop and see that you are now connected to the Japan server.
</p>
<br />

<p> Step 8 : Open up (https://whatismyipaddress.com/) to view changes.
<img src="https://i.imgur.com/jglmi2J.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Your Virtual Machine has a new IP address located in Japan!
</p>
<br />

<p> Step 9 : Browse through websites.
 
<img src="https://i.imgur.com/voXnfNz.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/DdruEyP.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<p>
Search for websites like google.com, Netflix, or Starbucks. Enjoy your exploring!
</p>
<br />


<p> Step 10 : Delete Virtual Machine.
 
<img src="https://i.imgur.com/DPBJBdT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/T2VpIPn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<p>
It's now time to delete your resources on Azure. Be sure to delete the "VPNPractice" virtual machine and the resource group. Finally, log off of Remote Desktop and you're done!
</p>
<br />
