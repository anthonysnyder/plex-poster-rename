# plex-poster-rename
A simple script to enable renaming of files for better integration with Plex

**Requirements**: 
- Synology
- Plex
  - _Use local Assets_ enabled for your movie folder. 
- ThePosterDB membership
- Plex Folder Structure in _/Movies/MovieName (release year)/MovieName (release year).ext_ format
- Synology Task Runner that is set to run once every minute

**Optional**:
- Private Slack Instance for Notifications

1) Copy the code in this repository and create a new Synology Task Scheduler item that will repeat daily every minute ( I do this because I tend to update large swaths of media at once and want this to run as frequently as possible)
   ![Image of Task Scheduler schedule (lol)](https://github.com/user-attachments/assets/a78c69eb-a26f-4d83-b485-b976619801b3) ![Image of where to place the Script in Synology Task Scheduler](https://github.com/user-attachments/assets/ac5cbc0b-d1ac-4c2c-a0f9-4b4aaf8129f2)

_Note: Make sure to replace the Placeholders under Directories with the directory that your movie folders live in._

2) Download any movie poster that you need from ThePosterDB.com
   
![Image of Blue Crush Poster that I want to download](https://github.com/user-attachments/assets/cb839279-f9c0-4449-99ab-cc72c8bc96aa)

5) Move the  newly downloaded file from Finder to the Synology directory for the movie itself.
![Image of Finder indicating where to move the file to](https://github.com/user-attachments/assets/71ed93b0-ae38-4dd4-8912-7b72e7673634)

 Note how the file is sti![Uploading wdefr.jpg…]()
ll in _MovieName (release year).ext_

![Image of the new file after being moved to Synology](https://github.com/user-attachments/assets/512c473c-3f45-4a90-b7be-5c1b6ed6febd)

7) 
8) Wait 1 minute a
