---
_last_editor_used_jetpack: block-editor
_oembed_2c379a93055204ca72c5d05b1aa6dca7: <div class="embed-youtube"><iframe title="Syncing your MPC Live mk2/X/One to Eurorack Pamela&#039;s New Workout" width="750" height="422" src="https://www.youtube.com/embed/sfs5zI07JQw?feature=oembed" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></div>
_oembed_e635f6db36b810294278ab3365b373e6: <div class="embed-soundcloud"><iframe title="MPC Forums BB 278 - Bahia Destiny by NearTao" width="500" height="400" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?visual=true&url=https%3A%2F%2Fapi.soundcloud.com%2Ftracks%2F822495652&show_artwork=true&maxwidth=500&maxheight=750&dnt=1"></iframe></div>
_oembed_time_2c379a93055204ca72c5d05b1aa6dca7: "1725041441"
_oembed_time_e635f6db36b810294278ab3365b373e6: "1626395564"
_publicize_done_22315546: "1"
_publicize_done_22890294: "1"
_publicize_done_external:
  twitter:
    "23256661": https://twitter.com/NearTao/status/1400484639806996485
_publicize_job_id: "59167713179"
_thumbnail_id: "2917"
_wpas_done_23256661: "1"
_wpas_done_24391465: "1"
author: neartao
categories:
  - music-production
  - uncategorized
cover:
  alt: a72d63d9-e867-43ea-9f7c-3a1e5846e6c0_1_105_c
  image: /wp-content/uploads/2021/06/a72d63d9-e867-43ea-9f7c-3a1e5846e6c0_1_105_c.jpeg
date: "2021-06-03T16:08:49+00:00"
guid: https://neartao.com/?p=2907
parent_post_id: null
post_id: "2907"
publicize_tumblr_url: http://.tumblr.com/post/652986583256104960
publicize_twitter_user: NearTao
tags:
  - akai-mpc-live-mk2
  - akai-mpc-one
  - akai-mpc-x
  - eurorack
  - pamela&#039;s-new-workout
timeline_notification: "1622736532"
title: Syncing your MPC Live mk2/X/One to Eurorak Pamela's New Workout
url: /2021/06/03/syncing-your-mpc-live-mk2-x-one-to-eurorak-pamelas-new-workout/

---
https://youtu.be/sfs5zI07JQw

This video shows how to sync up your MPC Live mk2/X/One over CV gates to a Pamela's New Workout.

Honestly, I'm not too worried about the variance in the BPM that shows up at higher levels. I've monitored the gates being sent over CV and have seen that it is not dropping gates, so over time the average will be correct, even if there is a small variance in the BPM at a specific gate trigger.

I'll go over the setup here and show some pictures, as well as do some math to show roughly what the possible difference is for a note and how far off it might be.

## MPC Setup

To setup your MPC to send gates, it's pretty simple. First you'll want to pick a track, and change it to a CV Track type.

{{< figure src="/wp-content/uploads/2021/06/9e4c80b8-333d-4e05-bf30-16dfb5e37a6b%5F1%5F105%5Fc.jpeg?w=1024" alt="" caption="" >}}

As you can see above the CV PORT is set to CV 1, and the GATE PORT is set to CV 2. For this particular application I am not going to be sending CV information, I just want a consistent clock gate being sent. So let's change this.

{{< figure src="/wp-content/uploads/2021/06/0337d441-9dae-4dad-a9ca-eeb389882185%5F1%5F105%5Fc.jpeg?w=1024" alt="" caption="" >}}

For my purposes I have set GATE PORT to CV 1, but you can use any CV you have available to you. The only thing I'd say to remember is that you'll need a splitter if you're on the MPC Live mk2 or on the MPC One, otherwise you can only use the CV 1 through CV 4 outputs to interface with your Eurorack. I documented the splitter solution I have using at [Akai MPC Live mk2 / One CV outs](/2020/06/15/akai-mpc-live-mk2-one-cv-outs/) in case you're looking for a solution.

