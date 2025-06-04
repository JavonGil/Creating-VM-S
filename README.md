![image](https://github.com/user-attachments/assets/d46d4750-4ffd-4390-bd31-0ea5687401bd)
<p align="center">
 
</p>

<h1>How To Create a Windows and Linux Virtual Machine in Microsoft Azure</h1>
I will be walking you through creating a Windows and Linux virtual machine (VM) in Azure. This skill set will be vital and is a key component to all of the IT projects listed. <br />

<h2>⚠️ Prerequisite</h2>

- <a href="https://azure.microsoft.com/en-us/pricing/purchase-options/azure-account/search?ef_id=_k_Cj0KCQjwzYLABhD4ARIsALySuCTvMpKHbOeSo9lv81A8vCg1XGDNwpOIuOsD2o8pmLnyl7dVku-Yn3IaApK-EALw_wcB_k_&OCID=AIDcmmfq865whp_SEM__k_Cj0KCQjwzYLABhD4ARIsALySuCTvMpKHbOeSo9lv81A8vCg1XGDNwpOIuOsD2o8pmLnyl7dVku-Yn3IaApK-EALw_wcB_k_&gad_source=1&gbraid=0AAAAADcJh_uVoYZIZMJRJFQ3v8k-BGmp2&gclid=Cj0KCQjwzYLABhD4ARIsALySuCTvMpKHbOeSo9lv81A8vCg1XGDNwpOIuOsD2o8pmLnyl7dVku-Yn3IaApK-EALw_wcB)">Microsoft Azure account</a> 

<h2>💻 Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)

<h2>🖥️ Operating Systems Used </h2>

- macOS Sequoia
- Windows 10 Pro (21H2)
- Ubuntu Server 22.04

<h2>✅ High-Level Steps</h2>

- Step 1: Creating a Resource Group in Azure
- Step 2: Creating the Windows VM in Azure
- Step 3: Creating the Linux VM in Azure

<h2>Demonstration Below</h2>

<h3> Step 1: Create a Resource Group in Azure </h3>

- After creating your account in Microsoft Azure navigate to the home page.<img width="1512" alt="Screenshot 2025-06-04 at 11 02 03 AM" src="https://github.com/user-attachments/assets/b92171a5-00dd-46a2-a448-9d9d7849493a" />

</p>
<br />

<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 05 40 AM" src="https://github.com/user-attachments/assets/92adb06b-f05f-4608-8a13-a0a84f6f6864" />
</p>
<p>
- Locate the Search Bar at the top of your screen and type "resource". Notice the options that populate as you type "resource" into the search bar. Select Resource Groups.
</p>

<br />

<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 06 21 AM" src="https://github.com/user-attachments/assets/fa2ccfc9-d5c7-4962-a9ee-58f31719e6ef" />
</p>
<p> - There should be no resource groups in sight. Click the + Create button and let the games begin!</p>
<br />
<br />

<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 07 54 AM" src="https://github.com/user-attachments/assets/5f3cfbfb-8630-45eb-9b19-77641dcdcf9d" />
</p>
<p>
 
 1. The Subscription box should reflect whatever you chose when setting up your Azure account. If you do not see that, click the drop down arrow to find it. 
 
 2. Name your Resource Group (Project-IT). This group is where our VMs will be stored in the Cloud.
 
 3. Next, choose the Region. *Tip: Select (US) East US 2 for ALL Region options. Making sure the Region matches for eveything we create.* Now click next at the bottom of the screen.
</p>
<br />

<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 08 29 AM" src="https://github.com/user-attachments/assets/d5fab9e9-1367-4fba-ad91-7e908039d65c" />
</p>
<p>
- Review the information and click Create. Make a mental note or write down the name and region you used for future reference. 
</p>
<br />

<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 09 29 AM" src="https://github.com/user-attachments/assets/eeb23a45-ef1c-44f8-b07d-c1ddc18c35fc" />
</p>
<p>
- After clicking Create you will be directed back to the RG (Resource Groups) section. You have successfully created your Resource Group in the Cloud. Now let's create some VMs! </p>
<br />

<h3> Step 2: Creating a Windows VM in Azure </h3><p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 10 41 AM" src="https://github.com/user-attachments/assets/e6492563-9a74-47a4-ad45-b3b0c3d91712" />
</p>
<p>
- From this screen, locate the search bar again and enter "vm". Select "Virtual machines" from the options. This will direct you to the Virtual Machines section.
</p>
<br />

<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 11 13 AM" src="https://github.com/user-attachments/assets/764b9a9f-17ae-49c5-a56e-e2a0028f47b5" />
</p>
- Simply click the + Create button to get started.
</p>
<br />

<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 11 47 AM" src="https://github.com/user-attachments/assets/eebba9f3-eeca-44db-8360-c65d025cee9c" />
</p>
<p>
 - Select the first option, "Azure virtual machine" from the drop down and click + Create button.
</p>
<br />

<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 13 24 AM" src="https://github.com/user-attachments/assets/e8ce4bd3-48ac-4826-9af1-2cb5b2a9bd6d" />
</p>
<p>
 - Your subscription should already be selected.
 
 1. Choose the RG we created earlier.
 
 2. Name the VM "windows-vm".
    
 3. Select the same Region as before. "(US) East US 2". *We want the RG and Region to be the same for everything we are creating.*
    
 4. Select "Windows 10 Pro, version 22H2" for the Image. This will be the Operating System (OS) for the VM. *Do Not select a Windows Server*
</p>
<br />

<p>
<img width="750" alt"CVM 6" src="https://github.com/user-attachments/assets/8d66c106-64c0-4ad1-a9ec-0f0c5570a014" />
</p>
<p>
 - Scroll down to select the Size. We want to use the "Standard_D2s_v5 - 2 vcpus, 8 GiB memory".</p>
