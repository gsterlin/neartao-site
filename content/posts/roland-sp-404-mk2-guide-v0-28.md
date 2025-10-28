---
_last_editor_used_jetpack: block-editor
_publicize_done_22890294: "1"
_publicize_job_id: "85769618203"
_thumbnail_id: "3614"
_wpas_done_24391465: "1"
author: neartao
categories:
  - music-production
cover:
  alt: Untitled
  image: /wp-content/uploads/2022/01/untitled.jpg
date: "2023-07-15T15:03:54+00:00"
guid: https://neartao.com/?p=3940
parent_post_id: null
post_id: "3940"
publicize_tumblr_url: http://near-tao.tumblr.com/post/722923357590405120
tags:
  - roland-sp-404-mk2
timeline_notification: "1689433437"
title: Roland SP-404 mk2 Guide v0.28
url: /2023/07/15/roland-sp-404-mk2-guide-v0-28/
wordads_ufa: s:wpcom-ufa-v3-beta:1689434118

---
Just a few simple tweaks for today based on some information I learned while running a few experiments (and answering questions) on my live stream at https://youtube.com/live/LT8YEWt7zuY?feature=share

The plan was to figure out a few volume maximums/limits, especially for recording. I decided to use the USB-C audio interface connection from the SP404 mk2 to my computer since it is a digital connection and I assume (a bit grossly perhaps) that it should be consistent for us. From here, I spent some time recording test tones, tried to record as loud as I could through the line ins and mic/inst jack without clipping, and then did some comparative analysis through Ableton Live to see how these various recordings compared to normalized audio.

Overall, it looks like there is a hard -3db limit for recording in. You can compensate for this with normalization, but this headroom appears to be reserved for the FX bus, as you can record the input through the FX and get samples that peak at 0db. Interesting for sure, but I don't have a straightforward way to 'defeat' the -3db limit through an FX chain that doesn't color the sample in some way, or otherwise avoid normalization. Normalize, it's fine, and not going to hurt anybody. That, or record someplace else, and then import the sample through the Application or an SD Card.

I got some questions, and actually spent possibly way too long on it, but dug a bit into sample length limits. It appears that the limit for samples is 185,506,412 bytes, and not the advertised 16 minutes. This really only matters in so much as you can load a mono sample that is up to 32 minutes. I suspect that this is an important tidbit for DJs who are looking to drop in mixes into their set that are longer than the 16 minute limit, but only just a guess. I am sure that there are uses for ambient folks out there as well, though this is an output only hack. Since the mk2 cannot record in mono only (it always records as stereo, even for mono input), you can only go so far with this. Regardless I hope it helps somebody.

I measured the impact of the System setting under GAIN for Attenuator, and unless my math is wrong, it looks like it is an easy to calculate -14db drop in audio volume if it is turned on. 99% of the time there is no reason to have this turned on, but I suppose if you have a device with no gain knob, it can get you by. Now it just makes me wish that there was a line in attenuator on the back though so I could get a bit of gain or drop the gain if I wanted to. It is what it is though.

As a result of all this tweaking I also added a section about maximizing recording volume into the Sampling Chapter. If you're struggling with quiet samples, check it out and see if it can help you get a bit louder.

Thanks everyone for your support and have a wonderful day!

[neartaos-sp-404-mk2-guide-0.28-1](/wp-content/uploads/2023/07/neartaos-sp-404-mk2-guide-0.28-1.pdf) [Download](/wp-content/uploads/2023/07/neartaos-sp-404-mk2-guide-0.28-1.pdf)
