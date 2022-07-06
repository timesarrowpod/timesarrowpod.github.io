# How to add new posts

1. Log in to GitHub.

2. Go to [the `audio` directory](https://github.com/timesarrowpod/timesarrowpod.github.io/tree/main/audio). Click the "Add file" button, then "Upload files", then "Commit changes". Make sure the filename includes only letters and numbers. It must be an mp3.

3. Go to [the `_posts` directory](https://github.com/timesarrowpod/timesarrowpod.github.io/tree/main/_posts). Click the "Add file" button, then "Create new file". The name of the file should start with the current date in `2022-07-06` format, then a dash, and then a slug for the article. So if you want the post to be at `/episodes/2022/07/06/times-arrow-pt1.html`, then you would name it `2022-07-06-times-arrow-pt2`.

4. Copy the example episode template below and paste it into your new file. Follow the directions in the template to add all the required fields for the episode.

5. Click "Commit new file".

## Example episode (copy this)

```
---
layout: episode
title:  "Episode Title"
date:   2022-07-06 14:03:13 EDT
categories: episodes
image: "/images/siddig.png"
mp3_url: "/audio/hangupthephone.mp3"
mp3_length: 4013799
---
Everything after the second set of dashes is a description of the episode. The first paragraph (this paragraph) will be used as the excerpt.

Put the date and time in the date field.

Put the audio file for the episode in the "audio" directory. It must be an MP3. The filename can't
have any spaces or special characters (best to keep it to letters and numbers).

Put the size of the audio file *in bytes* in the mp3_length field. So if the mp3 is 4MB large, don't put
"4", put the exact number of bytes - "4013799".

Put an (optional) image for the episode in the "images" directory. The image filename shouldn't
have any spaces or special characters.

Make sure "episodes" is listed in the "categories" field and "layout" is "episode".
```

# How to change site settings

To change the site description, title, image, etc: edit `_config.yml`.