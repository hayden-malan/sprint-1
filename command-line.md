#What a command line is, and what it does:

A command line is a tool that looks like a little black window that you can type specific commands into, one line at a time. It's not like Siri or google, so you can't type anything you like, only the specific commands it understands. Further down the page, I have provided a list of 10 of these commands and what they do.

 Programmers use command lines to talk to computers faster than using pictures, the mouse, and lists of menus. With a command line, you are essentially cutting out one of the translators between you and the computer. Computers process their knowledge in binary, that gets translated for us into text, and into the menus, icons, and all the things on your screen you can see and click.

 Putting commands into a command line saves both you and the computer the time and effort of having to navigate the things displayed on the screen, and make for faster and more effective control of what you are trying to do on the computer, whether that be making directories (folders) repositories (files that keep a history of what changes you have made, and allow you to upload, collaborate on and change them as many times as you like) or simply finding out what is in the folders(listing the files)

 ##10 Terminal Commands and What They Do:

 * ###pwd

 This shows you the Working Directory (current folder) that you are in, and if you type it into your terminal, it will respond by telling you the folder that you are currently situated in - this is useful if you want to make a new folder or file, and you want to know where you are making it to make sure you're not putting it in the wrong place

 * ###ls

 This command, when typed into the terminal, will make the command line look at the folder you are currently in, and list all the files and folders inside of it

* ###cd

 This command stands for Change Directory. Say you are in a main folder that has other folders inside of it, to do that, you would type cd followed by the name of the folder inside of it that you want to go to.
 This is the equivalent of looking at a list of folders and clicking on the one you want to go to. 
 
 It can get just as complex as the visual version, you can have a folder inside a folder inside a folder .

 Say your first folder is animals, inside that there's a folder called cats, and inside that there is a folder called tabby. 

 If your pwd was displayed as animals, to navigate to the tabby folder you could type : **cd cats/tabby/**

If you then wanted to go back to cats, you could type:
###cd ..

where the ".." means go back to the parent folder, (the one that the folder you are in now, is inside of)

You could also combine the two. if you are in the folder called tabby, but you want to be in a folder called ginger which is also in the folder called cats, then you would type:

cd../ginger
(".." to go back to cats, "/ginger" to get into ginger)











