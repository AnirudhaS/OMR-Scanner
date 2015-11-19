OMR-Scanner
===========

This was my final year project during Bachelor's (computer engg.)

This is a OMR Scanner Desktop application. It scans a predefined set of sheets(given as pdf for modeling inside), 
and gives the solutions for marked questions.

This is made to be compatible with a normal flatbed scanner which is cheaply available. The generic systems use expensive scanners
designed for the speicific job. 

Application will require .net 4 framework runtime. The scanner configuration and setting is handled the application. 
It uses Aforge's .Net library for image processing, and pre-processing. Since, due to that this is a resource heavy application
and it is recommended to use faster processor (2.6GHz+) with plenty of memory (2 GB).

There is some basic setup needed. These settings can be changed in the Worker.cs file. 
- Creation of a file named 'FileInfo' in 'D:\OMRSoft\'. This file holds the required information for basic file management and data storage storage functionality. 
It holds the following information in the order, separated by newlines,
  - ```scanned_image_index``` = The image number for the next scanned file.
  - ```scanned_img_dir```     = The directory for sotring the scanned files.
  - ```answer_key_dir```      = This gives the directory for basic text file including the answer key choices.
  - ```templates_dir```       = This will include XML temapltes giving the coordinates for the OMR sheet.
  - ```db_path```             = This has the Database path where resulting information is stored.
Of the above only template directory is important, as other information can be edited after basic understandng of the source code. 
