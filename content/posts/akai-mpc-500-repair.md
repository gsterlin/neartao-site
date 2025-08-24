---
_last_editor_used_jetpack: block-editor
_oembed_0eeaae8e0139faa28ce14434d55d4d0a: '<div class="embed-soundcloud"><iframe title="STBB #696 - Disco Gummy by NearTao" width="500" height="400" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?visual=true&url=https%3A%2F%2Fapi.soundcloud.com%2Ftracks%2F853394728&show_artwork=true&maxwidth=500&maxheight=750&dnt=1"></iframe></div>'
_oembed_c404a2464bb89b84092e565a24f16b6b: '<div class="embed-soundcloud"><iframe title="STBB #696 Disco Gummy [Non Entry] by NearTao" width="500" height="400" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?visual=true&url=https%3A%2F%2Fapi.soundcloud.com%2Ftracks%2F853634869&show_artwork=true&maxwidth=500&maxheight=750&dnt=1"></iframe></div>'
_oembed_time_0eeaae8e0139faa28ce14434d55d4d0a: "1594232310"
_oembed_time_c404a2464bb89b84092e565a24f16b6b: "1594232993"
_publicize_done_22315546: "1"
_publicize_done_22890294: "1"
_publicize_done_external:
  twitter:
    "23256661": https://twitter.com/NearTao/status/1279201452204920835
_publicize_job_id: "46164848506"
_thumbnail_id: "651"
_wpas_done_23256661: "1"
_wpas_done_24391465: "1"
author: neartao
categories:
  - music-production
cover:
  alt: IMG_1026
  image: /wp-content/uploads/2020/07/img_1026-e1593817420551.jpeg
date: "2020-07-03T23:52:43+00:00"
guid: https://neartao.wordpress.com/?p=644
parent_post_id: null
post_id: "644"
publicize_tumblr_url: http://.tumblr.com/post/622665785974947840
publicize_twitter_user: NearTao
tags:
  - akai-mpc-500
  - repair
timeline_notification: "1593820367"
title: Akai MPC 500 Repair
url: /2020/07/03/akai-mpc-500-repair/

