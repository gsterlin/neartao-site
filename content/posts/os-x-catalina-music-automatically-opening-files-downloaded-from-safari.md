---
_publicize_job_id: "37450963613"
author: neartao
categories:
  - technology
date: "2019-11-15T12:49:38+00:00"
guid: https://neartao.wordpress.com/?p=173
parent_post_id: null
post_id: "173"
tags:
  - automatic-opening
  - music
  - os-x-settings
  - safari
timeline_notification: "1573822180"
title: OS X Catalina - Music Automatically Opening Files Downloaded from Safari
url: /2019/11/15/os-x-catalina-music-automatically-opening-files-downloaded-from-safari/

---
TL;DR go to Safari -> Perferences -> General, and uncheck Open "safe" files after downloading to disable automatic opening of files downloaded by Safari.

A problem I've had with downloading content in OS X has been that a lot of files will automatically open once you've downloaded them. For compressed files, it will uncompress them, for PDFs it will automatically open them into Preview, and for audio files it will automatically start playing them in Music. For the compressed files, PDFs and others, I'm often not downloading enough of them to be too upset by this feature, but when I am downloading stems, one shots, or other audio content, I don't always want it automatically imported into Music.

I spent some time digging through the Music app preferences to see if I can find a way to disable this behavior. I had wrongly assumed that it was the Music app that was automatically importing content. After some searches around the web I found this [video](https://www.youtube.com/watch?v=XOhwo1RXlw0) that describes how to disable this behavior.

To properly resolve this issue go to Safari -> Perferences -> General, and uncheck Open "safe" files after downloading.

{{< figure src="/wp-content/uploads/2019/11/screen-shot-2019-11-15-at-7.42.35-am.png?w=1024" alt="" caption="" >}}

Unfortunately this feature does not have granular control over different file types. If you like this feature, but specifically don't like it for audio files, I suspect you'll have to disassociate the audio files from specific applications. Personally I'm okay with loosing the automatic opening of PDF files as that has been a hassle in the past, but uncompressing content has been a handy feature.
