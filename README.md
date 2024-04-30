# Server Setup - Add Client-PC

In this lab we will install and configure a Windows 10 Client PC and add it to our Domain we created in https://github.com/kendal-in-tech/Server-Setup---Active-Directory-

1. Download Windows 10 ISO from Microsoft Evaluation Center.

2. Install Windows 10 using Hyper-V. Specific guidelines for VM configuration depends upon your specific system. For my setup, I used 2048mb of Memory and 4 Virtual Processors. My Hard Drive size starts at 40GB but its dynamic (expandable). ![Screenshot 2024-04-29 195005](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/052a46aa-a6d8-4b5a-a10e-bbf12d6b61e3)

3. Allow install to complete. ![Screenshot 2024-04-29 195353](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/7262cc29-9a5d-459c-a6f7-41fb0e189baa)

4. Rename PC. Same as in Previous Lab.

5. I will now walk thru VM network setup. This setup is for the purpose of the lab. Network setup in actual environment may be different, how the same principles apply.

6. Power off both VMs. Go to Hyper-V settings and create a new Host-Based network adapter. Apply newly created network adaptors to both VMs. Start both VMs. 
![Screenshot 2024-04-29 201009](https://github.com/kendal-in-tech/Server-Setup-Add-Client-PC/assets/168005414/1c2714b6-cec6-4b04-a43d-3863e430c1bc)

7. 
