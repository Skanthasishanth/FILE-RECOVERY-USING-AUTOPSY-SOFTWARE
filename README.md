# FILE-RECOVERY-USING-AUTOPSY-SOFTWARE

## AIM
To use **Autopsy Digital Forensics Tool** to retrieve deleted files from a disk image.

---

## REQUIREMENTS
- **Operating System**: Windows 10/11, macOS, or Linux
- **Tool**: [Autopsy Digital Forensics](https://www.autopsy.com/)  
- **Test Data**: Disk image file (`disk.dd`, `disk.img`, `.E01`)

---

## ARCHITECTURE DIAGRAM

<img width="577" height="785" alt="Screenshot 2025-08-22 151258" src="https://github.com/user-attachments/assets/0e9e4744-5534-4828-8715-d6210ba065c3" />

## DESIGN STEPS:
### Step 1:
Open Autopsy and create a new case with appropriate case details.

### Step 2:
Add a disk image as a data source and let Autopsy analyze the content.

### Step 3:
Navigate to the "Deleted Files" section in Autopsy and examine or recover the deleted files.

## PROGRAM:
### **1. Copy Files to the Virtual Disk**  
- Open **File Explorer** → Go to the new drive (`C: or D:`), where the folder created in the New Virtual Disk
- Create a new folder (`Autospy`) and copy **images or files** into it.  

### **2. Delete the Files**  
- Select any one or two images → Press **Delete**.  
- Empty the **Recycle Bin** to permanently delete them.  

### **3. Recover Deleted Files Using Autopsy**  
### **Open Autopsy & Create a New Case** 

- Launch **Autopsy** and **Run as a administrator**  
- Click **Create New Case**.  

![](./images/a1.png)

- Enter a **Case Name** (e.g., `Autopsy1`).  
- Choose a **Case Folder** location.  
- Click **Next** → Click **Finish**.  

![](./images/a2.png)

### **Add the Virtual Disk as an Evidence Source**  
- Click **Add Data Source**  → **Select Host**

![](./images/a3.png)

- Select **Local Disk** → **next** 

![](./images/a4.png)

- Select Disk → **Choose the VHD drive (`Drive1`)**

![](./images/a5.png)

- Click **Next** → Keep default settings → Click **Finish**.  
- Wait for Autopsy to process the disk.  

### **Recover Deleted Files**  
- Go to **File Views** (left panel).  

![](./images/a6.png)

<img width="1920" height="947" alt="Screenshot 2025-08-22 091716" src="https://github.com/user-attachments/assets/ed4d92b8-eddb-4ab7-8000-43b98ec6e485" />



- Click **Deleted Files** → Find your deleted images.  
- Right-click an image → Click **Extract File**.  

- Select a folder to see the recovered files (e.g., `C:\forensic`).  
- Image is recovered successfully.


## Output :

#### Name - Kantha Sishanth S
#### Reg. No. - 212222100020

### Folder before deleting the files

<img width="970" height="188" alt="Screenshot 2025-08-22 091320" src="https://github.com/user-attachments/assets/d1700d45-07e9-4a7d-a46c-681420461766" />

### Folder after deleting the files

<img width="1157" height="242" alt="Screenshot 2025-08-22 154355" src="https://github.com/user-attachments/assets/052e0aac-c42d-421e-aba1-e8031bdd3ee5" />

### Folder after extracting the deleted images using autopsy

<img width="970" height="188" alt="Screenshot 2025-08-22 091320" src="https://github.com/user-attachments/assets/342802c8-6f29-4147-a847-e6cceeff0ac8" />


## RESULT:

Deleted files were successfully retrieved and analyzed using Autopsy.

