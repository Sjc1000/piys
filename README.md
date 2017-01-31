# piys
piys - piys indexes your shows

piys is a tool that will index and check your shows against an online API. Thanks to http://www.tvmaze.com/

It will check if your files are in order and give you proper names for the files. This give you the ability to fix any broken or bad formats you may have downloaded.


# Installing
For now, its not on pip. I will put it up soon.

- Download the files.
- run `pip install . --user` in the root directory.

Then you can just use `piys` from the command line.

# Running

`piys /directory/to/show_name`

After this, follow the onscreen prompts until you get a list of the videos.

The list on the left is your video files, the one on the right is the proper order. You can your files in the program so they match up if they don't already.

**Key Combos**

- Up - Move the cursor up
- Down - Move the cursor down
- Space - Select a video.
- PgUp - Move selected video[s] up.
- PgDwn - Move selected video[s] down.
- C - Change the output format. This uses Python's format syntax, See below for the values you can use.
- Enter - Accept the current order and move the files to the new format.


**Variables**

- {season} - The season number.
- {episode} - The episode number.
- {title} - The title of the eipsode.
- {index} - The index of the file.
- {ext} - The file format of the original file.

Examle: Season {season}/{episode} - {title}{ext}

That example will produce something like,  Season 2/10 - Name here.mp4

**Note** - If the format has / in it, it will be treated as a folder.

