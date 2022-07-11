# TryHackMe OhSINT Challenge
What information can you possible get with just one photo?

![WindowsXP Image](Images/WindowsXP.jpg)

First, we can observe the metadata in the .jpg image above by using _exiftool_. Run the following command in Kali Linux to install exiftool:

`sudo apt install exiftool`

Once exiftool has been installed, run the following command to retrieve the metadata from the .jpg image:

`exiftool WndowsXP.jpj`

![exiftool_output](Images/exiftool_output.png)

Under the Copyright results, we see the creator of this image is assocaited with OWoodflint. Let's give this a Google search with quotations around the name:

![OWoodflint_google](Images/OWoodflint_google.png)

A few search results show up for OWoodflint, specifically a Twitter account, Github, and WordPress site. Let's start with the Twitter page associated with OWoodflint. This profile was created in February 2019 and only had 2 tweets. The profile picture of this account is of a *cat*.

![OWoodflint_twitter](Images/OWoodflint_twitter.png)

One tweet lists a BSSID for a "free wifi" network _B4:5D:50:AA:86:41_. Let's look up this BSSID WiFi Network using `https://www.wigle.net/`. 

![OWoodflint_bssid](Images/OWoodflint_bssid.png)

By using Wigle, we find that OWoodflint is using a WiFi network that is located in Downtown *London*. If we search for the intersection of Charles II Street and Waterloo Place on Google Maps, we can then locate the WiFi Network location. 

![OWoodflint_gmaps](Images/OWoodflint_gmaps.png)
