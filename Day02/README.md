Cybersecurity Class – How We Installed and Ran Kali Linux
In this session, we learned how to install Kali Linux, a popular operating system used by cybersecurity professionals and ethical hackers.

We first tried installing Kali Linux using Oracle VirtualBox, but it didn’t work well on MacBooks with Apple Silicon (M1/M2 chips). So, we switched to UTM, another virtual machine app, and were able to install Kali Linux successfully.

**Part 1: Trying to Install Kali Linux Using VirtualBox
 *Step 1: Download and Install Oracle VirtualBox
          Go to https://www.virtualbox.org.
          Click on "Downloads".
          Choose macOS / Intel hosts (Note: VirtualBox doesn’t fully support Apple Silicon yet).
          Download the .dmg installer file.
          Open it, then drag VirtualBox into your Applications folder.
          Open VirtualBox from your Applications.
*Step 2:  Download the Kali Linux ISO File
          Go to the Kali Linux official website: https://www.kali.org/get-kali/
          Look for "Kali Linux ISO Images".
         Download the Installer ISO version (64-bit), such as:
         kali-linux-2025.2-installer-amd64.iso
*Step 3: Set Up a New Virtual Machine in VirtualBox
         Open VirtualBox and click "New".
         Give your VM a name like Kali-Linux.
         Select:
              Type: Linux
                    Version: Debian (64-bit)
              Click Continue.
*Step 4: Assign RAM (Memory)
         Set the memory size to at least 2048 MB (2 GB).
         Click Continue.
*Step 5: Create a Virtual Hard Disk
         Select Create a virtual hard disk now.
         Pick VDI (VirtualBox Disk Image).
         Choose Dynamically allocated (this saves space).
         Set disk size to 20 GB or more.
         Click Create.
*Step 6: Load Kali ISO into the VM
         Click on your Kali VM → Go to Settings.
         Select Storage → Click on Empty under "Controller: IDE".
         On the right side, click the CD icon → Choose a disk file.
         Pick the Kali ISO you downloaded earlier.
         Click OK.
*Step 7: Start the Virtual Machine
         Back in VirtualBox, select your Kali VM and click Start.
           The Kali Linux installer should now launch.