<p>- If you do not see this listed, click "See all sizes" to get more options. Sometimes the Region selected can cause this specific size to not appear. Make sure the size you pick has at least 2 vcpus and 8 GiB memory.
</p>
<br />

<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 14 38 AM" src="https://github.com/user-attachments/assets/82adabbf-1c47-455f-8101-c2523391726d" />
</p>
<p>
 - Next, you will create a username and password for the VM. We will need this to log on later with a Remote Desktop Connection (RDP). *Highly recommend writing down this information for later.*</p>
<p>- Now, locate the Licensing area towards the bottom of the screen. You will need to check the box to confirm. This is required because we are creating a Windows VM. Deployment will not work if left unchecked. Click "Next: Disks" then "Next: Networking" to move on.
</p>
<br />

<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 18 09 AM" src="https://github.com/user-attachments/assets/8e8b08e4-dd32-4fdf-932c-173fbccd57e4" />
</p>
<p>
 - Azure may auto populate a Network name for you. Go ahead and create a new one. Just note what you named the Networt, we will need it for the Linux VM. You can leave the rest alone and use the Default settings. Azure will automatically assign the Subnet and Public IP for you. Leave the RDP Port as well. We will need access the VM via Remote Desktop Connection later. Click "Review + create" button.
</p>
<br />

 - Review all the informatiom for the Windows VM. Our Subsciption, RG, and Region are correct. We named the VM "windows-vm". The Image and Size are correct and we have RDP active. Simply click "Create".
</p>
<br />

<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 23 40 AM" src="https://github.com/user-attachments/assets/ba796dc7-a01c-4cf2-a260-2eef0de08fcb" />
</p>
<p>
 - Once you click "Create", the Deployment of the Windows VM will begin. This can take a few minutes. When it's completed you will see "Your deployment is complete". Congrats! We just created our first Virtual Machine in the Cloud. Click "Create another VM" to get started on the Linux VM.
</p>
<br />

<h3> Step 3: Create a Linux VM in Azure </h3>

<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 29 28 AM" src="https://github.com/user-attachments/assets/fee7af76-e7b5-43f9-9219-f4783743d75d" />
</p>
<p>
Select the same RG that we created earlier. Name the VM "linux-vm" and choose the same Region as before. Since this will be the Linux VM, select "Ubuntu Server 22.02" for the Image.
</p>
<br />


<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 30 35 AM" src="https://github.com/user-attachments/assets/1c0a29f2-6714-4319-b822-c823db3c94e1" />
</p>
<p>- Choose the same Size option as before. "Standard_D2s_v5 - 2 vcpus, 8 GiB memory". </p>
<p>- Next, you will need to select "Password" for Authentication type. Azure defaults to SSH public key. Then, create a Username and Password. You can use information as the Windows VM to keep it simple. Once you are done, scroll done and click "Disks". Leave these options as default and skip to "Networking". 
</p>
<br />

<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 32 38 AM" src="https://github.com/user-attachments/assets/33e0e3c7-639e-49bf-aaf7-c89e4081d132" />
</p>
<p>
- Make sure to select the same Virtual Network that we created earlier. We can leave everything else as default. Scroll down and click "Review + create".  
</p>
<br />

<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 33 52 AM" src="https://github.com/user-attachments/assets/2e85d857-ec96-4e99-866c-d9df3e36bae7" />
</p>
<p>
- On the next screen you will see the deployment of the Linux VM in progress. This may take a few minutes.  
</p>
<br />

<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 35 27 AM" src="https://github.com/user-attachments/assets/35e7f18d-4cfa-4aa5-bf9e-c298b763d7e3" />
</p>
<p>
- The Linux VM has been successfully created.   
</p>
<br />

<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 35 53 AM" src="https://github.com/user-attachments/assets/0643dbc7-9387-4a33-a6c1-e8f5805a9412" />
</p>
<p>
- Locate the search bar at the top of the screen and type in "virtual". Select "Virtual machines" and you will be direct to your newly created VMs!
</p>
<br />

<p>
<img width="1512" alt="Screenshot 2025-06-04 at 11 36 00 AM" src="https://github.com/user-attachments/assets/7961c4f4-78a1-4891-8561-2c396ad4d528" />
</p>
<p>
- You can view the Windows and Linux VMs we created in the Cloud. You will notice the RG and Locations match, what OS they are running, Public IP addresses, and more! </p>
<p> *Pro Tip: Notice the Start, Restart, and Stop buttons above the OS and Size area. You can use these to "turn off", "turn on" , or "restart" the VMs like you would your physical PC or Laptop. To save on your subsricption, you can "Stop" the VMs from running while you are not using them. Just make sure to "Start" them when you are ready to use them again. If you want extra practice, you can simply delete the RG and recreate everything as needed.*   
</p>
<br />

<h2>🎉 Project Wrap Up</h2>

<p>
And that’s a wrap. In this project, we successfully created a Resource Group, a Windows VM running Windows 10 Pro, and a Linux VM running Ubuntu, all hosted in the cloud. Along the way, we got a hands-on look at the power of cloud computing and virtualization how simple it is to spin up multiple machines without needing physical hardware. With just a MacBook, I was able to set up and access two additional machines running completely different operating systems. No clutter, no pricey setups, just pure cloud efficiency. </p>
<p>This is a perfect example of why businesses are leaning heavy into Cloud Service Providers (CSPs) the flexibility, scalability, and cost effectiveness are game changers. Before we go, don’t forget to Stop your VMs in Azure when you're done to avoid unnecessary charges. Thanks for following along and being part of this journey. See you in the next project same energy, new level 😎      
</p>
<br />
