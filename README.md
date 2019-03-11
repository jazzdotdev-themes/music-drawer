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
    video_id = "", #needed
    list_id = "",  #optional
  }

  video = { #at least one needed
    mp4_src = "",
    ogg_src = "",
    webm_src = "",
    gp3_src = "", #for 3gp format because parameters can't start with a number
  }

  audio = { #at least one needed
    mp3_src = "",
    ogg_src = "",
  }
```  
The template will only display the first media to be found in this
order youtube , video  or audio
all configurations need at least one source 
the youtube configuration will need at least the youtube id

Example: if the audio tag is the only one send , template will use that media configuration.
```
  audio = {
    mp3_src = "",
    ogg_src = "",
  }
```

Example of html implementation in ```layouts/base_example.html```
