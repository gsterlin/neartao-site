---
_last_editor_used_jetpack: block-editor
_publicize_done_22315546: "1"
_publicize_done_22890294: "1"
_publicize_done_external:
  twitter:
    "23256661": https://twitter.com/NearTao/status/1458425312778334211
_publicize_job_id: "65191613471"
_thumbnail_id: "3536"
_wp_old_date: "2021-11-10"
_wpas_done_23256661: "1"
_wpas_done_24391465: "1"
author: neartao
categories:
  - music-production
cover:
  alt: Audio Setup Sketch
  image: /wp-content/uploads/2021/11/audio-setup-sketch.jpg
date: "2021-11-09T13:03:00+00:00"
guid: https://neartao.com/?p=3535
parent_post_id: null
post_id: "3535"
publicize_tumblr_url: http://.tumblr.com/post/667471751922499584
publicize_twitter_user: NearTao
tags:
  - akai-mpc-live-mk2
  - behringer-rx1602
  - boss-sp-202
  - boss-sp-303
  - eurorack
timeline_notification: "1636550663"
title: Music Studio Audio Setup - Zoom H6 Issues and How I Addressed Them
url: /2021/11/09/music-studio-audio-setup-zoom-h6-issues-and-how-i-addressed-them/

---
I've been working on trying to figure out where I am having issues with my audio setup, to try and get a hotter signal in my video recordings. So I drew up a rough sketch to see if I could get some notes on what the issue might be and go from there...

{{< figure src="/wp-content/uploads/2021/11/audio-setup-sketch.jpg?w=1024" alt="" caption="" >}}

The long component with the knobs/buttons on it that is unlabelled is the Behringer RX1602 that I picked up... I just forgot to label it apparently.

At any rate, the issue I think I've been having has been that while listening through the MPC headphone out jack, everything is fine, there is no distortion, but the Zoom H6 when I listen to the audio piped in through there with the headphones plugged in I'm not seeing clipping, but hearing some to tons of distortion.

There's a lot of connections in this setup, and there are several changes from Line Level to Euro Level that makes this difficult, and an interesting challenge. The tone of a lot of sounds are changing subtly just going from the Akai MPC as a digital sample, to the Eurorack, through device changes even without an FX, back out of the Eurorack to the RX1602, then through the Boss SP-202 to Boss SP-303 chain, back into the RX1602, out to the MPC Live Inputs, and finally to my Monitors/Zoom H6 output. It's a lot of steps, and a lot of opportunity for clipping or other issues to occur. Plus, sometimes a sound goes in, and when it goes through everything it comes out like garbage. In other words, sometimes it comes out as a great sound, and others not so much.

Now... I'm not a sound engineer, I am aware of ohms and differences in ohms being a problem, and some of these things, but I also don't want to make anything up. Is there an impedance problem? Maybe... but from a "I have a problem" experience, what I have been accidentally recording has been digital clipping. I looked at the waveforms and was able to see it. I just find it incredibly weird that no matter how loud I have the volume out while the headphones are connected to the MPC that the headphones sound great with no distortion, but as soon as I connect them to the Zoom I hear it once the headphones are over about the 50% mark on the volume set on the MPC. It literally does not matter what the gain on the Zoom H6 is either... blah.

As an experiment, I ended up hooking the MPC headphone jack out to the Zoom H6 Capsule TRS 1/8" inputs. For whatever reason, this allowed me to set the Akai MPC volume knob up to about 75% for output before experiencing distortion on the Zoom H6 recordings. Given this change, I was also able to adjust gain on the Zoom H6 so that my signal was closer to -3db on the meter, which definitely helps make the recordings feel louder without getting distortion and clipping.

Ultimately I don't feel I have really come to understand the issue so much as I have been able to isolate where the issue is so that I can then work backwards on how to manage the issue better. I do feel like the TRS input on the capsule may be a better solution as it seems to have a bit more headroom for whatever reason, but it may also be better for me to hook the 1/4" outputs on the MPC directly to the Zoom H6, and then monitors from the Zoom H6. The reason I am not doing this right now is that I don't always want to have the Zoom turned on with my iPhone hooked up to it, because it just becomes "yet another device that needs to be turned on without necessarily adding any value" to the setup. On the other hand, the argument can be made that if I am monitoring at the end of chain I wouldn't be having these kinds of issues in the first place.

Conclusion: You're probably best off to catch these types of issues of loudness, clipping, etc... if you just monitor at the end so that you are hearing what the recording device is hearing. Who would have thought? Lol
