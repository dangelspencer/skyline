# Part 1 - Description of overall test plan  
For this project, we will be using an automated testing framework for Nodejs called Jest. The purpose of using this automated testing framework is to be able to run tests before changes are made, to verify that existing functionality is not improperly affected by new code updates. We will be doing both unit and integration tests. Unit tests will verify that various functions work on their own and integration tests will verify that different parts of the project will work together in the correct way. Testing a function that calculates pay rates based on server usage would be a unit test. Testing repository methods to verify that the correct data is returned based on certain parameters would be an integration test.  

# Part 2 - Test Case Descriptions  
1. AT-1: Login Test  
* Purpose - Verify that a user is able to login  
* Description - Sends test login credentials to verify that a user receives a HTTP 200 response  
* Inputs - Username, password  
* Expected Outputs - HTTP 200 response (login accepted)  

2. AT-2: Edit personal information  
* Purpose - Verify that a user is able to update their personal information  
* Description - Sends a post with updated email address to verify that the email address can be properly changed in the DB  
* Inputs - Email address  
* Expected Outputs - HTTP 200 response  

3. AT-3: Change password  
* Purpose - Verify that a user is able to update their password  
* Description - Sends a post with current and new passwords to verify that the user’s password is able to be properly updated  
* Inputs - Current password, new password  
* Expected Outputs - HTTP 200 response  

4. AT-4: Update notification preferences
* Purpose - Verify that a user is still able to update their notification preferences  
* Description - Sends a post with an integer that relates to the type of notification preferences that they prefer  
* Inputs - Integer  
* Expected Outputs - HTTP 200 response  

5. AT-5: VM Creation  
* Purpose - Verify that virtual machines can be created from the application  
* Description - Test that virtual machines can be created using the triton datacenter api  
* Inputs - VM object  
* Expected Outputs - VM created in Triton datacenter with no errors  

6. AT-6: VM actions  
* Purpose - Verify that virtual machines can be stopped, started, and rebooted  
* Description - Collection of tests that confirm that vms on triton datacenter can be started, stopped, and rebooted  
* Inputs - VM ID and requested action  
* Expected Outputs - HTTP 200 response from triton (no errors)  

7. AT-7: VM Deletion
* Purpose - Verify that a virtual machine can be deleted  
* Description - Test to confirm that a virtual machine is deleted from triton datacenter when requested by the program  
* Inputs - VM ID  
* Expected Outputs - The vm should be removed from Triton datacenter with no errors  

8. AT-8: VM and User grouping  
* Purpose - Verify that only VMs assigned to a user are returned from the database  
* Description - Test will confirm that when a user views a list of virtual machines, they will only be able to see the ones that they’ve created.  
* Inputs - User ID  
* Expected Outputs - List of virtual machines belonging to the user  

9. AT-9: Network Addition
* Purpose - Verify networks can be created  
* Description - Test will confirm that a network can be created to host VM’s  
* Inputs - Network name, IP range or subnet  
* Expected Outputs - HTTP 200 response from triton (no errors)  

10. AT-10: Network Deletion  
* Purpose - Verify networks can be deleted  
* Description - Test will confirm that a network can be deleted if an only if no VM’s are hosted on that network  
* Inputs - Network ID  
* Expected Outputs - HTTP 200 response from triton (no errors)  

11. AT-11: Network Health  
* Purpose - Verify health of network  
* Description - This verifies if the specific network is reachable  
* Inputs - IP Address  
* Expected Outputs - HTTP 200 response from triton (no errors)  

12. AT-12: Network Deletion  
* Purpose - Verify networks with VM’s attached cannot be deleted  
* Description - Try to delete a network with VM’s attached  
* Inputs - Network ID  
* Expected Outputs - HTTP 500 response from triton (can’t delete network)  

# Part 3 - Test Matrix  
| Test | Normal/Abnormal/Boundary | Blackbox/Whitebox | Functional/Performance | Unit/Integration |
|:-----|:------------------------:|:-----------------:|:----------------------:|:----------------:|
|AT-1|Normal|Whitebox|Functional|Integration|
|AT-2|Normal|Whitebox|Functional|Integration|
|AT-3|Normal|Whitebox|Functional|Integration|
|AT-4|Normal|Whitebox|Functional|Integration|
|AT-5|Normal|Blackbox|Functional|Integration|
|AT-6|Normal|Blackbox|Functional|Integration|
|AT-7|Normal|Blackbox|Functional|Integration|
|AT-8|Normal|Blackbox|Functional|Integration|
|AT-9|Normal|Blackbox|Functional|Integration|
|AT-10|Normal|Blackbox|Functional|Integration|
|AT-11|Normal|Blackbox|Functional|Integration|
|AT-12|Abnormal|Blackbox|Functional|Integration|
