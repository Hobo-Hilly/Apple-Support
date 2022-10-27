

# Where do we get a copy of mac OS?
"you can't go out, and buy macOS directly, you do need to get it with a new Mac, or with an existing Mac, and that's where we get macOS from."

NOTE: Your macOS is pre installed, but if you get updates to new versions, well, it's not gonna magically be on your computer, you would get that from the App Store.

* Obtaining macOS
- macOS is pre-installed on all new purchases
- macOS is available through the Mac App Store as a free download
- The installer is only visible to OS X 10.8 and higher
- Download is a little over 5GB

FYI: Apple doesn't charge for macOS, on the App Store it's free. So you can download the new versions, and get it, but you MUST be on a Mac. Period.
Basically, you have to show you've already purchased that hardware


# What if my hard drive is Blank or Brand New?
 You have two options
 - Internet recovery which would take hours because regardless of your connection, apple only allows so much bandwidth for this task at their server farms. SO it takes "hours".
 - If you can 
- if you can go to another Mac somewhere, anywhere on any Mac, you can build a USB installer yourself.

# How does it work?
- with a USB key like this, you can have macOS loaded on it. And then even if your hard drive is completely blank, you can pop the USB key, and boot up off of it, and install macOS. 
- Also, even if your hard drive isn't blank, maybe you wanna do a fresh, and clean install, you wanna blow everything away. || You want to erase your hard drive, where you gonna install macOS from then, again, USB key. So USB installer's super handy.

* macOS Physical media
- Installation media is not provided in a physical form
- You can create your own physical media from any mac

* Once downloaded, you can create physical media
How to create a bootable installer for macOS

NOTE: Sometimes when creating the key without first deleting it manually can cause issues. So instead of letting the computer try to do it on it's own before building the key. We would manually erase the device by following these steps...

1. COMMAND+(Space) || click the magnifying glass in the upper right hand corner to get to SPOTLIGHT search
2. Type Disk Utility
3. Select the usb name in left bar menu
4. Click Erase

# How do find the Operating System you are looking for? Is my account able to find it?
So for example, if I wanted to build a installer for Catalina, I could go into the App Store, and then in the App Store, I would just search for Catalina like that, and right there I find MacOs Catalina. Okay, if you had Mojave previously, or whatever, you can search and find them, **(it does require you to have actually had a machine running that OS in order for it to show up here on your account.)** So if you're brand new to Mac, then you won't be able to search, and find Mojave, for example, it's just too far back, but if you're looking for something current like Catalina or Big Sur, you'll find it.


COMMAND+SHFT+'+' to blow up screen

* To create a physical USB installation media:
1. Download the macOS installer on any machine running OS X 10.8 or higher
2. Get a USB flash drive or HD with at least 8GB of storage
3. Format the removable drive using Disk Utility
    NOTE: All contents will be lost
4. From the terminal execute:
sudo /Applications/Install\ macOS\ Big\ Sur.app/Contents/Resources/createinstallmedia --volume /Volumes/Untitled

** Untitled is the name of YOUR usb key. However if you format it. It will be named Untitled

FYI: These USB keys can, one, can be used to reinstall macOS, that's handy, but they can be used for troubleshooting, and recovery. You can boot the recovery partition off of the USB key, even if you can't access the one on your disk, really handy if you're troubleshooting hard drive issues. 









* Uses for installation media
- Install macOS
- Repair macOS
- macOS Recovery
- Troubleshooting