---
So a few days back I posted about picking up an [Akai MPC 500 on Reverb](https://wordpress.com/block-editor/post/neartao.wordpress.com/620)... and it was absolutely a mess inside. In case you didn't see it, I'll post a picture below, but it was all jacked up. I suspect something heavy was dropped on it, or some other excessive amount of force. Maybe you can help decide?

{{< figure src="/wp-content/uploads/2020/06/99d1f477-1d68-410d-afad-a60e004da54c%5F1%5F105%5Fc.jpeg?w=768" alt="" caption="" >}}

So yeah, it was busted enough to snap the PCB in several places, and you can see where the metal frame got bent as well. Yesterday I picked up some Krazy Glue in preparation for the attempt for a big fix. I figured that particular glue would likely be the best way to hope to put the PCB back together as it does a really solid job bonding plastics. On the negative side, I am always getting this stuff stuck to my fingers and all over the place... so I wasn't exact thrilled to be working with it again.

To see if there was any hope, I ended up removing the PCB from the MPC, and a few parts kind of disintegrated, but it wasn't too bad, the master volume and the record volume knobs where effectively the only two things holding the upper portion of the board together. This helped a bit because most of the parts stayed attached, but it was made a bit more difficult to get the glue where it needed to go because the knobs were either in the way or where holding parts of the PCB in awkward positions. I decided this was a more desirable situation than trying to desolder all of the knobs to get a better job holding everything together with the glue. Especially since the PCB was so warped already that I suspected it wouldn't matter all that much.

{{< figure src="/wp-content/uploads/2020/07/img%5F1020.jpeg?w=768" alt="" caption="" >}}

Here you can see me getting some of the supplies ready including the glue, and just taking a good look at the board. There were four major fractures on the PCB, and the important thing for me was to preserve the board since I could not get another one through MPC Stuff unfortunately, and also because this would at least need to function as a base for me to solder everything to. One thing you cannot see from these pictures is that almost all of the solder joints have torn away from the PCB, and if you don't know what that means, well it means there is going to be a lot of soldering to do, since I cannot trust any of the bridges from the PCB to function since many of them were torn, and it is next to impossible to reattach the copper traces back to the PCB.

Below you can see what the PCB board looks like with everything glued back together. It is a bit janky still, but it is actually far more solid than I had anticipated. Fortunately none of the resistors were broken, and the trances to the resisters were at least all preserved. On the sad news, now that I could get a better look, you can see just how absolutely filthy the PCB is. I suspect it may be from excessive humidity, though I am not entirely sure. One thing I do know though, is that the device itself stinks like food... possibly curry. I'm going to have to tear the MPC 500 apart and scrub there whole thing down. It's not too much more work than I had intended anyways, since I was planning on stripping it down to replace the capacitors.

So I guess my take aways from the picture below, this thing is dirty as heck, and I had been hoping that I could bridge the PCB fractures with some small solder joints. At this point though, you can see what that huge gap, that is not going to happen. This is going to require running wire traces to replace all the broken joints, and unfortunately I don't have a way to really test if any of the knobs are working... the risk is that this could be a lot of work, and it still might fail.

{{< figure src="/wp-content/uploads/2020/07/img%5F1021.jpeg?w=768" alt="" caption="" >}}

Below is a picture after running most of the traces. This was probably three hours of work for me. Please note, I have not done much soldering in years, and I didn't have a good wire stripper so I was making due with the Swiss Army knife. Yeah, it took longer, but I just kept plowing through.

{{< figure src="/wp-content/uploads/2020/07/img%5F1023.jpeg?w=1024" alt="" caption="" >}}

Below shows me just hooking it up to test, without mounting it. I figured I'd run on batteries so I don't accidentally electrocute myself, and it was a quick way to see if it worked. Good news everybody... the left channel output worked, but strangely not the right channel. I also had a weird bug where I could hear the audio ins played directly through to the outputs. I'm not sure what path I had accidentally bridged, but I thought to take a mental note that it could be useful in the future depending on how much hacking I want to do on this device. The other problem I had was that the left audio channel was the only input that seemed to be working as well. Presumably I really messed up the paths on both of the knobs to some degree.

{{< figure src="/wp-content/uploads/2020/07/img%5F1025.jpeg?w=1024" alt="" caption="" >}}

Overall I ended up having to pull it apart and I ended up testing all of the paths, and ended up finding out that about six of them were wrong... whoops. I guess I should have read the traces from the board better. Unfortunately with the break it made it a little harder to read. I probably should have searched for a service manual, but I figured I was close enough that it was worth it to plow through further. One other problem I accidentally caused myself was that I removed two bridges from the knobs. Another oops... and this made the knobs only work on one of the input and one of the output channels.

{{< figure src="/wp-content/uploads/2020/07/img%5F1026-e1593817420551.jpeg" alt="" caption="" >}}

So after playing around a bit and getting everything to work it was time to screw it in and make sure that the case fit in properly and there weren't any problems with my wires getting in the way. I had a few solder joints get loose and disconnect, probably cold joints, so I did have to redo the solder a few times.

Below you can see that the board is a little bit wiggly still, even though it is screwed into the case. I was concerned about screwing it in too tight, so I give it a tiny less than I would normally do when mounting one of these boards.

{{< figure src="/wp-content/uploads/2020/07/img%5F1027.jpeg?w=768" alt="" caption="" >}}

This last image shows that at least everything fits in properly... 'ish. It does work though, and while it was a really big time sync so far (all in probably five hours), at least it is working.

{{< figure src="/wp-content/uploads/2020/07/img%5F1028.jpeg?w=768" alt="" caption="" >}}

Next up I think I'll be recapping he audio related capacitors. It isn't actually terribly noisy, but I know these tend to give out from previous experience, and I think while I have the time I will get the capacitors replaced. I've also got a few other fun goofy projects with the MPC 500, so I might try my hand at hacking and modifying it up a bit.

Stay tuned!