With this setup, you'll need to record some gates. For the MPC the easiest way to do this is to hold down NOTE REPEAT and lay out a single note consistently on your MPC. My process for this is to press Overdub and Play, then hold NOTE REPEAT set to 1/64 and hold down a single pad for the duration of the loop you've got setup. This will lay down a lot of note data at a consistently repeating timeframe that will function as our gate data for the MPC to send.

{{< figure src="/wp-content/uploads/2021/06/4bb7917b-dbad-4ed2-8a64-596bfdee0a18%5F1%5F105%5Fc.jpeg?w=1024" alt="" caption="" >}}

So what you put together should roughly look like the above. In this case I setup two bars of data, and if I need more then I can either record a longer Sequence, or just go to Sequence and x2 it to double the length. The important thing is that you have notes in place for every part of the sequence playing so that everything stays in time.

## Pamela's New Workout Setup

So the way that you sync Pamela's to your MPC is going to be through CV clock. One thing to note is that the more gates you send, the more accurate it will be and the faster it can react to a BPM change, but the more signals you send, the more you'll notice hiccups or oddities as they show up. We're talking about very small timeframes though, so it depends how sensitive you are.

The first thing you'll need to do is take the CV cable from your MPC and plug it into the Input Clk jack of your Pamela's New Workout.

At any rate, if you're on the BPM screen below, just do a long press on the Program knob. This will allow you to edit your settings to adjust your clock rate. Otherwise you ought to be able to rotate the Program knob to get yourself to the BPM page, and then do the long press.

{{< figure src="/wp-content/uploads/2021/06/a72d63d9-e867-43ea-9f7c-3a1e5846e6c0%5F1%5F105%5Fc.jpeg?w=1024" alt="" caption="" >}}

After you open up your settings menu, you'll want to rotate the knob to get to the PPQN setting. This is where you will set how many Parts Per Quarter Note that you will have. With a 1/64 Note Repeat, this means that you have 16 Parts Per Quarter Note. If you decided to record 1/64 Note Repeat with Triplets, you'll need to set your Parts Per Quarter Note to 48. So yes, you can send a wild

{{< figure src="/wp-content/uploads/2021/06/d39cce0e-9220-4f7f-85b7-f9f4371f8677%5F1%5F105%5Fc.jpeg?w=1024" alt="" caption="" >}}

With this said, you've should now be in sync. You may need to press the Start/Stop button to get the Pamela's New Workout to start triggering, and then you'll be off and going!

## Experiments

Below is some data that I collected by changing the PPQN values on Pam's and adjust the events on the MPC to match. I hooked up the Waldorf Iridium over Midi to watch for BPM variance as best I could and see how that might help correlate to the Pam's Variance.

BPMPPQNPam   
VarianceIridium   
VariancePam   
Stable201600.0Yes251600.1Yes301600.1Yes351600.1Yes381600.1Yes391600.1No901600.2No1001610.2No1201610.3No1901620.5No2501630.7No202400.0Yes252400.1Yes262400.1No302400.1No902400.2No1002400.2No1102410.2No1902410.5No2502420.7No204800.0No904800.2No1004800.2No1204800.3No1904820.5No2504820.7No

Just looking at the data I can already tell you that it's pretty obvious that the tolerance from Pam's is a function of how many events you are producing and how far they are off. This is why we're seeing a PPQN of 16 able to go to a higher BPM of 38 than the lower BPM's from the MPC with a higher PPQN, while maintaining BPM stability. This is roughly what I would expect.

Even with these BPM fluctuations coming from the MPC, you are still not seeing any displayed BPM fluctuations from Pam's until you break 100 BPM, and 120 BPM if you are using 48 PPQN.

## Conclusion

Am I bothered by this? Not even a little. I have confirmed that every single gate triggers, so you are not dropping events, which would be a problem. Further, the more events that you send, the faster that Pam's responds to the BPM changes and locks into the BPM.

Also, doing the math at 250 BPM, a variance of +/- 2 is less than 1% off (roughly 0.08%) for timing. Human's are typically not even that accurate, especially over long periods of time. I know some people get very particular about their BPMs, and seeing the displays wobble over time, but I am not one of those people. This is certainly close enough for me.

That said, I do have a breakout for Pam's, and I will be trying to sync Midi from Pam's to my other devices to also see how stable Pam's is for outputting a clock. Stay tuned!
