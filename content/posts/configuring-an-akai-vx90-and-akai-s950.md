---
_last_editor_used_jetpack: block-editor
_publicize_done_22315546: "1"
_publicize_done_22890294: "1"
_publicize_done_external:
  twitter:
    "23256661": https://twitter.com/NearTao/status/1363158202947276802
_publicize_job_id: "55046707523"
_thumbnail_id: "2295"
_wpas_done_23256661: "1"
_wpas_done_24391465: "1"
author: neartao
categories:
  - music-production
cover:
  alt: IMG_1804
  image: /wp-content/uploads/2021/02/img_1804.jpeg
date: "2021-02-20T16:06:40+00:00"
guid: https://neartao.wordpress.com/?p=2294
parent_post_id: null
post_id: "2294"
publicize_tumblr_url: http://.tumblr.com/post/643654974869553152
publicize_twitter_user: NearTao
tags:
  - akai-s950
  - akai-vx-90
timeline_notification: "1613837204"
title: Configuring an Akai VX90 and Akai S950
url: /2021/02/20/configuring-an-akai-vx90-and-akai-s950/

---
I spent a few hours messing around with the configuration, and trying to get everything to work. It is not exactly straight forward, and I had to dig through a lot of old posts and try and understand what exactly different sources were trying to tell me. I found a few that indicated that it should work polyphonically, but didn't exactly describe the steps to get there, or said things a little too generically. I can say, I now have it all working (yeah!), and will go through how to get this setup step by step, where you might hit a few problems, suggestions to test out issues. Let's get into it :D

Hardware Setup

First thing is first, you're going to need a few things... an Akai VX90, and Akai S950, a 13-pin cable, and a midi controller than can output midi notes.

{{< figure src="/wp-content/uploads/2021/02/img%5F1777.jpeg?w=1024" alt="" caption="" >}}

Sorry, I'm not going to be able to help you with sourcing the Akai gear... and I understand, it is super pricey.

Below is what the 13 pin connector looks like. I ended up getting mine off of eBay, by searching for " **13-PIN MIDI ROLAND GUITAR SYNTH INTERFACE CABLE**". The one I got is pin compatible, and I believe can actually carry all eight voices of the Akai S950 over, but... for this application we're only going to be able to use six of the eight voices, since the Akai VX90 can only support six voices. For those of you wondering, you really cannot take advantage of the other two voices in a meaningful way, so while I may look into a few applications in the future, just consider this a six voice only operation. If you want to experiment go nuts, but you'll be on your own :D

{{< figure src="/wp-content/uploads/2021/02/img%5F1779.jpeg?w=1024" alt="" caption="" >}}

The back end of both of your synths should look similar. Though you might not have the IB-105/IB-109 on your S950. Don't worry if you do not have either, we won't be using those connections for this setup.

{{< figure src="/wp-content/uploads/2021/02/img%5F1778-2.jpeg?w=1024" alt="" caption="" >}}

Of note though, and before things get covered with cables, is that you'll want to pay attention to the SAMPLER IN, MIDI IN, and MIDI OUT on your VX90, and VOICE OUT and MIDI IN on your S950. The VX90 does some MIDI magic to transform incoming notes into different MIDI Channel events on the S950 over the MIDI OUT port, so you won't be able to take advantage of MIDI THRU without a lot of rewiring and other things I'm definitely not going to cover here.

As you can see, the 13 pin cable I got is ridiculously long, but even though it is about six feet long, it still works fine. So go ahead and plug that into your VX90 SAMPLER IN port, and your S950 VOICE OUT port. Just be careful to make sure that your pins are aligned correctly, and you should be all set.

{{< figure src="/wp-content/uploads/2021/02/img%5F1780.jpeg?w=1024" alt="" caption="" >}}

Next up is plugging in your MIDI. From your controller, plug the MIDI OUT into the VX90 MIDI IN. If you want to test it, you can just try and play some notes from your VX90 right now if you've got it hooked up to a mixer.

Then from the VX90 MIDI OUT, hook that up into your S950 MIDI IN. This will get you all of the routing that you should need setup through hardware for the MIDI.

Finally, hook up the audio from the VX90 to your input. In my case I used the Phono outputs in the front of the VX90 because my STEREO outs on the VX90 are quite noisy. Something to repair in the future for certain.

{{< figure src="/wp-content/uploads/2021/02/img%5F1783-1.jpeg?w=768" alt="" caption="" >}}

Akai VX90 Setup

With all of that completed, you now have the hardware configured properly, but besides seeing if the VX90 plays, you are not likely going to be able to hear your S950 samples quite yet, because now we need to configure the software to actually do something.

