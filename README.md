# Team-Wars-Data-Analysis
Data Analysis Workflow for the Duel Links Team Wars League

Refer to pinned message in # analyst team channel in Discord for access to the Google Sheets

Team Wars Data Session Where I talk about all the sheets again in detail
https://youtu.be/WFRh6PK_QAQ

Quick Notes about the Matchup Table
https://youtu.be/395c_ngE4Ts

Match Report Tutorial Beginner/If you need a refresher
https://youtu.be/Kl3CeUH4GWU

Match Report Sheets Advanced in depth explanation of functionality and processes
https://youtu.be/hssqArMdK10

Player Records Sheets Advanced in depth explanation of functionality and processes
https://youtu.be/W15YCVEc-Jg

Match Up Table Advanced in depth explanation of functionality and processes
https://youtu.be/ZW4DYuNOPKk

You can update formulas directly in Google Sheets or copy and paste it into a text editor to edit then pasting it back into the sheet after you're done. I like to use Notepad++ because you can set the language to Visual Basic and the highlighting makes it easier to read

Match Reports should be named in the format of "Match Report WXGY" where X is the current week and where Y is the corresponding game #
Blank Match Reports have been created up to Week 10, please fill in those Match Reports instead of creating new ones
Unhide them from the bottom left and add edits to those - Jan 27

Reminder to change DC Loss or DQ Loss etc back to W/L on the match report Google Sheets after screenshot of the match report has been taken and posted to the match reports channel in Discord, as the aggregation counts # of capital W or L

If Skill or Deck Types do not show up in the dropdown list:
1. go to the “Dropdown List” sheet
2. Under the Deck or Skill columns see if that Deck or Skill is already listed
  a. If it is a Skill and not listed please add it to the bottom of the list
    i. top 10-15 most common skills are placed towards the top, the skills below are sorted alphabetically
      add the new entry where you think is the best fit
3. If it is a Deck and not listed, please check the top 10-15 most common decks and decide whether or not the deck in question can be classified as one of those decks
  a. If it can be classified as one of the common decks, please use the name of the common deck instead
  b. If you decide that it is different enough from the currently existing decks
    i. add the deck to the list and propose the addition to analyst chat
    ii. top 10-15 most common decks are placed towards the top, the decks below are sorted alphabetically
      add the new entry where you think is the best fit

If players do not show up in the dropdown list:
1. go to the “Dropdown List” sheet
2. ctrl +F to find the team the player belongs to and see if they are in that team’s list
  a. If you type the player name, then it gets highlighted in yellow, that means there is a duplicate player name
  so add that player into the player database as “[team name abbreviation] player name” if they are on a different team
  b. otherwise if they are on the same team please use the name already listed
3. if they are not then you can add that player to the database
  a. locate the sheet that player is on and enter their player name and Discord User ID

Player Records sorted by
Sorts by: Most wins, Least losses, Highest WPM, Highest Played then, A-Z Player name

Division Standings sorted by
Sorts by: Most Points (3x wins), Highest Round Difference, Head to Head

If a sheet becomes unlinked due to someone renaming/replacing a copy of a sheet already created: 
For example Match Report W1G5 becomes unlinked from Match Report Master (we can see this by the sheet name showing up as black/grayed out text and error message appears)
1. We have to rename the current G5 sheet to "G5 old"
2. Create a new sheet from master and paste the data from old to "G5 new"
3. Then link G5 new to the master by replacing "G5" with "G5 new" in the importrange
4. Then we can rename the "G5 new" sheet back to "G5" and delete "G5 old"
5. Check the importrange now correctly displays G5 data

to make the week 8 meta analysis you want to
In: TW S6 Match Reports
1. make sure week 8 master exists
2. change the range of the pivot table on the error checking sheet to week 8 master for week 7 master
3. if you check the filters have no errors, and that the numbers across decks and skills all match
In: TW S6 Player Records (step 4 optional but it has to be done by someone anyway)
4. add the importrange for week 8
In: TWS36CleanData.csv
5. duplicate the TWS36CleanData.csv sheet to make a backup, and name it today's date
6. from week 8 master that has been checked for errors, copy and paste the 1st and 2nd columns as values below the week 7 data (we don't include the discord id column when pasting), 
7. then copy and paste regularly the rest of the columns below the week 7 data (can click a column to select the whole thing and hold shift to select multiple columns, then copy it)
8. delete the header row that you don't need, (the extra 1st row with describing the data) and select more than 2 cells in the Season 6 column to drag down until it reaches the end of the data you pasted in (selecting 2 cells with numbers when dragging it will duplicate the numbers Season 6, 6, 6, 6 instead of increasing Season 6, 7, 8, 9 etc)
Actually doing the meta analysis:
9. once the above steps are completed, graphics table master will have a space with checkboxes at the bottom (may need to unhide) which controls which weeks are filtered, click to add checkmarks to select the weeks you want
9. b hide the rows after you're done to download a pdf of the sheet on A4 paper
10. the dropdown list of each of the deck types are controlled by the pivot table on the count of decks sheet, change the filters on that to the weeks you selected and I normally do the order of the decks in the matchup player by most-least played
11. all graphics matchup table, here you select all decks played instead of top 10 in the previous one
12. the data on all graphics matchup table is sent to pie chart sheet

# Uploading files... work in progress...

