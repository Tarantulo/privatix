# Privatix Ubuntu Service App Install Guide

This will be a short tutorial. That is a bit more simple and easy to follow then the original one.

Updated link to tutorial: [link to tutorial](https://privatix.atlassian.net/wiki/spaces/BVP/pages/270794846/1.+Download+and+install+the+application).

0. First of all install and load Ubuntu
1. Download preparation.py:  [preparation.py](https://raw.githubusercontent.com/Privatix/dappctrl/master/tool/initializer/preparation.py). Just click the link and download it.
2. Next Open the: Terminal app. Use the search.
3. **Important!** Set the sudo privileges that the password would not be required. Command:
```
**sudo -s**
```
4. Check if you have a directory for **/home/root** . You can use the terminal or use the file explorer. Info below.
5. Go to downloads directory in terminal. Check below for the commands to navigate in terminal.
6. Run this command in terminal
```
sudo python preparation.py
```
7. Next run this one:
```
sudo /opt/privatix/initializer/initializer.py
```
8. This will take from 5-10 minutes so be patient and let it work. There will be quite a lot of text. 
9. In case you have two or more network interfaces, you should choose the one that has your internet connection. Just type the name of the interface. For example ens3
10. If everything is ok. You will see: **All done.**
11. Last step is to launch. It will show you the command, run it on terminal:
```
/home/root/privatix-dappgui.sh
```
Where root is the name of your local user. Or it is just root.

12. Next follow the guide on [Privatix guide:](https://privatix.atlassian.net/wiki/spaces/BVP/pages/270663818/2.+Create+an+account). 

# Check the **/home/root** directory

You can use terminal. Use these commands:
- ls - shows the dirs and files in current place
- cd .. - goes back one directory
- cd foldername - changes to that specific directory

Or use File:
- Click Other Locations 
- Open Computer
- Open Home

# What to do if you do not have a /home/directory

Follow these steps:
- sudo adduser temp
- sudo cp -r /home/temp /home/root
- sudo chown -R root.root /home/root
- sudo deluser temp

#How to manually remove the Privatix
If you want to fully remove you have to delete the files in two locations if you want to reinstall Privatix.
```
Use: rm -r to delete a directory
```
1. /opt/privatix
2. 
