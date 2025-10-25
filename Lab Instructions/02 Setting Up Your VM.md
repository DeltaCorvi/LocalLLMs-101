---
author: Bronwen Aker
updated: 2025-10-03
presentation_type: Workshop
venue: WWHF - Deadwood
---

```table-of-contents
title: # Table of Contents
minLevel: 0
maxLevel: 3
```

# Welcome

In order to make it easy for everyone to "hit the ground running," I put together a virtual machine (VM) with software and LLM models pre-loaded. None of the software included in the VM requires a license for personal use. Some applications do have requirements for commercial or enterprise use. You should be able to make use of the VM and the software on it for a long time after WWHF is over. 
## Setting Up VMware 

This lab is set up to use VMware Workstation Pro version 17, or VMware Fusion 13. Installers are included with the course files and are available via Dropbox. Registered students should have received the link via email. 

MAKE SURE YOU DOWNLOAD THESE FILES AS THE FOLDER ON DROPBOX WILL GO AWAY AFTER WWHF IS OVER.

Here is the link: https://www.dropbox.com/scl/fo/1vapefglltatj0o009j6v/ACOqVIC1UtRQDGfpLlPXF-k?rlkey=qwwot6z63dxu5gfrnaysft1t1&st=o7u0vdn7&dl=0


### System Requirements

Before you do anything, make sure you have the system requirements to download and install both the VM software and the VM itself. 

---
#### VMware Workstation (Windows)

| Component    | Minimum                                      | Recommended                                |
| ------------ | -------------------------------------------- | ------------------------------------------ |
| **CPU**      | 1.3 GHz+, 64-bit, 2 cores, LAHF/SAHF support | Quad-core 64-bit (Intel i5/i7 or Ryzen 5+) |
| **RAM**      | 2 GB (4 GB better)                           | 16 GB (8 GB workable)                      |
| **Disk**     | 1.5 GB for install + space per VM            | SSD, 60 GB+ free for VMs                   |
| **Host OS**  | Windows 10/11 64-bit                         | Windows 10/11 64-bit                       |
| **Display**  | 1280×800                                     | 1920×1080 or higher                        |
| **GPU (3D)** | DirectX 11 / OpenGL 4.3 capable              | DirectX 11 capable GPU                     |

---
#### VMware Fusion 13 (macOS):

| Component    | Minimum                            | Recommended                                          |
| ------------ | ---------------------------------- | ---------------------------------------------------- |
| **CPU**      | Intel Core 2 Duo (64-bit) or newer | Quad-core Intel i5/i7/i9 or Apple Silicon (M1/M2/M3) |
| **RAM**      | 4 GB                               | 16 GB (8 GB workable)                                |
| **Disk**     | 750 MB for install + space per VM  | SSD, 60 GB+ free for VMs                             |
| **Host OS**  | macOS 12 (Monterey) or later       | Latest macOS (Ventura / Sonoma)                      |
| **Display**  | 1280×800                           | 1920×1080 or higher                                  |
| **GPU (3D)** | Metal-capable GPU (for Intel Macs) | Metal-capable GPU / Apple Silicon GPU                |

---

> [!warning] If you have Apple Silicon (M1/M2/M3):
>- Only **ARM-based guest OSes** are supported (ARM Linux, Windows 11 ARM).
>- Intel x86 guest OSes (e.g., older Windows/Linux ISOs) will not run under Fusion on Apple Silicon..

> [!info] About RAM... 
> Theoretically, RAM stands for "random access memory", but in reality it stands for "rarely adequate memory"! 😉 In short, if you have the system resources to increase the amount of RAM allocated to your VM, DO IT!

---


### Installing VMware

Included in the file bundle for this workshop, there should be installer files for VMware Workstation Pro and VMware Fusion. Sorry, no support for VirtualBox at this time. 

- Find the installer appropriate to the operating system for the host on which you will be running the virtual machine. 
- Copy the installer file to the host system. 
- Double click on the file and follow the prompts to complete the installation process.

### Installing the VM

Unlike when you install a new VM from scratch, this VM has already been built and customized to have all the software installed that you need to complete the activities in this workshop. 


### Running the Ubuntu Virtual Machine in VMware 

1. **Download the VM archive**    
    - In the files you downloaded, find `filename.zip`
2. **Install or verify extraction software**    
    - **Windows:** Install [7-Zip](https://www.7-zip.org/) if it’s not already on your system.        
    - **Mac:** Install [Keka](https://www.keka.io/) if it’s not already on your system.
        
3. **Extract the archive**    
    - Choose a location where you want the VM to live and run from.        
        - Example: a dedicated folder such as `C:\VMs\Ubuntu`, or your **Desktop** if that’s easiest.            
        - You can move it later, but it’s best to pick the permanent location now.            
    - **Windows:** Right-click the `.zip` file → **7-Zip → Extract Here** (or extract to your chosen folder).        
    - **Mac:** Right-click the `.zip` file → **Open With → Keka** → extract to your chosen folder.        
    - Make sure all extracted files stay together in a single folder.
        
4. **Open VMware Workstation**    
    - Start **VMware Workstation**.
        
5. **Open the VM**    
    - In VMware, go to **File → Open…**        
    - Browse to the folder where you extracted the VM.        
    - Select the file ending in `filname.vmx` 
        
6. **Start the VM**    
    - Click **Power on this virtual machine**.        
    - Ubuntu will boot and be ready to use.

---

### Troubleshooting Tips

- **If you accidentally open the wrong file**:    
    - Always select the `.vmx` file, not `.vmdk` or other files.
        
- **If VMware asks “Did you move or copy this VM?”**:    
    - Choose **“I copied it”**.        
    - This ensures VMware assigns new IDs so the VM won’t conflict with others.
        
- **If you want to move the VM later**:    
    - Shut down the VM first.        
    - Move the entire folder (not just some files) to the new location.        
    - Open VMware → **File → Open…** → select the `.vmx` file in its new location.


## Logging Into the VM

The username for all labs is: `llm-lab`
The password is: `LLMs4evr`


*That's it! We're ready to roll!*



Next, [[03 Working With Ollama]]...