Let's start with the VX90 configuration. To configure the VX90, you're doing to need to press the EDIT button. You can see it is on for me because the red LED has turned on, and I now see in the menu Exx to indicate I am in edit mode.

{{< figure src="/wp-content/uploads/2021/02/img%5F1786.jpeg?w=1024" alt="" caption="" >}}

Next we'll need to move over to the menu item E06 to configure the Sampler mode. To navigate through your edit options, look to the SELECT or number buttons and you'll see BWD to move backwards, and FWD to move forwards. In all likelihood you'll need to use FWD to move over to E06, and then use the VALUE slider to make sure it is set to ON. Once it is on you will see the SAMPLER LED light up red, indicating that the VX90 can now receive audio information from the S950.

{{< figure src="/wp-content/uploads/2021/02/img%5F1788.jpeg?w=1024" alt="" caption="" >}}

Next up is to adjust a-b balance, which allows us to mix how much audio comes from the VX90 and how much comes from the S950. For now, let's set it to 100, but later when you want to have two voices playing, you can adjust it to get a mix of the VX90 oscillator and S950 oscillator playing together.

{{< figure src="/wp-content/uploads/2021/02/img%5F1789.jpeg?w=1024" alt="" caption="" >}}

Next we'll move on to option E10 to adjust the VCF. I'd suggest setting this to 100 as well, just to make sure that the filter is wide open for our application, and doesn't interfere with our S950 program we'll be creating next.

{{< figure src="/wp-content/uploads/2021/02/img%5F1792.jpeg?w=1024" alt="" caption="" >}}

Similarly, I'll suggest editing E11 to make sure that there isn't any resonance for now that could cause us problems or confusion as we get started, so set the resonance to 00 for now.

{{< figure src="/wp-content/uploads/2021/02/img%5F1793.jpeg?w=1024" alt="" caption="" >}}

Next up, make sure your High Pass Filter is not impacting the sound by also setting it to 0. Again, this will be good to adjust once you're ready to make some sounds, but for now it could just make things confusing when processing the S950, so just set it to 00.

{{< figure src="/wp-content/uploads/2021/02/img%5F1813.jpeg?w=1024" alt="" caption="" >}}

The next two settings are for setting how the VX90 actually plays, and you can absolutely adjust these two settings as well, but setting them as directed for now will make sure that we have everything setup properly before we begin to experiment.

First up, let's have the VX90 be setup on Polyphonic mode, this ensures that when you play one note, it will play one oscillator from the VX90 and one oscillator from the S950. You can use DUAL or UNI later to stack the voices for a thicker sound, but the easiest way to test that everything is working properly is with POLY mode. So head over to E50 and set it to POLY.

{{< figure src="/wp-content/uploads/2021/02/img%5F1790.jpeg?w=1024" alt="" caption="" >}}

We need to make sure E51 is 00 to disable portamento.

{{< figure src="/wp-content/uploads/2021/02/img%5F1791.jpeg?w=1024" alt="" caption="" >}}

Last but certainly not least, we need to make sure we have the MIDI channel on the VX90 set to MIDI channel 1. Head over to E70 and set the MIDI CH to 01.

{{< figure src="/wp-content/uploads/2021/02/img%5F1814.jpeg?w=1024" alt="" caption="" >}}

Akai S950 Setup

With all those settings changed, we're ready to move over to the S950. Personally, I'd suggest an initial boot up without a disk, and we'll just use the default TONE PRGRM to make sure everything works. You'll have plenty of time to mess with samples later!

Also, if you want to try and skip all of the steps, I have provided a disk image at the end of this blog that is the TONE PRGRM that you will have created once you've completed all of the steps listed here.

{{< figure src="/wp-content/uploads/2021/02/img%5F1794.jpeg?w=1024" alt="" caption="" >}}

So first up, and this hung me up on my S950, we need to make sure that we have OMNI turned off, otherwise you're not going to be able to get Polyphonic sounds. The reason for this is because it the way we are going to setup the program it will play all eight S950 oscillators/samplers at the same time, consuming all of your polyphony. Which is almost certainly not what you want.

To disable OMNI, press the MIDI button to get into the MIDI menu, and on the first page you can arrow over to the Omni on/off, and press OFF on your PARAMETER KEY.

While you are here, also make sure that your Basic MIDI channel is set to 1. I imagine you can play with this some, but if you're following along with me, keep it at 1.

{{< figure src="/wp-content/uploads/2021/02/img%5F1806.jpeg?w=1024" alt="" caption="" >}}

Now, with our simple TONE PRGRM we have something to work with. We'll need to go to EDIT PRGRM in order to make sure we have six key groups that will respond to each separate MIDI event uniquely for each VX90 received key press.

Page down to the third page, and you should see that we currently only have one key group due to Select ( 0 to 1) indicating that we only have the one key group at this time.

