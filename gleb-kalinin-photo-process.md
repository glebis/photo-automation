## Intro
This file describes [Gleb Kalinin](http://glebkalinin.ru/)'s approach to processing and storing RAW files. This is work in progress, as I am still finding my ideal workflow. The purpose of this file is to create a comprehensive workflow description for a digital photographer, producing noticible amount of work on a regular basis. Some of the steps require purchasing certain software (FastRawViewer, CaptureOne), some are free to use by anyone.

## Principles
Hardware should be always ready to go and at full capacity:
* SD cards should be empty by the end of every image sorting. When you grab a camera, you should be certain you wouldn't need to worry about freeing card space.
* Latest sets, active ongoing projects should be accessible on your main computer, but also backed up daily to the external drive.
* 
* Batteries should be fully charged.

## File structure

Images are stored in a hierarchical chronological file structure:
yyyy/
  /yyyymm/
    /yyyymmdd photoshoot name

Images are sorted into this structure by a script that goes through each RAW file EXIF data, read its creating date and created a corresponding folder if needed. Photoshoot name is appended manually in [FastRawViever](https://www.fastrawviewer.com).

Primary culling is performed in camera or in FastRawViewer. The latter is a much faster alternative to any kind of import (LightRoom, CaptureOne). 

Second step of culling and selection of the keepers is performed in CaptureOne. Selection can be performed by viewing groups (of 2, 3, 4 or more photos) and navigating through groups using Alt+left/right arrow keys.

## Tethering

Tethering is performed in CaptureOne.
New scene/client = new Album name (as files are exported based on an album name), optionally a subfolder in Capture folder. 

h3. Additional backup using Automator script

## CaptrueOne

### Importing

Files are renamed in CaptureOne using following template: .

### Exporting

For exports I keep a single Outputs folder inside my main Pictures folder. My processing receipt created a folder accouding to the following template:
yyyymmdd (Collection name) by (Author)

[] (For now, Author is hardcoded into CaptureOne Preset text, good idea to use metadata for this).

[] Learn to automatically put an .URL file with a link to my page and a PDF file with basic info about my work. PDF should contain legal and distribution info, porfolio samples

[] Uploading using rsync

## Synology storage

Todo: Learn Synology to autobackup (and empty?) SD cards


