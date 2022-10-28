# Summary
- This is a little bit about how MacOS handles printers. We're going to see how we can get one attached to our system, install drivers if need be. And we'll learn a little bit about ways that we can share a printer across the network. So we don't have to go in and install multiple printers on multiple machines.

================================================================================================================
# How do we add printers to our mac?
''
Apple has tried to make it as easy as possible and so we certainly see that with printers. In fact many times your Mac will just automatically find printers on the network. We have 'air print' where it could just find those systems and add them in. 

So you might not even have to do anything like your printer might automatically set itself up and you're done. But we do need to know how to go in and check to confirm that it actually happend.

# Options
Now you can do it manually also if you need to, you might need to go in and manually tell your Mac, here's this printer that exists

NOTE: macOS Big Sur is the seventeenth major release of macOS, Apple Inc.'s operating system for Macintosh computers. It was announced at Apple's Worldwide Developers Conference on June 22, 2020, and was released to the public on November 12, 2020.

* From the desktop of mac running 'Big Sur'
1. got to the apple icon/ apple menu
2. select system preferences  
3. Find printers and scanners (its a printer icon); select it
STATUS: you can now see all active printers && scanners connected to your mac.
    Unless you have connected printers before || the printer automatically set up via 'air print' this will show an empty list. 'No printers are available. Click Add (+) to set up a printer

# How do I add a printer?
1. Select the '+' sign on the bottom left hand side of the menu

STATUS: The machine is now activly trying to find printers on the network it is connected to.

2. From the pop-up window showing all the printers connected to the network. Select the one you are trying to setup. * Make sure that 'Use:' box at the bottom is a supported format. i.e. 'Secure AirPrint'    
3. Select Add at the bottom of the window
STATUS: So from this point I can just pick the printer and hit add it's gonna reach out, make sure it identifies the printer and then add it in.
4. DONE! It should show the printer as added and idle 


# Do we need to download drivers/ install drivers on our printers?

Short answer: No not usually

NOTE: As the little status bar appears on the screen right after we click add to add a new printer. There are two things happening. 

- One, it's figuring out the model of the printer to make sure that we have the appropriate driver for it. If it does not find the appropriate driver it will try and reach out to an apple server and retrieve it. Apple actually maintains a database drivers.
- And then the second thing is once it looks at the printer it's got to figure out what features the printer has.
- A lot of business printers have optional features like an extra paper tray or a stapler hole puncher duplex, these are special components printers have to allow things that we don't normally need a home.
- A home printer is likely not going to have that, but it could be something more advanced. Like you have a multi function printer that has a scanner and fax functionality. So it's got to figure all that out. 

Considerations

But if it's a multi function printer that has scanner and all that other stuff, that's extra software. And so in that case we may need to install drivers. 
==============================================================================================================
Printers can be added by two methods
1. Manually connecting the printer and installing drivers (if required) 

2. Automatically discovering the printer

Common Unix Printing System (CUPS)*
# What the F is CUPS ?

And CUPS is the common UNIX printing system and it was designed to give a common set of printer driver like functionality that would work in MacOS and Linux and anything that was UNIX based. 

Well, Apple loved the idea. And so they hired the guy and they acquired the project and since, I don't know, I think like 2007 they've had this open source printing project that they have financially supported and it manages all the printing. 

And the cool part here is if you are HP or somebody like that and you're making a printer, you can make one driver a CUPS driver. And that will now work in MacOS and Linux and all these other OS's and they still make a Windows driver, but the drivers are available

NOTE: Now, we don't need to know much about CUPS because Apple is already installed it, it's already doing its thing. But if you want to learn more, you can check that out at cups.org

HP Support Website

https://support.hp.com/us-en

You can look up your printer here via model number

- The foundation of printing in most Unix-based OSes
- Owned by Apple, but an open-source project
- Uses PPD files for printer drivers

# What is a PPD Postscript Printer Definition file?
    - A PPD file describes all the functionality of that printer and how you can talk to it.
    - And that PPD file is all you need is the same across all these different OS's   :) FINALLY 

# What happens if the OS detected by the (ANY BRAND PRINTER WEBSITE HERE) is incorrect?
EX:
    In this case it's saying detected operating system MacOS 10.15. Well, as Catalina, I'm not running Catalina, but that's what it detected. But you know what, it's okay. Even if it came up and said, hey, you're running MacOS Mavericks or something really old. That's okay because the CUPS driver is actually the same across all the different versions. So as long as it picks MacOS, I'm going to be in good shape.
# What if MacOS isn't there?
EX:    
    If MacOS isn't there a lot of times you can pick Linux and you'll be okay because ultimately with CUPS, what you need is what's called a PPD file and a PPD file is a postscript printer definition file. 
    And what it does is it describes all the functionality of that printer and how you can talk to it. And that PPD file is all you need is the same across all these different OS's. 
    So I don't need a perfect match it just needs to be close. Now, where that's different is if there's a scanner, if there's a duplex or if there's all that other stuff, then I am gonna need to make sure I get the right operating system. 

''
    PostScript Printer Description (PPD)*
    Apple provides native drivers for many printers
        - /System/Library/Printers
    Most vendors provide PPD files for their printers as it enables both MacOS as well as Linux - /Library/Printers




- When printing, your document is pre-processed and stored in /var/spool/cups
- The spool folder is protected to ensure users cannot access each other's print jobs

A printer on your machine can be shared to other systems on the network
1. System Preferences -> Printers & Scanners
2. Select the printer
3. Select Share this printer on the network

Printer Preferences
1. System Preferences -> Sharing
2. Select Printer Sharing
3. Select the printer
4. Assign desired permissions

