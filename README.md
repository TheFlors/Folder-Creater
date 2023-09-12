# Folder-Creater

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
