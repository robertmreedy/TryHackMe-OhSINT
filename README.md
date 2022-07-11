# TryHackMe OhSINT Challenge
What information can you possible get with just one photo?

![WindowsXP Image](WindowsXP.jpg)

First, we can observe the metadata in the .jpg image above by using _exiftool_. Run the following command in Kali Linux to install exiftool:

`sudo apt install exiftool`

Once exiftool has been installed, run the following command to retrieve the metadata from the .jpg image:

`exiftool WndowsXP.jpj`

