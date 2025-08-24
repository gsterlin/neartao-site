---
_publicize_done_22315546: "1"
_publicize_done_22890294: "1"
_publicize_done_external:
  twitter:
    "23256661": https://twitter.com/NearTao/status/1313565218212139009
_publicize_job_id: "49634979886"
_thumbnail_id: "1060"
_wpas_done_23256661: "1"
_wpas_done_24391465: "1"
author: neartao
categories:
  - music-production
cover:
  alt: Screen Shot 2020-10-05 at 4.48.46 PM
  image: /wp-content/uploads/2020/10/screen-shot-2020-10-05-at-4.48.46-pm.png
date: "2020-10-06T19:41:00+00:00"
guid: https://neartao.wordpress.com/?p=1049
parent_post_id: null
post_id: "1049"
publicize_tumblr_url: http://.tumblr.com/post/631256727252336640
publicize_twitter_user: NearTao
tags:
  - akai
  - autosampler
  - music-notation
timeline_notification: "1602013327"
title: Music Notation - Dynamics &amp; Akai Auto Sampler
url: /2020/10/06/music-notation-dynamics-akai-auto-sampler/

---
Well over at the MPC Forums a user created a topic [Tidy Keygroup Names](https://www.mpc-forums.com/viewtopic.php?f=48&t=204251) and thought that there was a bug when they were auto sampling, as it was putting f/p/fm/pm into the names of the samples instead of actual velocity. I chuckled to myself, because this seems kind of strange to show up into sample names.

Why is this strange you may ask? Well, for starters the auto sampler uses both the note names, as well as the midi note numbers in the file name when you auto sample an instrument. This makes sense, even if it is duplicate information. However, when you do multiple velocity levels, the auto sampler adds f/fm/pm/p (or a subset there of) into the file names. Strange huh? Especially if you don't know what it means.

The notation indicate loudness without specifying an actual or precise loudness. Essentially, it is up to the player to use their instincts, emotions, or placement within a surround environment and other instruments to determine how loud to play. To break it down for you, here's a table to explain the various f/mf/mp/p meanings

fffvery very loudffvery loudfloudmfnot so loudmpnot so quietpquietppvery quietpppvery very quietMusic Notation - Dynamics

So to break it down for the MPC, it's basically recording samples denoted as loud, not so loud, not so quiet, and quiet, which covers your four velocity levels.

This is a complete assumption, but I am guessing that the reason Akai would do this is that it requires at most 2 characters to represent the four velocity layers for the auto sampled content, instead of needing 3 characters to represent from 000 to 127.

Personally, I am not a fan of this style of notation, and would have much preferred to see Akai use either hexadecimal notation which would still utilize only two characters, or to have done something the F/f/p/P to use only one character. Instead we have the solution that Akai went with, which is obtuse, and doesn't really help the person auto sampling understand what the values actually are without opening up the Program to see what the content is. Oddly, this leaves the artist with a clear indication of what the note is, what the midi note is, but the artist is left to speculate what the velocity may or may not mean.

If you're looking for more information, check out the Wiki page [Dynamics (music)](https://en.wikipedia.org/wiki/Dynamics_(music)).

If you'd like to see some funny conversations on about this notation... read below

{{< figure src="/wp-content/uploads/2020/10/camkaef.jpeg?w=138" alt="" caption="" >}}
