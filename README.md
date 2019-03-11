# Instructions of Use and Installation 

Include in the page the tags for 
the scripts and the template
```
include "chunks/music-drawer.html"
  
include  "chunks/music_box_script.html"
```  

send the information of the media to be displayed
in the following format
```  
  youtube = {
    video_id = "",
    list_id = "",
  }
  video = {
    mp4_src = "",
    ogg_src = "",
  }
  audio = {
    mp3_src = "",
    ogg_src = "",
  }
```  
The template will only display the first media to be found in this
order youtube , video  or audio
also if a configuration is found for any of this media the template
will asume it has all the necessary data for it.

Example: if the audio tag is the only one send , template will use that media configuration.
```
  audio = {
    mp3_src = "",
    ogg_src = "",
  }
```

Example of html implementation in ```layouts/base_example.html```
