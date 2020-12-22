# [The Freedom Wrapper Project](https://github.com/mdbench/The-Freedom-Wrapper-Project/blob/master/README.md)
[![GitHub license](https://img.shields.io/github/license/mdbench/The-Freedom-Wrapper-Project?style=for-the-badge)](https://github.com/mdbench/The-Freedom-Wrapper-Project/blob/master/LICENSE) [![GitHub forks](https://img.shields.io/github/forks/mdbench/The-Freedom-Wrapper-Project?style=for-the-badge)](https://github.com/mdbench/The-Freedom-Wrapper-Project/network) [![GitHub stars](https://img.shields.io/github/stars/mdbench/The-Freedom-Wrapper-Project?style=for-the-badge)](https://github.com/mdbench/The-Freedom-Wrapper-Project/stargazers)

![TFWPBanner](https://raw.githubusercontent.com/mdbench/The-Freedom-Wrapper-Project/master/TFWPLogo.png)

## The Freedom Wrapper Guide

### For Newbloods:

**The following is a guide on how to get set up with The Freedom Wrapper Project so you can officially make your own application!**

1. First things first. You’ll need to install Android Studio on your computer. Head over to this website to download and install it: [Android Studio Download](https://developer.android.com/studio). 

2. Now, you’ll need to download The Freedom Wrapper Project Repository to your computer. The easiest method will be to download the master archive located here: [The Freedom Wrapper Project Download](https://github.com/mdbench/The-Freedom-Wrapper-Project/archive/master.zip). Once downloaded, head to the folder where you downloaded it and unzip or extract the file. This is usually as easy as right clicking the file and going to the button that says: **“Extract here”** or **“Unzip.”** It will take a couple of seconds for it to extract. In the file that is extracted, you should see all of the available applications The Freedom Wrapper Project has pre-made, along with the original source code dubbed **”The Freedom Wrapper Project”**. 

3. Next, open up Android Studio (if you already haven’t). It will show you a prompt that says open or make a new project. Click the **“Open”** button. Use the file browser to navigate to the folder where you downloaded The Freedom Wrapper Project master archive and click on the folder with the green android/alien where it says **“The Freedom Wrapper Project.”** It’ll take a few seconds to a minute to load depending on your computer. 

4. On the left-hand side there is a button that says **“Project.”** It is right next to the **“ResourceManager” button.** I promise it is there. There are a lot of buttons on Android Studio so give yourself some time to adjust and don’t feel overwhelmed. Once opened, you should see some folders with folder trees. Click on the sideways triangle (it honestly looks like a video play button) to open up a folder’s tree. It will expand or close each time you click it. The first file you will need to modify is in the folder labeled **“java.”** Go to **com.matthewbenchimol.thefreedomwrapperproject** and click the sideways triangle (play button) again. Now, double click on the file that says: **“MainActivity.”** Go down to the *48th* line of code where it says `webView.loadUrl(“https://wikipedia.org”)` and replace the *https://wikipedia.org* with the website you are trying to “wrap”. Make sure you keep the `“ ”` surrounding the website or the build will not compile! For example, let’s say you want to create a wrapper for Facebook. You would place *https://facebook.com* where the Wikipedia link is and the product would look like this: `webView.loadUrl(“https://facebook.com”)`. I have provided comments on the various lines of code should you be interested in turning on or off certain aspects of the application that are preset. I highly suggest you leave them as is unless you know what you are doing. For future reference, all java code comments start with // and are grayed out. They are a method to explain what a line of code does without affecting the compiling of that code for use in your application when you build it. 

**That’s it! That is technically all you have to do to create your first application. There are additional network security settings I highly suggest. These are not specifically necessary. If you want the extra security (you do), continue below. Otherwise, skip the fifth and sixth steps.**

5. Open the **“Project”** button again if for some reason you or Android Studio toggled it close. This time go to the folder that says **“res.”** Click the sideways triangle to open up the folder tree. Then, click on the sideways triangle for two folders to expand the folder tree. One is called **“xml”** and one is called **“raw.”** Open the browser of your choice. For example, **Chrome or Firefox.** Go to the website you are trying to “wrap.” Sticking with the Facebook example above, go to *https://facebook.com.*

- For *Firefox*: Once the page is loaded, click on the padlock next to the website in the navigation bar. Click on the arrow that says **“Connection secure”** and click **“More Information.”** This will open up a page security tab. Once that is opened, click on the button that says **“View Certificate.”** It will open a page where you can export certificates. Click on the certificate tab to the farthest right and scroll down to where it says download. Click the **“PEM (cert)”** option. Save the certificate to the folder we opened earlier in **“res”** labeled **“raw.”**

- For *Chrome*: Once the page is loaded, click on the padlock next to the website in the navigation bar. Click on the tab that says **“Certificate (Valid).”** Click on the tab that says **“Details.”** Go to the certificate hierarchy and click on the certificate that has **“Builtin Object Token:”** next to it. Go to the button on the bottom right that says **“Export.”** Save the certificate to the folder we opened earlier in **“res”** labeled **“raw.”**

6. Now, go back to Android Studio and open the **“xml”** folder tree we discussed in *Step 5* and double click on the file that says **“network_security_config.”** Follow the directions that are listed as code comments. They should start like this: `// this is a network security configuration`.

7. Lastly, go to the top of Android Studio where the drop-downs are and click on the **“Build”** drop-down next to **“Refactor”** and **“Run.”** Then, click **“Generate Signed Bundle / APK…”** and follow the prompts. Make sure you click on the .apk button when creating your application. The app bundle (.aab) is strictly for the Google Play Store and will not be install-able on your Android phone. It is meant for Google Play Store Submissions. You will also be prompted to create a signing key. Please make sure you make one. This is important: a signing key let’s everyone know the application is legitimate and gives users the ability to verify it accordingly. You can fill anything you want for the signing key. I suggest you add the minimum: First and Last Name (Your Name – as this is *your* application), Organization (The Freedom Wrapper Project), and add a password that is yours and yours alone. After that, you can just press the **“Next”** button. Then, click the **“V1”** and **“V2”** check boxes and highlight the **“Build Variant”** that says **“Release.”** It will start the build process. 

8. There should be a notification that pops up after you have successfully built the application. It will say **“locate”** on it. Click it and Android Studio will automatically open the folder containing your recently developed application. Copy the .apk file it created to a folder that will let you find it easily now and in the future, change the name of the file (while preserving the .apk file tag at the end of it), download it to your phone through a USB (preference) or by uploading it to the cloud. Install it and ignore the warning about **“installing from unknown sources.”** You made this app so you can guarantee it is not malicious. Open it when it is finished installing on your Android Device. **Congratulations! You are now using The Freedom Wrapper Project.**

### Further Customization:

**The following guide will be updated occassionally, as customization is an evolving process and not an endstate. Keep that in mind and feel free to check back in occasionally for new methods and techniques.**

1. Let's say you really want to make The Freedom Wrapper Project application your own. This is the section for you! First things first, go to your preferred search engine. Type in the name of the website you are "wrapping" and click search. Go to images and grab an icon of the website you chose for your recently created application. Save it anywhere you will remember it for use in the near future. 

2. Open up Android Studio again. You will likely be doing this a lot, as I am hoping I have made this your new hobby or, at the very least, your new curiosity. Once you have the project opened in Android Studio, open up the **"Project"** tab on the left side and navigate to the file tree (you have been there before) labelled **"res"**. Right click the **"res"** folder, go to **"New"**, and then go to **"Image Asset."** Click on it. It will open up a new window with a bunch of awkwardly green icon templates. On the left-hand side, there is a section about 4 lines down that says **"path."** Click the greyed out folder on the end of it. Nagivate to the picture you just downloaded. There is an option to resize the image at the bottom of the window. Just move it left or right to resize your imported image. Click **"next"** and click **"next/finish"** after that to set your new image as the icon for your app.

3. There you go! You have just added a custom icon to your application. There is a lot more customization you can do and I highly suggest you examine all the files in The Freedom Wrapper Project Source code, checking the code comments at your leisure. There are a decent amount of comments that will give you a necessary walk-through. **Enjoy and have some fun!**

### Need help?

- [Join us on Keybase!](https://keybase.io/team/tfwp) 
