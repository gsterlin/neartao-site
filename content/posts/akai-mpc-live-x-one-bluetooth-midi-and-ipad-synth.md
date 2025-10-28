---
_last_editor_used_jetpack: block-editor
_oembed_ac02496d50c9760eef5ed256ef613e69: <div class="embed-youtube"><iframe title="Akai MPC Live/X Bluetooth Midi and iPad Synthesizers" width="750" height="563" src="https://www.youtube.com/embed/BkjlWcGXtMo?feature=oembed" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></div>
_oembed_b59cdad80d2282a4ddddbea441111e15: <div class="embed-youtube"><iframe title="Akai MPC Live/X Bluetooth Midi and iPad Synthesizers" width="500" height="375" src="https://www.youtube.com/embed/BkjlWcGXtMo?feature=oembed" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></div>
_oembed_time_ac02496d50c9760eef5ed256ef613e69: "1725008086"
_oembed_time_b59cdad80d2282a4ddddbea441111e15: "1726315147"
_publicize_done_22315546: "1"
_publicize_done_22890294: "1"
_publicize_done_external:
  twitter:
    "23256661": https://twitter.com/NearTao/status/1358803535840780290
_publicize_job_id: "54499095666"
_thumbnail_id: "2096"
_wpas_done_23256661: "1"
_wpas_done_24391465: "1"
author: neartao
categories:
  - music-production
cover:
  alt: IMG_1735
  image: /wp-content/uploads/2021/02/img_1735.jpeg
date: "2021-02-08T15:42:59+00:00"
guid: https://neartao.com/?p=2091
parent_post_id: null
post_id: "2091"
publicize_tumblr_url: http://.tumblr.com/post/642566309263048704
publicize_twitter_user: NearTao
tags:
  - akai-mpc-live-mk2
  - akai-mpc-live/x/one
  - apple-ipad
  - bluetooth-midi
  - ipad-synthesizers
timeline_notification: "1612798983"
title: Akai MPC Live/X/One Bluetooth Midi and iPad Synth
url: /2021/02/08/akai-mpc-live-x-one-bluetooth-midi-and-ipad-synth/

---
I figured I'd do a quick video to build on my last post [Akai MPC Live/X/One Bluetooth MIDI With an iPad](/2021/02/03/akai-mpc-live-x-one-bluetooth-midi-with-an-ipad/) where I had describe how to get a Bluetooth MIDI connection working. In this post I will cover how to quickly get audio out of your iPad into your MPC, and get the MIDI connection over bluetooth to control/sequence the synthesizer on your iPad.

Introduction

I recorded another video to go along with the post. If you'd prefer to follow step by step instructions I'll also write them up after the video.

https://youtu.be/BkjlWcGXtMo

MPC Audio Input Setup

By default, when you boot up your MPC, it is not going to have monitoring turned on. For the MPC X, this is less of an issue in some ways, since it can do hardware monitoring, but I'm going to go over the steps necessary to enable software monitoring for your MPC so that you can get audio into it so you can sample.

{{< figure src="/wp-content/uploads/2021/02/img%5F1725.jpeg?w=1024" alt="" caption="" >}}

From the Main menu, a quick way to get to the Sampler is to do one of the following

- Hold <SHIFT> and press <MIX>
- If configured, quickly double tap <MIX>
- Press <MENU> and then on the touch screen touch <SAMPLER>
- Hold <MENU> and press <PAD 9>

The last two options will work on any of the MPC Live/X/One models, and I know that there are shortcuts on the others. Personally, I frequently double tap <MIX>, but YMMV for this option depending on which MPC model you have.

{{< figure src="/wp-content/uploads/2021/02/img%5F1726.jpeg?w=1024" alt="" caption="" >}}

Above, you can see in the bottom left the button says "Off". This is telling you that for the Input 1,2 that is selected in this case, that the monitoring is Off, and you will not be able to hear any of the audio. Go ahead and touch where it says "Off" to turn monitoring "On".

{{< figure src="/wp-content/uploads/2021/02/img%5F1727.jpeg?w=1024" alt="" caption="" >}}

With Monitoring "On", you should be able to play any audio from your iPad (or any other device) that is hooked up to your MPC and hear sounds. If you don't hear anything, then check the volume on your device, the gain setting you have on your MPC, and make sure that you have the appropriate cables to route audio into your MPC.

{{< figure src="/wp-content/uploads/2021/02/img%5F1728.jpeg?w=1024" alt="" caption="" >}}

Now, to be able to control your synthesizer you have loaded on your MPC, you'll need to switch your Track to a MIDI track, that's what I have selected in the middle of the screen to make sure I can send MIDI information out from the MPC. Unfortunately, where "MIDI PORT" is, it currently says <none>, and if you scroll through your selections, you're going to see that you're probably not able to select your iPad as a target right now.

Connecting your MPC Bluetooth MIDI to your iPad

Before we kick off into this section, if you have not done these steps to setup Bluetooth MIDI, then check out my post [Akai MPC Live/X/One Bluetooth MIDI With an iPad](/2021/02/03/akai-mpc-live-x-one-bluetooth-midi-with-an-ipad/). This will get you off the ground.

Assuming you did follow my steps, and have powered off your devices, well this section is for getting you back into operation.

{{< figure src="/wp-content/uploads/2021/02/img%5F1729.jpeg?w=1024" alt="" caption="" >}}

Head over to your Bluetooth settings on your MPC, and you're likely to see something like this. Unfortunately, no matter how many times you select your iPad and hit CONNECT on the touch screen, nothing is going to happen. For whatever reason (and I am sure there are several, I just don't know them), you are not able to initiate a Bluetooth connection to your iPad from your MPC.

Instead, head over to the Bluetooth settings on your iPad.

{{< figure src="/wp-content/uploads/2021/02/img%5F1730.jpeg?w=1024" alt="" caption="" >}}

As you can see above, my MPC Live II is not connected, and to resolve this I just need to touch on the MPC Live II line to initiate the connection. So go ahead and do this now.

{{< figure src="/wp-content/uploads/2021/02/img%5F1732.jpeg?w=1024" alt="" caption="" >}}

You'll see a spinning icon, and hopefully this will end with a "Connected" displayed on the line.

{{< figure src="/wp-content/uploads/2021/02/img%5F1733.jpeg?w=1024" alt="" caption="" >}}

Heading back over to the MPC, you can confirm in the MPC Bluetooth settings that it is connected. We're almost there!

{{< figure src="/wp-content/uploads/2021/02/img%5F1734.jpeg?w=1024" alt="" caption="" >}}

To wrap things up, make sure you setup a MIDI track type, and select your iPad as the target MIDI PORT. Once this is done, and you have a synthesizer running on your iPad, you should be good to play instruments be able to hear them playing through your MPC and able to record them.

Conclussion and Notes

This is a really great way to be able to use your iPad as a synthesizer for your MPC. The iPad/iPhone apps have a world of great synths and sounds to draw from, so I encourage you to check things out over there.

One thing I do want to note though, is that I have found notes do get stuck from time to time, especially if you start running your iPad synthesizers in the background. I'll keep playing around with this, but I just wanted you to know that if you have a problem with notes getting stuck, you may need to go through the process to kill the application on your iPad and then reload it.

Good luck getting this setup for yourself, and as always have fun!
