# Server Setup - Add Client-PC


![2](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/8405af26-7c75-4fc9-974f-f7e648320411)


In this lab we will install and configure a Windows 10 Client PC and add it to our Domain we created in https://github.com/kendal-in-tech/Server-Setup---Active-Directory-

1. Download Windows 10 ISO from Microsoft Evaluation Center.

2. Install Windows 10 using Hyper-V. Specific guidelines for VM configuration depends upon your specific system. For my setup, I used 2048mb of Memory and 4 Virtual Processors. My Hard Drive size starts at 40GB but its dynamic (expandable). ![Screenshot 2024-04-29 195005](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/052a46aa-a6d8-4b5a-a10e-bbf12d6b61e3)

3. Allow install to complete. ![Screenshot 2024-04-29 195353](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/7262cc29-9a5d-459c-a6f7-41fb0e189baa)

4. Rename PC. Same as in Previous Lab.

5. I will now walk thru VM network setup. This setup is for the purpose of the lab. Network setup in actual environment may be different, how the same principles apply.

6. Power off both VMs. Go to Hyper-V settings and create a new Host-Based network adapter. Apply newly created network adaptors to both VMs. Start both VMs.
   
![Screenshot 2024-04-29 201009](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/272d4e44-b18a-4291-931e-9847088f744a)

7. On Client - PC VM, navigate to the network settings. 

![Screenshot 2024-04-29 201820](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/7e104836-c853-4db0-871f-efe04a3a30e4)

8. Navigate to Network Properties. We want to edit the DNS settings. 
![Screenshot 2024-04-29 201820](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/ba195033-04d2-434b-9f81-516878e33c18)

![Screenshot 2024-04-29 201934](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/9f8945bd-fd34-4e9c-8200-2fa184920e6d)

![Screenshot 2024-04-29 201953](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/f7b1c1bf-8165-414b-89b1-22d4459daca5)

9. Go to the Server - DC - PC and use CLI, run IPCONFIG and get the IP address to the server. We will use this as the DNS server of the client PC.

![Screenshot 2024-04-29 202211](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/181a39a3-275c-41d0-a0bc-a57effd95c47)

![Screenshot 2024-04-29 202354](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/3aad8d55-db4e-4b80-a5a6-55f8c7fc5012)

11. On Client - PC, navigate to "Access Work or School" in Settings. Enter Administrator and Adminstrator Credentials. from previous Lab. 

![Screenshot 2024-04-29 211930](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/ab4b27d2-5f0b-4680-b91b-2054985b027f)

12. Restart PC.

![Screenshot 2024-04-29 212001](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/997dc9d3-9caf-4f8b-8524-134486e87aa4)

13. Verify Login after restart. ![Screenshot 2024-04-29 212053](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/f9238724-8390-403e-b0ac-60f8288866d2)

14. System should ask for password reset. Reset is needed since this is the first time logging in as this newly created user. (User created in previous lab.) 

![Screenshot 2024-04-29 212108](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/082f3b0b-341a-4b7f-a39d-25223404f351)

15. OPTIONAL: Check users in CLI using command: net user /domain on Client - PC. 

![Screenshot 2024-04-29 212414](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/f99f6710-1b72-4cb8-ab54-8d8f2ad52417)

The Client - PC is now connected to the Domain we created in the Previous Lab.

We will continue to use this same Lab setup in Future Labs.

Create new users, and make sure that you can login into the Client PC.


![2](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/ff2d0930-d90e-4683-b100-9d4dfe040a34)




