#What a command line is, and what it does:#

A command line is a tool that looks like a little black window that you can type specific commands into, one line at a time. It's not like Siri or google, so you can't type anything you like, only the specific commands it understands. Further down the page, I have provided a list of 10 of these commands and what they do.

 Programmers use command lines to talk to computers faster than using pictures, the mouse, and lists of menus. With a command line, you are essentially cutting out one of the translators between you and the computer. Computers process their knowledge in binary, that gets translated for us into text, and into the menus, icons, and all the things on your screen you can see and click.

 Putting commands into a command line saves both you and the computer the time and effort of having to navigate the things displayed on the screen, and make for faster and more effective control of what you are trying to do on the computer, whether that be making directories (folders) repositories (files that keep a history of what changes you have made, and allow you to upload, collaborate on and change them as many times as you like) or simply finding out what is in the folders(listing the files)

 *To summarise*: The command line is a text interface for the computer's operating system. To access the command line, we use the terminal.

 ##10 Terminal Commands and What They Do:##

  ###pwd###

 This shows you the Working Directory (current folder) that you are in, and if you type it into your terminal, it will respond by telling you the folder that you are currently situated in - this is useful if you want to make a new folder or file, and you want to know where you are making it to make sure you're not putting it in the wrong place

 ###ls###

 This command, when typed into the terminal, will make the command line look at the folder you are currently in, and list all the files and folders inside of it

###cd###

 This command stands for Change Directory. Say you are in a main folder that has other folders inside of it, to do that, you would type cd followed by the name of the folder inside of it that you want to go to.
 This is the equivalent of looking at a list of folders and clicking on the one you want to go to. 
 
 It can get just as complex as the visual version, you can have a folder inside a folder inside a folder .

 Say your first folder is animals, inside that there's a folder called cats, and inside that there is a folder called tabby. 

 If your pwd was displayed as animals, to navigate to the tabby folder you could type : **cd cats/tabby/**

If you then wanted to go back to cats, you could type:
**cd ..**

where the ".." means go back to the parent folder, (the one that the folder you are in now, is inside of)

You could also combine the two. if you are in the folder called tabby, but you want to be in a folder called ginger which is also in the folder called cats, then you would type:

cd../ginger
(".." to go back to cats, "/ginger" to get into ginger)

###mk dir###

This command stands for **make directory** and it allows you to make a new folder inside the folder you are currently in. If you were in the folder "cats" and wanted to make a folder called "persian" then you would type:

mk dir persian 

###touch###

This command is similar to mk dir, but instead of making a folder, it will make a file. The same logic is used, if you are in the folder "persian" and you wanted to create a text document called "persian.txt" then you would type

touch persian.txt

#####All of the 5 commands above are used for navigating the file system, *pwd* to show the folder you're in, *ls* to list what that folder contains, *cd* to change the folder you are in, *mk dir* to make a new folder inside the one you are in, and *touch* to make a new file inside your current folder.######

Below are some commands for *manipulating* these folders and/or files.

###cp###

This command copies files or folders. It does this by copying them from one place to another.

if you had two text files called "gingercat1.txt" and "gingercat2.txt" and you wanted to copy the contents of gingercat1.txt into "gingercat2.txt" then you could type:

**cp gingercat1.txt gingercat2.txt**

notice the first file listed is what gets copied, and the second file listed is where it gets copied to.

you could also copy a file and place the copy into a different folder using this command. If for example, you had a file called "persian.txt" but it was currently in your folder "cats1" and you wanted another copy of it in your folder "favecats" while both cats1 and favecats are in the same folder called "allcats", you would:

first navigate to the allcats folder. you will know when you get there because by typing pwd, you should get the response allcats/

then type **cp cats1/persian.txt favecats**
to make a copy of persian.txt appear in the favecats folder.

The cp command can be even more useful when you use wildcards, but I won't delve into that right now.

###mv###

The mv command stands for move, and you use it to move files and folders from one location to another. It is very similar to the cp command with the way it works. You type mv followed by the name of the file you want to move, followed by the location you want to move it to, which is usually a folder. if the folder is in a different folder than the file you want to move, you'll have to remember to use the correct combination of ".." to go back a folder and /subfoldername/ for subfolders

it can also be used to rename a file just like you would with your mouse and the menus that you can see on your screen when you use your computer every day. to use the mv tag to rename a file, simply type: mv followed by the name of the file you want to rename, followed by the new name you want it to have (remember to use the same file extension eg. .txt unless you want it to be a different kind of file)

###rm###

The rm command is used to remove (delete) files and folders. This can be done by typing rm followed by the name of the folder or file that you wish to delete. it makes it easier if you are in the same folder that the file or folder you are trying to delete is in, because then you don't have to use ".." and "/" to tell the computer which  file or folder you are looking for.

you could also type rm -r followed by the name of a folder you would like to delete. This will delete that folder, and all of the folders inside of it. 

**Remember: there is no command to undo the deletion of files and folders, deletion is permanent, so don't delete anything that you will want back in the future.** 


###git init###

The git init command is used to initiate a .git repository. That does sound like a bunch of jargon, so to simplify it, this command will create a special folder which will act as a library of sorts. Inside this folder will be another folder called .git and in there is where the main copy of anything you put in there will actually stay, but only once changes to the other copy of it that you have outside of the .git folder, and inside the folder you just created,  have been saved, and then committed, will they be allowed to affect the copy in there.

 I'm not sure if that made it any simpler, so perhaps to provide context: Don't you hate it when you're working as a group in Google Docs, and one person types on the same line that you're typing on, and it all becomes a big mess? Isn't it super inconvenient when you're working in Microsoft Word and something goes horribly wrong and it all freezes up and you perhaps lose hours of work because nobody told you about regular saving?

 Well, Git is a Version Control System, aka. your knight in shining armour when it comes to issues like how to merge changes made to files and folders by different collaborators in a way that makes sense, and how to have access to all possible versions of a file or folder since it's creation, and how to protect all of those.

 This means that if you are working on a piece of html code, and everything is working well, until you make one change and then suddenly nothing will work, you can refer back to a previous version that did infact work, and try to solve your problem from there.

 *inhales* Ok so that was about what Git is, so what git init does is it allows you to create a special folder, a repository, which implements the benifits of git to your folders and files within that repository. other functions include being able to pull from a central repository, and push to the central repository. 

 In this way everyone can have their own personal repository, but also collaborate on a global repository, like GitHub.

 But I digress.

###exit###

You can use the exit command to close the black box (the command line) and leave the terminal, which will enable you to get on with whatever else you are doing on your computer.

simply type: exit 
then hit enter, 
and you will have vanquished your terminal, which will log you out, and fade away into the ether. For now.

Thank you for your time!

by Tat
 

















