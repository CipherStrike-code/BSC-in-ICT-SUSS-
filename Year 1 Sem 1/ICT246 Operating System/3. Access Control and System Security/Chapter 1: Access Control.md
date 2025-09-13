## Access Control Overview
**What is Access Control?**
Access Control is the process that determines who has access or is allowed to access certain apps, data and resources, and under what circumstances.

**Why do we need Access Control?**
It helps to ensure that our OS is secure and that only authorised users are allow to perform certain taks. It also helps to improve overall security against malware, as the malware dont have permission to execute certain permission if we have access control. 

Types of Access Control:
1. Mandatory Access Control (MAC)
2. Discretionary Access Control (DAC)
3. Role-Based Access Control (RBAC)

**Mandatory Access Control**
- Access is based on **security labels** and **security clearances**.
- Labels can be applied to objects such as files.
- Clearances can be applied to subjects such as a user.
- User cannot grant hist or her clearance to another person to access a particular object.
- Clearance to the is set by a main body but the permission to the clearance is automaticaly done by the system.
- E.g. A staff with a security clearance of confidential cannot access items above the label of confidential (e.g. secret)

**Discretionary Access Control**
- Access is controlled by the owner of the object and access rules that state which subjects can perform which actions on that object.
- DAC allows each user to control access to his or her own objects
- It is flexible, and allows users or subjects to grant access rights to other subjects
- Can sometimes become messy as you do not know who you grant the permissions to
- E.g. Google Document, Emails

**Role-Based Access Control**
- Access Control is based on the roles that the subjects have, and on rules that state which roles have what access to which object.
- Usually, a role is a job function wihtin an organisation
- Access are given to roles, instead of individuals and every user is assigned roles which can be same or different
- Not as flexible as DAC, but is easier to manage as it is centrally controlled

## File Access Control
- A general model for file access is represented as and access matrix
- The basic components of the model are
  - subject
  - object
  - access right
- In a server OS, usually users group instead of users are created as the subjects, and folders that contain files are being used as objects.
<p align="center">
  <img width="690" height="888" alt="image" src="https://github.com/user-attachments/assets/229cdbb9-5267-4965-951a-ea3286389d77" /><br>
  <img width="1003" height="866" alt="image" src="https://github.com/user-attachments/assets/d869e811-ee37-4a53-846a-4cb1142be0e4" />
</p>




















































