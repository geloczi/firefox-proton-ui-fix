# Firefox Proton UI fix
Restores the classic tab style (Firefox 89 or newer)

The new **Proton UI** appeared in Firefox 89 and I'm one of those people who want back the **classic tabs**.


## Motivation

Setting the **browser.proton.enabled** option to **false** is not working anymore since Firefox version 91. 
I love Firefox, but I was really upset to see there is no option anymore to turn back on the classic style. 
I decided to do some research in order to find an option to alter the user interface, and 15 minutes later this project was born. It is as it is, just a quick fix :)

## Installation

### 1. Enable legacy CSS

Start Firefox, and navigate to **about:config**  
Set **toolkit.legacyUserProfileCustomizations.stylesheets** to **true**  

### 2. Find out where is your profile data stored on the disk

Still in Firefox, navigate to **about:support**  
Find the row starting with **Profile Folder**, and click the **Open Folder** button.  
After you clicked the button, your **profile folder** is opened in the *Windows File Explorer*.  

The **profile folder** path is something like this:  
C:\Users\YourUsername\AppData\Roaming\Mozilla\Firefox\Profiles\abcd123.default-release

### 3. Create the "chrome" folder

Create a new folder inside your **profile folder** named **chrome**, then open it.  

Your **chrome** folder should be located inside the profile folder like this:  
C:\Users\YourUsername\AppData\Roaming\Mozilla\Firefox\Profiles\abcd123.default-release\chrome  

### 4. Copy the CSS file

Download the **chrome/userChrome.css** file from this repository.  

Copy **userChrome.css** into your **chrome** folder.

C:\Users\YourUsername\AppData\Roaming\Mozilla\Firefox\Profiles\abcd123.default-release\chrome\userChrome.css  

### 5. Restart Firefox

Restart Firefox to apply the CSS fix.  
