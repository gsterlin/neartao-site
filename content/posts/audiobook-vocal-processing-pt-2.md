---
_last_editor_used_jetpack: block-editor
_publicize_done_22315546: "1"
_publicize_done_22890294: "1"
_publicize_done_external:
  twitter:
    "23256661": https://twitter.com/NearTao/status/1280947973879283713
_publicize_job_id: "46343576374"
_thumbnail_id: "587"
_wp_old_date: "2020-07-08"
_wpas_done_23256661: "1"
_wpas_done_24391465: "1"
author: neartao
categories:
  - music-production
cover:
  alt: IMG_0981
  image: /wp-content/uploads/2020/06/img_0981.jpeg
date: "2020-07-06T19:19:00+00:00"
guid: https://neartao.com/?p=677
parent_post_id: null
post_id: "677"
publicize_tumblr_url: http://.tumblr.com/post/623102417120231424
publicize_twitter_user: NearTao
tags:
  - ableton-live
  - audio-book
  - somnium-beyond-the-darkness
timeline_notification: "1594236769"
title: Audio Book Vocal Processing Pt. 2
url: /2020/07/06/audiobook-vocal-processing-pt-2/

---
Well I just (hopefully) wrapped up the audio processing for my sister's book. Since the last post, I probably could have done three other posts about the series of events that happened. Suffice it to say that there are some competing formats, tools, and audiobook sites that aren't exactly in alignment.

So... I had gotten my sister's book all processed, converted to .mp3 format, and she was quite happy with the sound. Unfortunately she doesn't really understand audio processing or audio file formats, so this kicked off a chain of unfortunate re-exports. Each process and export job probably took me 60-90 minutes... and since I had only ever expected to do this twice, I never automated the job. Each time I ended up processing the files, it was "just one more change" which had me shrug, and go off and do a whole bunch of clicking to re-process the files again. After time five, you'd think I would have learned my lesson. Which I did, but maybe not the one you'd think.

I guess I will just dump a few thoughts and notes for somebody who might stumble upon this post, or to remind myself in the future in case I forget...

First, Amazon's website for posting audio books is kind of a mess, and doesn't exactly give the best information about some of the problems. The best example I will give is that I exported the audio files as mono 320kbps .mp3 files... Ableton Live can only export to 320kbps for .mp3, and Amazon requires a minimum of 192kbps anyways. However, Amazon threw an error for the upload that the file was only 160kbps. Guess what, Amazon sees a 320kbps mono file as a 160kbps file, because apparently it doesn't know the difference between mono and stereo. The fix was simple, just export the file as stereo, but it was a mono recording... making it kind of a 'dumb' fix.

Second, RMS was a problem, as it is the average volume of a file, and not the peak. This is fine, and why I was doing mild compression on my sister's voice, but Amazon also requires that you don't peak over -3db, so you cannot just normalize your audio, and instead need to process a bit differently. I forget all the intermediate tweaks, but I ultimately ended up adding a Push limiter from Ableton Live, and set the max value to -3db, which remediated the problem quite nicely, but as I said, was another round of processing.

Third, my sister wanted to backing music to her intro and closing tracks, which was nice, but she wanted the music very quiet so that it wouldn't disturb her reading, and she didn't want the music to be ducked by her speaking, since this was bound to sound weird to the listener. Oh, and she wanted only about 1/3 of the file to be spoken word. This hit the hardest RMS issue, and while I could have raised the volume, this isn't what she wanted. So instead, I basically just started trimming the track from the start and end a bit, until we were able to fit within the RMS parameters, while also keeping the maximum volume below -3db.

I guess the bad news is the entire investment of time was significantly higher than I had anticipated, but the good news is that I have a pretty good audio processing chain that I can use for my sister's next audio book when she finishes her writing.
