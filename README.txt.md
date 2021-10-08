# AI_for_development_aid

Connecting to the Azure Server with VSCode

1. Download Remote SSH extension for VSCode
(https://code.visualstudio.com/docs/remote/ssh-tutorial)
2. Use the Blue button on the bottom left to promt the extension to open, and then it will open a dropdown menu at the top of the editor.
3. Select connect to host, then select add new ssh host
4. Type "ssh username@congoubuntu.eastus.cloudapp.azure.com" and then select where you want to save the config file.
5. After saving the file hit the blue button again and select the connect to host option which will then show the congo ubuntu connection.
6. A new window will open and prompt a question for which operating system the VM is using, select linux, then it will ask for your password.
7. After entering your password you are connected to the VM .

Creating a a python file in your folder & selecting interpreter 
1. Select explorer and go to the folder with your username as the title, in my case "jmv192"
2. Enter azure password again
3. create new folder whereever you want (can just be a child of the "username" foldeR) and name it whatever you want but have the
.py after or .ipynb
5. at the bottom, select the tab to the right of the blue tab, and at the top of VSCode it will prompt you to chose an interpreter path.
6. choose the python 3.6.9, we can use different ones depending on the interpreter we want but this is the base one
7. you can write whatever code in the file created previously and it will work now.

Creating and Activating a Virtual Environment
1.Once you are in the "username" folder on Azure you can create a folder to contain your python projects and virtual environment
2. Open the terminal at the bottom of VSCode and navigate to that folder. (cd "path")
3. After the terminal is in this folder you want type python
4. check if you have pip 3 installed (which pip) if not install pip3 (sudo apt install python3-pip
5. Install venv package ( sudo apt-get install python3-venv)
6. create venv  (python3 -m venv ./venv)
7. cd into the venv folder 
8. activate the venv (source bin/activate)

Working with Venv on DataDrive
1. To work on datadrive and open venv you need to start VSCode in a broader part of the Server so we need to reconnect to the server and when it asks to open folder normally it is pre filled with "home/username/" delete everything but / so that it is just "/" and open that
2. Now with the VSCode Folder explorer go to home/username/folder with venv
3. either cd into this or right click on the folder and open hit the open in integrated terminal 
4. run source bin/activate
5. cd out to / (cd ../)
6. cd into DataDrive
7. cd into folder with code
8. python3 "scriptname.py)
