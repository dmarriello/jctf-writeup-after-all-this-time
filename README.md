# after-all-this-time writeup

### Setup/tools used
FTK Imager - This tool was used to open the original .ad1 file given. It is Windows exclusive as far as I know. There are alternatives but this one makes your job easiest (though it was a nightmare to find/download a legitimate version that didn't look like malware).

Kali Linux - I mainly used Kali for John the Ripper, but being able to 

KeePass 1.41 - This will be needed to view a database file. Annoyingly, this is a different version of KeePass than the one used for the crack-keepass challenge so you will need to download it again.

Audacity - This will be needed to view an audio file's spectrogram.

dcode.fr - This website, especially the "Cipher Identifier" page, helped a lot with getting this challenge done.



## Step 1

First off, opening the .ad1 file as evidence in FTK Imager gives you a bunch of files to comb through. It is an image file, so make sure to select that option when opening the file. 

Our main point of interest is at [root]/Users/User/Desktop currently. There are two files that read "nothingimportant.txt", one of which was deleted. These files give various hints about storing passwords and them being given a key to layer the security. 

There's also a PDF file of a book called "The Time Machine", which is where the next major puzzle lies. 

Just before we tackle that puzzle, it's worth noting that in [root]/Users/User/Documents, there is a folder called "security_keepout" which has a file called "beausFortressOfPwnitude.txt" which seems to have encrypted passwords. The name of the file references the Beaufort Cipher, but without a key, we cannot decode it currently.



## Step 2

Upon looking at the PDF, two major things of note jump out. The second page has a note on it and some numbers, which I will attach an image of, and the final page has some highlighting via an comment shown by Adobe.
