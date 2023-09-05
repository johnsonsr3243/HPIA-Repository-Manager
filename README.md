# HPIA-Repository-Manager
Creates and manages driver repositories for use by HPIA

**to install** download the .msi file from packages. The program will install to c:\program files (x86)\hpia driver repository management
A shortcut will be placed on your desktop. this program should be launched by a user with read/write permission to the directory you intend on installing your repository at. on first launch you will see this screen:

![image](https://github.com/johnsonsr3243/HPIA-Repository-Manager/assets/120566210/22a4c9e3-ada8-4f3e-9cad-0a8585c16460)

**to manage or create a repository**, navigate to the path for it, ensuring you are at the parent folder of the .repository folder. otherwise navigate to the target directory and click create. the filters currently in the repository will populate. you can (should) create a folder for each windows version you plan on using a repository for. You can remove models by clicking the "select" checkbox and clicking "remove from repo". filters are removed by PLATFORM not model, and thus any devices sharing the platform id will also be removed. 

![image](https://github.com/johnsonsr3243/HPIA-Repository-Manager/assets/120566210/1b7b9828-2b54-4439-b985-90d3185b9866)

**to add models** click add models. at the add models screen you can search either by platform id or by model name. when you click add the screen will add the filters, close the child form, and repopulate the datagrid on the mainform

![image](https://github.com/johnsonsr3243/HPIA-Repository-Manager/assets/120566210/e3ddb3f4-3ebd-4cc1-80d0-403179505353)

**to add all models from sccm namespace** click "import from sccm", fill in the fields, hit load, and hit add to repo. note the big red text

![image](https://github.com/johnsonsr3243/HPIA-Repository-Manager/assets/120566210/f1be9d37-67d4-4faa-a815-26d7fd2424f5)

**to start downloading or updating repository** once you have added whatever filters you want, click 'sync' to start a repository sync. you will see some console text in the textbox, but during this time the form will mostly be frozen and unable to be interacted with. the console will indicate when the sync has ended. logs are located in the .repository folder under 'activity'.

![image](https://github.com/johnsonsr3243/HPIA-Repository-Manager/assets/120566210/11bbc3cb-e34f-4e11-ba43-765bab0e5926)