{{< figure src="/wp-content/uploads/2021/02/img%5F1795.jpeg?w=1024" alt="" caption="" >}}

Arrow over to Copy(+) and press the ON/+ button five times so that you now have six key groups to work with.

{{< figure src="/wp-content/uploads/2021/02/img%5F1796.jpeg?w=1024" alt="" caption="" >}}

Now the next part is a little tedious, but I am going to post pictures for all of the settings to make sure that everything matches up.

Page down to page 16, and we will set the MIDI channel offset for each KG so that the MIDI ch. matches the key group. KG1 to MIDI ch. 1, KG2 to MIDI ch. 2, etc...

Don't worry, you're almost done and should be able to hear something shortly!

{{< figure src="/wp-content/uploads/2021/02/img%5F1807.jpeg?w=1024" alt="" caption="" >}}

{{< figure src="/wp-content/uploads/2021/02/img%5F1808-1.jpeg?w=1024" alt="" caption="" >}}

{{< figure src="/wp-content/uploads/2021/02/img%5F1809.jpeg?w=1024" alt="" caption="" >}}

{{< figure src="/wp-content/uploads/2021/02/img%5F1810.jpeg?w=1024" alt="" caption="" >}}

{{< figure src="/wp-content/uploads/2021/02/img%5F1811.jpeg?w=1024" alt="" caption="" >}}

{{< figure src="/wp-content/uploads/2021/02/img%5F1812.jpeg?w=1024" alt="" caption="" >}}

The last step is to now page down to page 17, so we can set the audio outputs. As we did for the MIDI channels, we now want the OUTPUTs to match the key groups. So KG1 is set to 1, KG2 is set to 2, KG3 is set to 3, etc...

{{< figure src="/wp-content/uploads/2021/02/img%5F1815.jpeg?w=1024" alt="" caption="" >}}

{{< figure src="/wp-content/uploads/2021/02/img%5F1816.jpeg?w=1024" alt="" caption="" >}}

{{< figure src="/wp-content/uploads/2021/02/img%5F1817.jpeg?w=1024" alt="" caption="" >}}

{{< figure src="/wp-content/uploads/2021/02/img%5F1818.jpeg?w=1024" alt="" caption="" >}}

{{< figure src="/wp-content/uploads/2021/02/img%5F1819.jpeg?w=1024" alt="" caption="" >}}

{{< figure src="/wp-content/uploads/2021/02/img%5F1820.jpeg?w=1024" alt="" caption="" >}}

Now, if everything is setup properly you \*should\* be able to hear some sounds! Start by playing a single note at a time, and play up and down the keyboard/pads of your controller. If you don't hear anything, the first thing I would suggest checking is that you have monitoring turned on your device.

Once you can hear a single note playing at the same time, try playing a chord to make sure that you can hear individual notes playing at the same time. This is where I had made a mistake by not having OMNI turned off on the S950, and as soon as I turned it off everything worked as expected.

If you've got a Gotek drive, or can write an .hfe file to disk, the file below has a default program pre-setup to work with the VX90 so you could skip the steps above.

[s950-settings-for-vx90-setup](/wp-content/uploads/2021/02/s950-settings-for-vx90-setup.zip) [Download](/wp-content/uploads/2021/02/s950-settings-for-vx90-setup.zip)

Conclusion

If you've got the hardware, I'd say that this is pretty fun to mess around with. On the other hand, if you're really considering dropping $1k or more for both the VX90 and the S950, I'd be pretty hard pressed to say that all of this is worth it. Both devices have a unique sound to them, and how they can operate with each other is even more unique, and likely rare to see the two together, but these old devices are something you'll need to also factor in if you're looking to repair, maintain, and keep working. All I am saying is that it is not a cheap investment, so just think about what you are getting in to.

For those of you who do have both devices though, definitely good luck putting it all together and I am sure you can record off some really cool sounds, key groups, and other things. I'm going to be experimenting and seeing what I can come up with, and will keep you guys posted on where it goes for sure.

Links

Links that had different and important information for putting this post together

Graph Paper - [Connecting the VX90 to the S950](https://blog.perkowitz.net/2013/08/26/connecting-the-akai-s950-and-vx-90/)

Graph Paper - [Akai Sampler and Synths](https://blog.perkowitz.net/2013/08/25/akai-samplers-and-synths/)

Gear Sluts - [How do people use the S950 in their setups?](https://www.gearslutz.com/board/electronic-music-instruments-and-electronic-music-production/922751-how-do-people-use-s950-their-set-ups-2.html)

Gear Sluts - [One stupid question about the S950! Help!](https://www.gearslutz.com/board/electronic-music-instruments-and-electronic-music-production/692468-one-stupid-question-about-s950-help.html)
