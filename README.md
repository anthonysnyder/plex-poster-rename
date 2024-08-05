# plex-poster-rename
A simple script to enable renaming of files for better integration with Plex

**Requirements**: 
- Synology
- Plex
  - _Use local Assets_ enabled for your movie folder. 
- ThePosterDB membership
- Plex Folder Structure in _/Movies/MovieName (release year)/MovieName (release year).ext_ format   
  **- This is CRITICALLY important because the script is comparing the name of the poster you download to the name of the parent folder and will ONLY rename the file if they are an exact match**  
- Synology Task Scheduled that is set to run once every minute

**Optional**:
- Private Slack Instance for Notifications
- Newly created Slack Webhook URL for insertion into script
- Newly created Slack Channel for notifications (mine is #poster-rename)

1) Copy the code in this repository and create a new Synology Task Scheduler item that will repeat daily every minute (I do this because I tend to update large swaths of media at once and want this to run as frequently as possible)
   ![Image of Task Scheduler schedule (lol)](https://github.com/user-attachments/assets/a78c69eb-a26f-4d83-b485-b976619801b3) ![Image of where to place the Script in Synology Task Scheduler](https://github.com/user-attachments/assets/ac5cbc0b-d1ac-4c2c-a0f9-4b4aaf8129f2)

_Note: Make sure to replace the Placeholders under Directories with the directory that your movie folders live in._

2) Download any movie poster that you need from ThePosterDB.com
   
![Image of Blue Crush Poster that I want to download](https://github.com/user-attachments/assets/cb839279-f9c0-4449-99ab-cc72c8bc96aa)

5) Move the  newly downloaded file from Finder to the Synology directory for the movie itself.
![Image of Finder indicating where to move the file to](https://github.com/user-attachments/assets/7d4d9f80-1368-455f-9c19-17a40bb75365)

![Image of the new file after being moved to Synology](https://github.com/user-attachments/assets/efb6e464-01a8-4c71-bcf1-87ce5835137f)
- Note how the file is still in _MovieName (release year).ext_

7)  Wait 1 minute and the Script will run automatically in the background and automatically rename the file to _poster.jpg_ which is what Plex requires in order to consider it a Local Media Asset.
    ![Newly automatically renamed file is now present on the Synology](https://github.com/user-attachments/assets/3dbbaade-0edf-467c-9442-6c2344b7a661)

Optional Info: 
If you opted to use Slack for notifications when the script runs successfully, you should get a notification that looks like this: 
![Screenshot from Slack showing file rename](https://github.com/user-attachments/assets/d6c75ec8-6c83-4dfc-884d-c33b8e7a3056)

