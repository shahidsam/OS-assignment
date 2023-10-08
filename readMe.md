# Author Name:Md Shahidul Alam icdcp_78
# ProjectName: OS-assignment
I have created a basic OS project for OS assignment for DevOps Course.

## Recommended installation Process:
1. Clone the repository in local.
2. Create a user with user group:
    ## sudo useradd -m -s /bin/bash icdcp-78
3. Create two directories in user's home directory:
    ## sudo mkdir /home/icdcp-78/os-concepts /home/icdcp-78/ubuntu-is-the-best
4. Create two files in each directory:
    ## sudo touch /home/icdcp-78/os-concepts/file1 /home/icdcp-78/os-concepts/file2
    ## sudo touch /home/icdcp-78/ubuntu-is-the-best/file1 /home/icdcp-78/ubuntu-is-the-best/file2
5. List the files with detailed information (including file permission):
    ## ls -l /home/icdcp-78/os-concepts/
    ## ls -l /home/icdcp-78/ubuntu-is-the-best/
6. Update file permission:
    ## sudo chmod 640 /home/icdcp-78/os-concepts/* /home/icdcp-78/ubuntu-is-the-best/*
7. Create another group
    ## sudo groupadd shahid_78
8. Update file ownership to the newly created group:
    ## sudo chown username:shahid_78 /home/username/os-concepts/* /home/shahid_78/ubuntu-is-the-best/*
9. Add the user to the new group:
    ## sudo usermod -aG shahid_78 icdcp_78

10. Create a file called crash.in in different directories and include the word "crash" in it:
    ### Let's say we're creating these in /tmp and /var/tmp directories.
    ## echo "crash" | sudo tee /tmp/crash.in > /dev/null
    ## echo "crash" | sudo tee /var/tmp/crash.in > /dev/null

11. Find the file in all the locations using the find command:
    ### This will search from root for crash.in. The 2>/dev/null part discards error messages.
    ## find / -name crash.in 2>/dev/null

12. Replace the lines with "crash" to "broken" in all found files:
    ## find / -name crash.in 2>/dev/null | xargs sed -i 's/crash/broken/g'











## Recommended IDE Setup
