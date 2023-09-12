# Folder-Creater

  This application allows you to create any number of files in any location you want.

## Using Steps

### Step - 1 : 
  ![image](https://github.com/TheFlors/Folder-Creater/assets/120198325/09cd2ffc-48ed-4f06-a55d-4c39e11ea992)
  * Enter Your File Extension.
    
### Step - 2 : 
   ![image](https://github.com/TheFlors/Folder-Creater/assets/120198325/b18cd1c4-c16a-4a06-9eda-9b1d79c7c48a)
  * Enter Your Folder Name (What You Want to Create)
    

### Step - 3 : 
  ![image](https://github.com/TheFlors/Folder-Creater/assets/120198325/5e0fa828-f364-4a91-8e52-d1afb156af45)
  * Enter Folder Count.(However much you want)

  
### ---Folders Successfully Created.---

## Codes
```
import os
import time 


def createfolder():
    print("\nEnter File Extension.")
    folderpath = input("---->")

    print("\nEnter Folder Name.")
    foldername = input("---->")

    try:
        print("\nEnter Folder Count.")
        foldercount = int(input("---->"))
    except:
        print("\nPlease Enter Folder Count!")
        createfolder()
    
    try:
        i = 1
        while i <= foldercount:
            os.chdir(folderpath)
            os.mkdir(str(i) + " " + foldername)
            i+=1
    except:
        print("\nPlease Enter File Extension!")
        createfolder()

    print("\nFolders Successfully Created.")
    createfolder()

createfolder()
```


## Frequently Asked Questions
### How I can find my file extension?

![image](https://github.com/TheFlors/Folder-Creater/assets/120198325/1b5fefd1-73ae-429f-b1dc-8d71577a8a35)
* Press Here in Folder and copy extension and paste in app.


