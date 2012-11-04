# Postprocessing Script for SABnzbd+

To use the script, extract the zip into your sabnzbd script folder and select sabtoanidb.py as your post processing script in your anime category.

You have to enter your anidb username and password into the config file. also you have to modify the target directory in the config file to tell the script, where your anime folder is. (the script will copy the files to a directory with the name of the anime in that folder.)

Note:
If you use the delete option to delete the sourcefolder after moving, external sub-files will be lost!

## Tags for renaming:

    %ATr%: Anime Name (Romaji)
    %ATe%: Anime Name (English)
    %ATk%: Anime Name (Kanji)
    %ATs%: Anime Name (synonyms) (lists all synoyms currently)
    %ATo%: Anime Name (other)
    
    %ETr%: Episode title (romaji)
    %ETe%: Episode title (english)
    %ETk%: Episode title (kanji)
    
    %GTs%: Group Name (short)
    %GTl%: Group Name (long)
    
    %EpHiNo%: Highest (subbed) episode number
    %EpCount%: Anime Episode count
    %AYearBegin%: The beginning year of the anime
    %AYearEnd%:  The ending year of the anime
    %ACatList%: Category of the Anime
    
    %EpNo%: File's Episode number
    
    %Type%: Anime type, Value: Movie, TV, OVA, Web
    %Depr%: File is deprecated if the value is '1'
    %Cen%: File is censored if the value is '1'
    %Ver%: File version
    %Source%: Where the file came from (HDTV, DTV, WWW, etc)
    %Quality%: How good the quality of the file is (Very Good, Good, Eye Cancer)
    %AniDBFN%: Default AniDB filename
    %CurrentFN%: Current Filename
    %FCrc% : The file's crc
    %FCRC%: The file's crc in upper letters
    %FVideoRes%: Video Resolution (e.g. 1920x1080)
    %FALng%: List of available audio languages
    %FSLng%: List of available subtitle languages
    %FACodec%: Codecs used for the Audiostreams
    %FVCodec%: Codecs used for the Videostreams
    %suf%: File Suffix


## anidb.py has several commandline arguments:

```
Options:
  -h, --help            show this help message and exit
  -u USERNAME, --username=USERNAME
                        AniDB username.
  -p PASSWORD, --password=PASSWORD
                        AniDB password.
  -r, --recursive       Recurse into directories.
  -s SUFFIX, --suffix=SUFFIX
                        File suffix for recursive matching.
  -c, --no-cache        Do not use cached values.
  -l, --multihash       Calculate additional checksums.
  -i, --identify        Identify files.
  -a, --add             Add files to mylist.
  -w, --watched         Mark files watched.
  -n, --rename          Rename files.
  -m, --move            Move Files
  -x, --delete          Delete Folders after moving files
  -d DIRECTORY, --directory=DIRECTORY
                        Target parent directory.
  -o, --no-color        Disable color output.
```
