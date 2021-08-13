Skill Builder 6.0 Release Notes
===============================
version - 2/10/98


Installation Directions
=======================
To update your version of SkillBuilder from 5 to 6 please follows these steps:
1. Exit any Skill Builder course you might have opened.
2. Make a backup copy of your existing Skill Builder player by copying all files in the skillb directory (not subdirectories) to a backup location. The player filenames have extensions .DLL, .DAT, .EXE and .HLP.
3. Leave the existing course subdirectories within the \Skillb directory, such as \skillb\a70011.
4. Copy the 6.0 player files from the Skill Builder 6.0 CD to your skillb directory. Make sure to include the new Skill Builder tutorial (atutor directory) from the CD as well.
5. Start any existing course by the usual method to confirm that the engine upgrade was successful.


Please note, that once you install the Skill Builder 6.0 player, you can NOT go to one of your old Skill Builder 5.x Roms and expect to install the 5.0 player back on top of the Skill Builder 6.0 player. The Skill Builder installation program does not allow you to install older players over newer ones.




Changing the Interface
======================
After you install Skill Builder 6.0 you will notice that you are automatically presented with the new "Contemporary" Skill Builder interface.  If you wish to revert to the "Classic" Skill Builder interface (used by version 5), you simply need to change a setting in the NETG.INI file.  To do this follow these directions:

1. Exit any Skill Builder course you might have open.

2. Start notepad which can be found in your Accessories group.

3. Open the file c:\windows\netg.ini (please substitute in the correct path for your Windows directory).

4. The contemporary vs. classic interface is determined via a flag, InterfaceMode, which is set in the course section.  A course section is designated by [], for example [A70011]. Under this section heading you will see a variety of settings.  To change the interface for a particular course change the setting of the InterfaceMode flag.  If the InterfaceMode flag is not there you will need to add it.  

For example, below you will notice the course settings for the course 71021:
[A71021]
Feedback=2
StudentMgt=2

To set the user interface back to the Classic interface you would need to add the InterfaceMode flag and set it to a value of 133 (which stands for Classic).  The updated section would look as follows:
[A71021]
Feedback=2
StudentMgt=2
InterfaceMode=133

If at some later point you wanted to change to the Contemporary interface you would need to change the InterfaceMode flag to 134.

5. After making the change to the course sections, save the NETG.INI file.  The next time you start a Skill Builder course, you will see your InterfaceMode setting take effect.




