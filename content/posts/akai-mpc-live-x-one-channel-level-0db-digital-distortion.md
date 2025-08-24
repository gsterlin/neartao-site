---
_last_editor_used_jetpack: block-editor
_oembed_2ea5383fea8b880ea2f2d1e294d484b6: <div class="embed-soundcloud"><iframe title="Feeling Of Falling Down by NearTao" width="500" height="400" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?visual=true&url=https%3A%2F%2Fapi.soundcloud.com%2Ftracks%2F969579925&show_artwork=true&maxwidth=500&maxheight=750&dnt=1"></iframe></div>
_oembed_ed3ac648715b7dab633ab0fd9b970cfa: <div class="embed-youtube"><iframe title="MPC Live/X/One Channel Level Over 0db Distortion Test" width="750" height="422" src="https://www.youtube.com/embed/az0yqx5eSIQ?feature=oembed" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></div>
_oembed_time_2ea5383fea8b880ea2f2d1e294d484b6: "1611188683"
_oembed_time_ed3ac648715b7dab633ab0fd9b970cfa: "1726106443"
_publicize_done_22315546: "1"
_publicize_done_22890294: "1"
_publicize_done_external:
  twitter:
    "23256661": https://twitter.com/NearTao/status/1351626759926652929
_publicize_job_id: "53650900794"
_thumbnail_id: "1812"
_wpas_done_23256661: "1"
_wpas_done_24391465: "1"
author: neartao
categories:
  - music-production
cover:
  alt: Screen Shot 2021-01-19 at 3.24.16 PM
  image: /wp-content/uploads/2021/01/screen-shot-2021-01-19-at-3.24.16-pm.png
date: "2021-01-19T20:25:02+00:00"
guid: https://neartao.wordpress.com/?p=1807
parent_post_id: null
post_id: "1807"
publicize_tumblr_url: http://.tumblr.com/post/640772114662735872
publicize_twitter_user: NearTao
tags:
  - akai-mpc-live-mk2
  - eurorack
timeline_notification: "1611087905"
title: Akai MPC Live/X/One Channel Level 0db Digital Distortion
url: /2021/01/19/akai-mpc-live-x-one-channel-level-0db-digital-distortion/

---
Over at MPC Forums [Monstre Sensible](https://www.mpc-forums.com/memberlist.php?mode=viewprofile&u=105910) kicked off a thread [Export Song](https://www.mpc-forums.com/viewtopic.php?f=48&t=209558). A key question asked what happens to audio over the 0db mark, and if this could be considered headroom. I was ready with the "here is the manual page" to describe the behavior, but Akai didn't actually document what happens in the manual. So... time to get some scientific experiments started.

In response I setup a little test, using a normalized single cycle loop, and hooked it up to my Eurorack oscilloscope so I could see what was happening. In theory, this should determine if we have digital distortion in the MPC Live/X/One on the Channel Volume or not.

[0db Digital Distortion](/wp-content/uploads/2021/01/0db-digital-distortion.zip) [Download](/wp-content/uploads/2021/01/0db-digital-distortion.zip)

Above is the project file that I created for the test, in case you want to check my work. You can also verify what is happening by simply resampling the audio in the Sampler. It sill show the same (technically more accurate because there is no ADDA conversion) digital distortion.

https://youtu.be/az0yqx5eSIQ

Above is the video that I recorded to show what is happening, and you can see the characteristic squaring of the sample from moving beyond 0db in the MPC's channel volume. The little notch/spike you can see on the oscilloscope I attribute to the analogue gear that I have, and not anything "fancy" that the MPC is doing to add sound.

Summary, the MPC is just flat out digital clipping audio about 0db. So consider that when you are mixing. Later!
