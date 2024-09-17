# How to run an Omeka-S Docker image on MacOS.
For this guide we will be using the following repository from the Ghent University: https://github.com/GhentCDH/Omeka-S-Docker.git

1. In your system, open a terminal. You can do this by pressing Cmd + Space to open Spotlight, typing "Terminal," and pressing Enter.
2. Navigate to the Applications Folder
In this folder the Omeka-S-Docker folder will be placed, if you rather place the folder somewhere else then navigate to that folder. I recommend not placing it in a Download folder.
To navigate to the Applications folder using the terminal, use the cd command:
```bash
cd /Applications
```

3. Verify Your Current Directory
To ensure that you are in the correct directory, use the pwd command:
```bash
pwd
```

4. Clone the Git Repository
```bash
git clone https://github.com/GhentCDH/Omeka-S-Docker.git
```
This command will create a new folder named Omeka-S-Docker inside the Applications directory and copy all files from the repository into this folder.
5. To verify that the repository has been cloned successfully, list the contents of the Applications directory:
```bash
ls
```
6. You should see a directory named Omeka-S-Docker in the output. Now you can navigate to this folder:
```bash
cd Omeka-S-Docker
```
Now we will closely follow the instruction from the repo with some extra clarification steps and notes.


