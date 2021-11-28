# UTS SAS
------
## Fiandio Adhi Pradhana(1202192034)/IT 02-01
------
**Question**
------
<img width="461" alt="bbbb" src="https://user-images.githubusercontent.com/92350603/143621126-49a7a818-0d3d-4a3f-b737-ff4fafdae37f.PNG">

**Answer**
------
### A. Instalasi windows server 2022

Download ISO Installer windows server 2022

   https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2022
   
   Select download the `ISO` then follow it step by step.
   
   <img width="874" alt="cccc" src="https://user-images.githubusercontent.com/92350603/143621513-6da949ad-311d-4c4b-af20-f8dc3031a9e4.PNG">

- Then open `Oracle VM`
 
 
 
 ![OPEN VB](https://user-images.githubusercontent.com/93086665/143688074-1e9de5ea-e3f0-44ef-8c16-547681064c7e.png)

- Next Klik `New`, and do it like the picture below :
  
  Enter the name of the machine and type of system to use


- Define ram, create the disk defining type and size

![3](https://user-images.githubusercontent.com/93086665/143722345-0528ad07-049e-47b6-91a7-00b4834220b5.png)
![4](https://user-images.githubusercontent.com/93086665/143722363-d042dbb9-33f1-460d-8a9a-01d48018d799.png)

- Go to the machine configuration and in the `Network` section set `Bridge adapter`

![image](https://user-images.githubusercontent.com/93086665/143722408-fc63d1ac-2ade-4494-86e1-6ad482d828c0.png)
-  Click on `Start` and select the `ISO downloaded`


-  Click on `Start` and the Windows Server 2022 installation wizard will load
![1](https://user-images.githubusercontent.com/93086665/143688385-8fb46fe9-6674-48ca-be82-2af467a7a9e4.png)

-  Click on `Install now`
![2](https://user-images.githubusercontent.com/93086665/143688386-f00383d2-f111-4f3f-86bd-d79309dde0cf.png)

- Select windows server 2022 desktop experience
![3](https://user-images.githubusercontent.com/93086665/143688387-2da4ce6e-eaba-4707-931b-863002423ede.png)
- Accept the license and then proceed with the installation of Windows Server 2022
![4](https://user-images.githubusercontent.com/93086665/143688388-9e9b1d19-ec7f-4b16-927b-1871a9b79d6c.png)
- Select windows server 2022 install microsoft server advanced (Custom)
![5](https://user-images.githubusercontent.com/93086665/143688381-20ec0dbe-e8c1-4f9f-ba8e-0715439e9076.png)
- Location installation of windows server 2022
[6](https://user-images.githubusercontent.com/93086665/143688382-07e463a9-1fb1-491e-8146-091373ce2f29.png)
- installation progress
![7](https://user-images.githubusercontent.com/93086665/143722442-0da9bae5-d4a5-45e0-9b15-9868c6f7fa1c.png)
- The system will reboot to complete the process

![BOOTING WINDOWS (2)](https://user-images.githubusercontent.com/93086665/143722530-833a14d0-725a-4edb-80b5-2195c30152a3.png)

- Next, custom your password administrator

- Access the menu `Input – Keyboard – Insert Ctrl + Alt + Del`. Enter the password created and wait for the configuration to load

![TAMPILAN AWAL](https://user-images.githubusercontent.com/93086665/143722478-b77c8eca-69dd-47f8-86c0-611bfbaf3178.png)

- Windows Server 2022 has been successfully installed

![TAMPILAN AWAL WINDOWS](https://user-images.githubusercontent.com/93086665/143722493-37a16165-230d-475b-bf36-61b2f67afe09.png)



### B. Instalasi Active Directory Domain Services
-  Before doing the installation, we change the computer name first by going to windows powershell.
   Then type `rename-computer -Newname Server2022`
      - Open the start menu and select `Windows PowerShell`
      
  ![B  WINDOWS POWERSHELL](https://user-images.githubusercontent.com/93086665/143722868-25ab2409-05d3-4542-b113-6d1fac8c153b.png)
  ![B RENAME COMPUTER SERVERS](https://user-images.githubusercontent.com/93086665/143722798-213c2174-9a76-4581-a2e7-ec4ca66a5d53.png)

      - Then Restart, and open`Server Manager`
      
 ![B SERVER MANAGER (2)](https://user-images.githubusercontent.com/93086665/143722836-143ef68f-ad1a-4c83-ac82-be412a56a234.png)
 
      - Select Menu `manage`, Then `Add Rules and Features` 
      
  ![B ADD ROLES](https://user-images.githubusercontent.com/93086665/143722885-429434d5-bb79-4bfd-b2ac-44a9c113fccb.png)

      - Select Next
      
   ![B NEXT ADD ROLES](https://user-images.githubusercontent.com/93086665/143722909-cc04bd92-e755-4e32-af5a-26dfebcd6da3.png)

      - Select option`Role-based or feature-based installation`. And `Next`
      
  ![B  ROLES-BASED OR FEATURE](https://user-images.githubusercontent.com/93086665/143722933-8c5aa3b4-1019-4138-a9ad-8148277da9ba.png)

      - Click `Select a server from the server pool` to select a local storage directory. Then `Next`
      
   ![B  SELECT DESTINATION](https://user-images.githubusercontent.com/93086665/143722938-e6f7c5e3-418b-47ba-adad-c0e03a96eae9.png)

      - Next, put a check mark in the `Active Directory Domain Services` box. When you check the box, on the right appears 
        a brief description of ADDS and how it works. Then click `Add Features`.
   ![B  ACTIVE DIRECTORY DOMAIN](https://user-images.githubusercontent.com/93086665/143722957-b4c01094-0bbc-482b-bfab-2aa80fa646f7.png)
   
   
### C. Instalasi DNS server
   - We need to install and configure the Active Directory role and DNS server to work together.
     Checklist `DNS Servers` then `add features` 
     
   ![B  DNS SERVER SESUDAH DI KLIK](https://user-images.githubusercontent.com/93086665/143722986-75624927-dc29-44e8-805d-0783e49873fc.png)


### D. Instalasi Net Framework 3.5
   - Checklist `.NET Framework 3.5 features`
  
  ![D NET FRAMEWORK](https://user-images.githubusercontent.com/93086665/143723019-5d4920c6-8eb8-412a-9aae-266bb1ec5cd0.png)

   - Click `Next`
   
  ![D  ACTIVE DIRECTORY DOMAIN SERVICES](https://user-images.githubusercontent.com/93086665/143723039-2c79a72f-8192-48c0-be2e-ffeeb65e3f3c.png)

   - Click `Next`again
   
  ![D  NEXT AGAIN](https://user-images.githubusercontent.com/93086665/143723063-5a34ba98-4ee2-40df-bb6d-37a969e5d895.png)

   - Select `Install`
   - 
 ![D  INSTALL NETFRAMEWORK](https://user-images.githubusercontent.com/93086665/143723077-2b560258-3d66-48b5-b0d8-475b2ff70a51.png)

   - Success 
   
 ![D](https://user-images.githubusercontent.com/93086665/143723084-2a183397-13c1-4ba5-b48a-b282b44e333a.png)

### E. Promote Server to a Domain Controller
-  Setting to static ip using `cmd`, type `sconfig  

![E1](https://user-images.githubusercontent.com/93086665/143723810-e4089002-7ff2-4b22-9558-abc606b70c08.png)

-  Setting the IP Address Server-ADDS and pointing the DNS to the static IP address used.

![E2 1](https://user-images.githubusercontent.com/93086665/143723840-a2bd080c-d488-47cd-860c-e820b34fb9f7.png)

-  Click `Promote this server to a domain controller` for ADD configuration

![E3](https://user-images.githubusercontent.com/93086665/143723848-9d812fdd-14e8-4e2f-b842-62060a86ca46.png)

-  Select `Add a new forest` and enter the domain name to be used in the Root Domain Name. For example here I use the domain `fiandio.com`

![E4](https://user-images.githubusercontent.com/93086665/143723870-2f2748b3-e155-4ec2-a2d5-24b547264555.png)


-  Select `Windows Server 2016` at the functional level, put a check mark on `Domain Name System (DNS) server` and `Global Catalog (GC)`. 
   And fill in the Directory Services Restore Mode password with strong password criteria.
   
![E5](https://user-images.githubusercontent.com/93086665/143723883-c1df59dc-4764-451a-8e4e-0855f3e8878e.png)


-  then click `Next`

![E6](https://user-images.githubusercontent.com/93086665/143723892-f94c265d-b337-4c6b-9797-e4b2cd854749.png)


-  Fill in `The NetBIOS domain name` according to the domain name used.

![E7](https://user-images.githubusercontent.com/93086665/143723897-5ba725b4-b43e-4abb-acef-84780824c361.png)

-  Skip the Paths section, click `Next`.

![E8](https://user-images.githubusercontent.com/93086665/143723911-efcba842-2701-4a0a-a2ea-e9ab53836257.png)

-  Check the configuration specified in `Review Options`, if it is TRUE. Click `Next`.

![E9](https://user-images.githubusercontent.com/93086665/143723920-10e4aa99-9cc9-46dc-9c98-4916dc68b5e8.png)

-  If there is `All prerequisite checks passed successfully.` Click `Install` to apply the specified configuration.

![E10](https://user-images.githubusercontent.com/93086665/143723929-3c2f0cc1-a2e2-4795-929c-4bc4266cf64f.png)

-  After the installation is complete, the laptop will restart automatically. Then login using administrator password

![E11 2](https://user-images.githubusercontent.com/93086665/143723936-b1a41035-4a6c-41e4-acc4-4c0f79778ce5.png)
![E12](https://user-images.githubusercontent.com/93086665/143723953-c7053eb5-5185-46ba-a048-0fb162d9c086.png)
![E13](https://user-images.githubusercontent.com/93086665/143723949-84571778-7042-4ea8-8ffb-35e47fcf033f.png)
-  To check the configuration results, open cmd and type `netdom query fsmo`

![E14](https://user-images.githubusercontent.com/93086665/143723970-df0f7f78-d66f-41fe-bae8-312e4deb91c2.png)
![E15](https://user-images.githubusercontent.com/93086665/143723968-c47aad85-c4d5-4d48-81de-8e8fb8b230d0.png)

Selesai 






