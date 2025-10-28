---
_last_editor_used_jetpack: block-editor
_oembed_6f03028c25bef2f06a2d6ad4c4f70c8c: <div class="embed-soundcloud"><iframe title="Long Voyage YAM by NearTao" width="500" height="400" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?visual=true&url=https%3A%2F%2Fapi.soundcloud.com%2Ftracks%2F962528446&show_artwork=true&maxwidth=500&maxheight=750&dnt=1"></iframe></div>
_oembed_2560a6082a4c01d265350b20410b5af7: <div class="embed-soundcloud"><iframe title="My Time Here Is Done by NearTao" width="750" height="400" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?visual=true&url=https%3A%2F%2Fapi.soundcloud.com%2Ftracks%2F961929730&show_artwork=true&maxwidth=750&maxheight=1000&dnt=1"></iframe></div>
_oembed_a0c0bc021264b5d7d0dca889169288f5: <div class="embed-soundcloud"><iframe title="My Time Here Is Done by NearTao" width="584" height="400" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?visual=true&url=https%3A%2F%2Fapi.soundcloud.com%2Ftracks%2F961929730&show_artwork=true&maxwidth=584&maxheight=876&dnt=1"></iframe></div>
_oembed_c981a273ab8bd22b3042561860f6c406: <div class="embed-soundcloud"><iframe title="My Time Here Is Done by NearTao" width="500" height="400" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?visual=true&url=https%3A%2F%2Fapi.soundcloud.com%2Ftracks%2F961929730&show_artwork=true&maxwidth=500&maxheight=750&dnt=1"></iframe></div>
_oembed_f996a81a84d50b5371faa94ff6f12df7: <div class="embed-soundcloud"><iframe title="Long Voyage by NearTao" width="500" height="400" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?visual=true&url=https%3A%2F%2Fapi.soundcloud.com%2Ftracks%2F962528446&show_artwork=true&maxwidth=500&maxheight=750&dnt=1"></iframe></div>
_oembed_time_6f03028c25bef2f06a2d6ad4c4f70c8c: "1610216155"
_oembed_time_2560a6082a4c01d265350b20410b5af7: "1610129704"
_oembed_time_a0c0bc021264b5d7d0dca889169288f5: "1610130326"
_oembed_time_c981a273ab8bd22b3042561860f6c406: "1610237520"
_oembed_time_f996a81a84d50b5371faa94ff6f12df7: "1610216178"
_publicize_done_22315546: "1"
_publicize_done_22890294: "1"
_publicize_done_external:
  twitter:
    "23256661": https://twitter.com/NearTao/status/1347610377710936064
_publicize_job_id: "53185016691"
_thumbnail_id: "1656"
_wpas_done_23256661: "1"
_wpas_done_24391465: "1"
author: neartao
categories:
  - music-production
cover:
  alt: f7a5f8df-cb19-42c9-b42a-304d5e1d45a1_1_105_c
  image: /wp-content/uploads/2021/01/f7a5f8df-cb19-42c9-b42a-304d5e1d45a1_1_105_c.jpeg
date: "2021-01-08T18:25:22+00:00"
guid: https://neartao.com/?p=1654
parent_post_id: null
post_id: "1654"
publicize_tumblr_url: http://.tumblr.com/post/639768017842159616
publicize_twitter_user: NearTao
tags:
  - access-virus-ti2-darkstar
  - akai-mpc-live-mk2
  - waldorf-iridium
timeline_notification: "1610130325"
title: '#jamuary2021 - My Time Here is Done'
url: /2021/01/08/jamuary2021-my-time-here-is-done/

---
The track was named as such... because I threw my hands up in desperation. \*not\* a good track, but I did learn something... but first

https://soundcloud.com/neartao/my-time-here-is-done

So the picture comes courtesy of the dang thing that the MPC Live did to twist up my song.

{{< figure src="/wp-content/uploads/2021/01/f7a5f8df-cb19-42c9-b42a-304d5e1d45a1%5F1%5F105%5Fc.jpeg?w=1024" alt="" caption="" >}}

Yeah, above is the drum track... but let me explain how I got there...

I figured I would play around with transpose on sequence mode... just do a pattern of I/IV/I/V... (or no semitone offset, +4 semitone offset, no semitone offset, +5 semitone offset). With me so far? I basically just copied my main sequence twice, second sequence I put a +4 semitone transpose on the sequence, and for the third sequence I put a +5 semitone transpose on the sequence. I then went to song mode and just did the pattern Seq 1, Seq 2, Seq 3, Seq 4... and then converted the whole thing back into a sequence.

When playing everything back, it sounded off and a little funny, but I didn't make anything off it immediately until I got to recording out past the end and could hear some drum noises playing that weren't supposed to be there. I wondered what it could be, and hopped off to the drum track to see if anything weird was going on... and saw the above pictured mess.

At first I was wondering why the notes were changing all willy nilly, and bouncing all over the place... and my guess is that because of how Akai (well generic MIDI really) has a drum map setup... I suspect that the PC is moving the events to the +/- semitone adjustment for where they are on the drum map. Personally I would say this is ridiculous... and it kind of is to do this for a drum map, but on the other hand I suppose I could see some interesting side effects to take advantage of such behavior to try and make some new drum patterns. I still think this behavior is weird, and I am going to look to see if I can find a way to disable this behavior on a per track basis... because frankly... you should be able to do a transpose adjustment to the entire track but ignore things like drum tracks.

Anyway... for me the simple fix was to just delete out the bung bars, and then copy and paste back in what I wanted. I can imagine this being a right mess had I exploded the drum hits to their own tracks... so I suppose user be warned... if you're going this route, don't explode and do mutes until \*after\* you have put the song into a sequence again.

There is, as usual with Akai workflows, a pretty easy fix... and this would be to do transposes at the track level, that way you can control what does and does not get transposed, but I still find the behavior at the sequence level a bit odd/awkward.

Until next time... I suppose.
