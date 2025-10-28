---
_last_editor_used_jetpack: block-editor
_oembed_8cb27a5590e596446089fa991aad4b3f: '{{unknown}}'
_oembed_23df4dfb6dec3e9be8f84ed9ec8dac79: <div class="embed-soundcloud"><iframe title="Jilted Breath by NearTao" width="500" height="400" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?visual=true&url=https%3A%2F%2Fapi.soundcloud.com%2Ftracks%2F972655576&show_artwork=true&maxwidth=500&maxheight=750&dnt=1"></iframe></div>
_oembed_f08b37f8139ec8a3882727c91776ff10: '{{unknown}}'
_oembed_time_23df4dfb6dec3e9be8f84ed9ec8dac79: "1611613811"
_publicize_done_22315546: "1"
_publicize_done_22890294: "1"
_publicize_done_external:
  twitter:
    "23256661": https://twitter.com/NearTao/status/1353745242361655296
_publicize_job_id: "53889230858"
_thumbnail_id: "324"
_wpas_done_23256661: "1"
_wpas_done_24391465: "1"
author: neartao
categories:
  - music-production
cover:
  alt: IMG_1679
  image: /wp-content/uploads/2020/01/img_1679.gif
date: "2021-01-25T16:43:07+00:00"
guid: https://neartao.com/?p=1880
parent_post_id: null
post_id: "1880"
publicize_tumblr_url: http://.tumblr.com/post/641301734579372032
publicize_twitter_user: NearTao
tags:
  - akai-mpc-live/x/one
  - mpc-test
timeline_notification: "1611592991"
title: Akai MPC Live/X/One Plugin Track Velocity Test
url: /2021/01/25/akai-mpc-live-x-one-plugin-track-velocity-test/

---
Based on the above MPC Forums topic [BUG ON MPC 2.9? PLUGIN TRACK LEVEL EFFECTS PROGRAM LEVEL](https://www.mpc-forums.com/viewtopic.php?f=48&t=210039) I created a test project to see if I could reproduce the issue below. In essence, the poster was stating that when they change the velocity setting on the track level for a plugin, that it was impacting the velocity setting for another track with the same plugin. Unfortunately this is mostly what I have for information at the time, making it difficult to either confirm or deny the problem. Below is some notes on what I attempted to test to see if I could figure out what the poster was hitting because this wasn't behavior that I had come across before.

[Plugin Velocity Test](/wp-content/uploads/2021/01/plugin-velocity-test.zip) [Download](/wp-content/uploads/2021/01/plugin-velocity-test.zip)

The project is setup as follows:

This is an MPC project created in standalone mode on Firmware 2.9.

I created a program "Program 01" with a kick on Pad A1, and a snare on Pad A2.

Track 01 (kick) - Program 01  
Track 02 (snare) - Program 01

When I reduced the velocity parameter on the track level for either Track 01 or Track 02, the behavior is that only the notes on the track are reduced, and it is not impacting notes played on the other track.

I created a second program "plugin 01" that was a tube synth, and assigned it to Track 03 and Track 04 to do a similar test as above.

Track 03 (tube synth C2 notes) - plugin 01  
Track 04 (tube synth C3 notes) - plugin 01

When I reduced the velocity parameter on the track level for either Track 03 or Track 04, the behavior is that only the notes on the track are reduced, and it is not impacting notes played on the other track.

So, the behavior is as I expected, and I think I need more details from the original poster to attempt to recreate this issue. There are a lot of other variables such as how the tracks are setup, which plugin is being used, if it is in standalone or controller mode, among other things. There is a lot unknown that makes it hard to reproduce the issue.
