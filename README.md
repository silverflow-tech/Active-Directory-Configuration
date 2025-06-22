# Active-Directory-GPO-Configuration

This is a follow-up project for 'Windows 2022 Installation' and it will go over how to install and manage Active Directory. 

Step 1: Login to your Windows 2022 VM. If you don't know how to setup the VM for it, here is the link to my previous project > https://github.com/silverflow-tech/Windows-2022-Installation

![image](https://github.com/user-attachments/assets/67fbf06f-9ed0-4f3d-8e01-58cb4a63c58b)

Step 2: Click on the search bar at the bottom and type 'Server Manager'. Click on it and you will see the screenshot below

![image](https://github.com/user-attachments/assets/ed2d75eb-1406-4f3f-904f-5fff92211f33)

Step 3: Click on the 'Manage' tab > 'Add roles and features'

![image](https://github.com/user-attachments/assets/1d89c8ff-5b31-4962-9226-460f56a9c00e)

Step 4: You'll see the screenshot below and click 'Next'

![image](https://github.com/user-attachments/assets/84c988e9-7cef-4c97-a266-5d92ac4818af)

Step 5: For Installation Type, leave it at default for 'Role-based or feature-based installation' > Next

![image](https://github.com/user-attachments/assets/b124fd28-cd99-4e47-89a0-b24304a486eb)

Step 6: This will be default > Next

![image](https://github.com/user-attachments/assets/621f208d-ded4-49ee-a1e2-fb5b19d7fd94)

Step 7: Under the 'Server Roles' section, I'm going to select AD DS, DHCP, DNS, Remote Access, and Remote Access Desktop. You can follow along or you can add based on what you need accrodingly. 

![image](https://github.com/user-attachments/assets/b3583cdd-db96-4b30-9568-f1543ab981bd)

Step 8: Now we're going to got the "Features' section on the left side and confirm Group Policy Management' has been selected (Should be by default). Click 'Next' 

![image](https://github.com/user-attachments/assets/f2b198b0-2f6d-4964-bfa5-477a89b6e63c)

Step 9: Click 'Next" and add features based on what you selected before and click 'Install' when you're done

![image](https://github.com/user-attachments/assets/b304e351-09cd-462d-bea9-d168d3cfefe0)

Step 10: Once the installation is done, restart the server to complete the process

![image](https://github.com/user-attachments/assets/bb02cac9-26d6-4f80-8284-12b30e01e20b)

Step 11: Once you login, open 'Service Manager' and click on 'AD DS' if shown at the bottom or on the left menu tab

![image](https://github.com/user-attachments/assets/4aaf10c3-dca7-4ad2-a2ba-52fc762449ea)

Step 12: Click on the 'more' option for Configuration required...' and 'Promote this server to a domain' 

![image](https://github.com/user-attachments/assets/e14384e8-3661-445b-8407-93a3fc2f1a3c)

Step 13; Click on 'Add a new forest' and choose a root domain name. At the end of the domain name it must follow up with '.local' as shown below. 

![image](https://github.com/user-attachments/assets/fdf435d3-9e2d-40cf-8fda-ac4703eb20c1)

Step 14: Create a password DSRM password and click 'Next' 

![image](https://github.com/user-attachments/assets/3e9e35bf-67e2-4023-aded-d4bf363d0250)

Step 15: Install and it will automatically reboot. Log back in

![image](https://github.com/user-attachments/assets/b4eef6c8-3844-4704-8d2f-0d71895dea03)

Step 16: On the search bar, type in 'Active Directory Users and Computers'. Open the application

![image](https://github.com/user-attachments/assets/e05096a4-6b90-4df3-8928-8c0b0c8d77d7)

Step 16: Now I'm going to create new OU (Organizational Units). Right click on your domain controller > New > Organizational Unit

![image](https://github.com/user-attachments/assets/e994a536-7a29-45cc-837d-f0f096b95fa2)

Step 17: I'm going to create 3 OUs and then create 3 more OUs within each one. It should look like this

![image](https://github.com/user-attachments/assets/9e27c3ac-f657-414c-9e89-0ce7d2fbba20)

Step 18: Now we're going to create different groups for different departments. For this project, we're going to add IT, Accounting, HR, Sales, Sale, and Management. 

Go to one of your OUs > Users > Right click inside > New > Group. 

![image](https://github.com/user-attachments/assets/263f4b50-ab16-4284-b9eb-8ebc06f69746)

The final product should look like the screenshot below

![image](https://github.com/user-attachments/assets/0ef46a24-3f85-455e-a8be-b21cec8ee314)

Step 19: After creating the groups, it's time to create new users. Right click inside the OU > New > User.

![image](https://github.com/user-attachments/assets/fa28b29f-f67c-4e67-b70e-f7a0f9eb861d)

Step 20: Enter the information for the new user and create a password for the user

![image](https://github.com/user-attachments/assets/6ca18515-1ff0-4855-b9d5-2c832d2e2a6e)

Step 21: I've created 5 users as shown below. 

![image](https://github.com/user-attachments/assets/b3e5255c-cd25-408a-ad64-2ebec602357d)

Step 22: I'm going to organize this better by placing these users to the right group. I will place alice and bob to the 'Accounting Group', Chris and Jason to 'HR Group', and Paige to 'IT Group'

There are multiple ways you can do this. The method I'm going to use is by double-clicking on the group > Members > Add

![image](https://github.com/user-attachments/assets/54ede1dd-be89-44f7-860b-51c738cb5187)

Step 23: Enter the names you want to add to the group and click 'Check names'

![image](https://github.com/user-attachments/assets/70bbbca8-5c9c-40f1-b061-ec80d5e0b8e5)

Step 24: Confirm and click 'Apply' > 'Ok'

![image](https://github.com/user-attachments/assets/03b9d09b-c0c0-4f0a-8317-079830d01804)

Step 25: Do this for the other groups and that completes this project!






