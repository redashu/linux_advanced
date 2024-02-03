# linux_advanced

### problem 1 

<details><summary>show</summary>
<p>

 ## Assignment: Linux Permissions

### Objective:
Understanding and managing file and directory permissions in a Linux environment.

### Instructions:

1. **Create Users:**
   - Create three user accounts named `user1`, `user2`, and `user3`.

2. **Create Directories:**
   - Create a directory named `assignment`.
   - Inside the `assignment` directory, create two subdirectories named `docs` and `scripts`.

3. **Assign Permissions:**
   - Set the following permissions on the directories and files:
     - The owner should have read, write, and execute permissions.
     - The group should have read and execute permissions.
     - Others should have no permissions.

4. **File Operations:**
   - Inside the `docs` directory, create a file named `report.txt`.
   - Inside the `scripts` directory, create a shell script named `generate_report.sh`.

5. **Adjust Permissions:**
   - Adjust the permissions on the `report.txt` file to allow the owner to read and write, the group to read, and others to have no permissions.
   - Adjust the permissions on the `generate_report.sh` script to allow the owner to read, write, and execute, the group to read and execute, and others to have no permissions.

6. **Switch User and Verify:**
   - Switch to each user (`user1`, `user2`, and `user3`) and try to perform the following actions:
     - List the contents of the `assignment` directory.
     - Read the contents of `report.txt`.
     - Execute the `generate_report.sh` script.



</p>
</details>

### Problem 2 

<details><summary>show</summary>
 <p>


  ### Assignment: Advanced Linux Permissions

**Objective:**
Understanding and applying advanced Linux file permissions with additional complexity.

#### Instructions:

1. **Create Users and Groups:**
   - Create three users: `admin`, `developer`, and `guest`.
   - Create two groups: `team` and `public`.

2. **Create Directories:**
   - Create a directory named `project`.
   - Inside the `project` directory, create subdirectories named `source`, `documentation`, and `config`.
   - Inside the `config` directory, create subdirectories named `dev` and `prod`.

3. **Set Permissions:**
   - Assign the following permissions to the directories and files:
     - The owner of the `project` directory should be `admin` with read, write, and execute permissions.
     - The group of the `project` directory should be `team` with read and execute permissions.
     - Others should have no permissions on the `project` directory.
     - Apply the sticky bit to the `documentation` directory within the `project` directory.
     - Apply SGID to the `config` directory within the `project` directory.
     - Apply SUID to the `code.c` file within the `source` directory.
     - Create an ACL on the `settings.properties` file, allowing read access to the `developer` user.

4. **User Group Assignment:**
   - Add the `developer` user to the `team` group.
   - Add the `guest` user to the `public` group.

5. **Verify Access:**
   - Switch to the `admin` user and navigate to the `project` directory.
   - Try to create a new file in the `source` directory and edit `code.c`.
   - Switch to the `developer` user and attempt to view and edit `code.c` and `settings.properties`.
   - Switch to the `guest` user and attempt to view the contents of `manual.txt` and `settings.properties`.
   - Explain any unexpected behavior due to the sticky bit, SGID, SUID, or ACL.

6. **Document and Explain:**
   - Document the steps you took to set permissions.
   - Explain the expected results when users attempt to perform various actions.
   - Provide screenshots or output demonstrating the permissions, sticky bit, SGID, SUID, and ACL on directories and files.

7. **Advanced Challenge:**
   - Create a script named `permissions.sh` that, when executed by `admin`, automates the process of setting up the entire directory structure and permissions as described in steps 1-3, including sticky bit, SGID, SUID, and ACL.

**Note:**
- Ensure that you perform all actions as a user with appropriate administrative privileges.
- Use the `chmod`, `chown`, and `chgrp` commands to adjust permissions as needed.
- Explore and understand the impact of sticky bit, SGID, SUID, and ACL on file and directory access.

 </p>
</details>
