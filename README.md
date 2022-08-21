# LMAuploader
Scripts to help upload bootlegs to the Live Music Archive on the Internet Archive
# Requirements
- The latest version of python. Please consult the internet for this, it can be finicky to set up.
- The internetarchive library. Instructions for installation can be found [here](https://archive.org/services/docs/api/internetarchive/installation.html).
- Your archive.org credentials in a config file. This can be done by running `ia configure` and entering your email and password.
- A folder of the music files you are trying to upload to LMA, placed in the same folder as the script.
- ``music-tag``, a Python library that allows for the program to read from audio file tags.
- ``lxml``, a Python library for HTML parsing.
# What the script does
The `upload.py` script allows the user to input the information required to upload a bootleg to LMA, generates an info file, and gives the option to rename the files. Run the script using `python upload.py` while in the same folder as the two scripts and the folder of music files to upload. The script will prompt you for the required information, as well as any optional fields. When it comes to enter the setlist, first enter the total number of entries when prompted, then paste the entire setlist after the next prompt. If successful, the script will notify the user and print the link of the archive.org entry. 
# What the script does not do
Please also ensure that all the files you are uploading exist in the same folder that is entered when prompted. These scripts also do not affect the tags of the music files. To edit those please use separate software. 
# Bugs
If you encounter bugs or errors please report an issue. Thank you!
# TODO
- Create more streamlined CLI user experience with argparse.
- Package better to reduce dependencies. 
