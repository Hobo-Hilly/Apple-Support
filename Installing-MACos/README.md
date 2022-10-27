# Summary 
In this episode we're gonna use it. So we'll see how to perform an install, how to boot from removable media, how to perform the clean install some of the configuration options and troubleshooting steps we can perform along the way. And hopefully by the end of the episode we've installed Mac OS.

This is out of itpro.tv's library in the series Apple certified support Professional

==============================================================================================================

NOTE: Quick little trick here when you format the drive, if you're running a newer version of Mac OS, you're not actually seeing the hard drive here, you're seeing virtual volumes or logical volumes. So I need to go up top here to the view menu and under view. If I can get it here under view I'm gonna choose show all devices and under show all devices you'll see that my drives change and now I can see my SSD drive right there.

Installation considerations

WARNING: So here's the way this process is going to work. We are going to assume that you've got a Mac and that it doesn't have any data on it that is important to you. So you need to be okay with just ERASING the Mac and starting clean.

- The macOS installation process is fairly straightforward
Boot from the installation media and click next a series of times
Installing through the app store is practically automatic
There are some customizations available

Especially true with a clean install
- Performing a Clean Install of macOS
1. Boot from installation media
2. Hold the 'Option' key during boot if necessary ( Like f12 on a windows machine to get to system boot menu)
3. Select your preferred language               * (it's a little bit tricky is sometimes if you're holding option, when you press power, it doesn't quite register it. So what's ideally perfect is that you'll hit power and then hold the option key on your keyboard.)
4. Choose Install macOS
5. Install macOS - Perform an installation.
6. Select Continue
    * Review and accept the EULA by clicking Agree
7. Select a hard drive to install to
Note that the installation media may show up also
Select Install to complete the installation

# What happens to the hard drive during an installation?

- All right so if it is a completely blank hard drive, then it's going to format it and put the Apple file system on there, the A P F S. So it's gonna format that drive, put the final system in place and then start copying files so it'll set up as one big partition and put the data on there.

- If it is already running macOS it doesn't format the drive, it leaves your data there and it just overwrites the operating system. So it replaces the version of macOS that you have with the new version.

- Your applications and your documents, they all stay in place. And so it's more of an upgrade than a clean install

If you want to do a clean install... From the boot menu
1. select disk utility and continue
2. select drive/disk you want to work with in the left menu
3. ERASE



macOS Disk Layout
- A file system "container" is created
- Virtual volumes are created to store the OS and user data on one drive
- Finding information is easier as there is one place to look
- Upgrades are more simple as files are in their default location
- Most common type of installation

Multiple partitions can facilitate several scenarios
- Running multiple OSes side-by-side (dual-boot)
- Separating user and system data
- Restricting file growth
- Isolating data for easy backup selection
- Providing for alternate file systems

# What do I need to do to be able to boot to more than one OS on a MAC?
''
When you boot up your computer you pick; do I want to boot up into macOS or do I want to boot into Windows? But you need to have two partitions for that. You have one partition for macOS and another partition for Windows or maybe just want to keep your data and your operating system separate. i.e. I wanna have all of my data on one hard drive and my operating system on another. Well if you have two hard drives you can do that in a Mac book, you can't have two hard drives so you do two partitions.

If you need a refresher... Here is a pretty small but potent explanation. https://en.wikipedia.org/wiki/Disk_partitioning#Partitioning_schemes

''
Bootcamp
- Multiple partitions allow for multiple operating systems
- Bootcamp leverages this to enable macOS and Windows to coexist
- Separate partitions ensure one OS does not damage the other's files
- Separate partitions allow for each OS to use their native file system

Considerations
- Separating user and system data can make it more simple to locate information
- Backups are smaller and faster because you only backup the user data disk
- Can create problems with some software as well as future upgrades

Installer Log
- Available in the macOS Installer menu bar
- go to Window
- Select Installer Log

This will show you what the installer is doing. You can see errors and failures right from the terminal! 
Top right hand corner of pop-up terminal will have a drop down tab to show other settings


NOTE: 

- We had partitions and partitions were pretty limited. You can only have four and there were these logical partitions that has all sorts of formating rules. They weren't all that flexible. That's the old way of doing things. 

- The new way is to use a volume. Volumes are logical, you can have as many of them as you want and they can be laid out however you want. So that's kind of the new way to do it 