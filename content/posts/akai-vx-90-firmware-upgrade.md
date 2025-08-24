---
_last_editor_used_jetpack: block-editor
_publicize_done_22315546: "1"
_publicize_done_22890294: "1"
_publicize_done_external:
  twitter:
    "23256661": https://twitter.com/NearTao/status/1359984026694656003
_publicize_job_id: "54647492036"
_thumbnail_id: "2173"
_wpas_done_23256661: "1"
_wpas_done_24391465: "1"
author: neartao
categories:
  - music-production
cover:
  alt: img_1741
  image: /wp-content/uploads/2021/02/img_1741.jpeg
date: "2021-02-11T21:53:49+00:00"
guid: https://neartao.wordpress.com/?p=2171
parent_post_id: null
post_id: "2171"
publicize_tumblr_url: http://.tumblr.com/post/642861430054535168
publicize_twitter_user: NearTao
tags:
  - akai-vx-90
  - tauntek-custom-firmware
timeline_notification: "1613080432"
title: Akai VX 90 - Tauntek Firmware Upgrade
url: /2021/02/11/akai-vx-90-firmware-upgrade/

---
I've been looking off and on for an Akai VX 90, and finally found one. Probably paid too much, but wanted to hook one up to my Akai S950, so there will be that, once I get the cable in.

I've spent the last couple of days just playing around with it, reading the manual, and trying to get my brain around how it works. As you can see from the featured image, the interface is a bit sparse, and not a whole lot of direction as to what is going on.

{{< figure src="/wp-content/uploads/2021/02/img%5F1741-1.jpeg?w=1024" alt="" caption="" >}}

Above, you can see that unlike the Akai S950, there's not much in the way of knobs, and if you want to edit anything you're going to have to be using the number pad or value slider a lot. Or do you? In my research on the Akai VX 90 I did find some smart people working on a customer firmware for the device the device in forum posts, but it was hard to tell if the work was done for the Akai VX 90, the AX 60, AX 73, or something else. Well... with a little poking and searching on eBay, I was able to find something that NESYNTH was selling on [eBay](https://www.ebay.com/itm/TAUNTEK-OS-ROM-Compatible-with-Akai-VX90-and-Akai-AX73-Upgrade-EPROM-ROM-chip/164276942244?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649) that was created by [Tauntek](http://www.tauntek.com), and it just showed up today. I took some pictures and figured I'd try and give a high level overview of how to upgrade the firmware yourself if you happened to want to try. If you're looking for what was documented check out the page [A firmware update for the AKAI AX73 Synthesizer](http://www.tauntek.com/AX73.htm).

Before I get into the upgrade itself, the firmware opens up the option to using MIDI CC to assign your own controls to different parameters so that you can make changes with knobs, sliders, and buttons. This will definitely be much easier, and I figured it may also lead to some interesting control voltage to MIDI CC opportunities. It also allows for SYSEX dump backups, which I'll also be looking into once I get settled in how the VX 90 works.

{{< figure src="/wp-content/uploads/2021/02/img%5F1739.jpeg?w=1024" alt="" caption="" >}}

As is the style for other Akai systems of this time, you probably just need to remove two screws on each side, and one on the back in order to get the case off. The rack ears were included, but removed when shipped, and I currently have no reason to put them back on. In another month or two I am sure that will change, but for the time being they will remain off.

Before you get started, don't forget to unplug the VX 90. These systems can hold an incredible amount of charge and just pass the power on to you. Don't want to electrocute yourself, and you don't want to accidentally fry anything fragile here. Always remember to ground yourself, and it is not a bad habit to get into to just touch the metal on the case to help discharge any shocks you may have built up yourself.

{{< figure src="/wp-content/uploads/2021/02/img%5F1740.jpeg?w=1024" alt="" caption="" >}}

Once you get the top off, you'll see the guts of the synth. There isn't too much going on with the boards really. The left side is mostly power and regulators, so nothing too fancy, the lower right board appears to be the 6 chips that provide the VCO voices and the upper right is two boards, the one on top that is brown is your audio output interface, and the lower board has the MIDI and (covered) the firmware that you'll be replacing if you're going to do this job.

{{< figure src="/wp-content/uploads/2021/02/img%5F1742.jpeg?w=1024" alt="" caption="" >}}

I took the picture above to show where the firmware actually sits. It's not hard to get at, but you can see that you'll need to take the top board off so that you can get at it and be able to replace it.

{{< figure src="/wp-content/uploads/2021/02/img%5F1744.jpeg?w=1024" alt="" caption="" >}}

In the picture above, you can see I removed to screws, one on the middle back of the board, and one on the bottom middle of the board. You only need to remove the one on the bottom, and then the two black screws on the outside of the case that hold up the audio output for the board. The upper screw that I removed helps hold the PCB to the metal bracket on the audio out section (or at least I am pretty sure), and seems be unnecessary to remove.

{{< figure src="/wp-content/uploads/2021/02/img%5F1745.jpeg?w=1024" alt="" caption="" >}}

From here you can just flip the board over without having to remove all the cables and jacks, it's a little bit tight and in the way, but doesn't require having to pull the whole thing apart. One that is out of the way you can remove that metal mounting bracket that is covering the firmware.

{{< figure src="/wp-content/uploads/2021/02/img%5F1746.jpeg?w=1024" alt="" caption="" >}}

Now, for those of you that don't know, look closely at the chip here. First it's labelled Akai AX 73 v1.2A... so yeah, this is literally the same system as the AX 73, just repackaged inside of the VX 90 rack mount. Second though, what I wanted to point out is you can see a notch in the white outline for the chip, this is showing you which direction the notch on your firmware should be when you install it. There is a tiny notch there on top if you look closely. Absolutely make sure that you line this up properly or you're going to fry the chip. This old hardware definitely doesn't have circuits to protect from putting chips in incorrectly, and it will result in burnt out chips and can negatively impact other components. Be careful, cautious, and don't be afraid to double or triple check as you make these changes.

{{< figure src="/wp-content/uploads/2021/02/img%5F1747.jpeg?w=1024" alt="" caption="" >}}

Here's a picture of the replacement chip, still in the STATIC packaging to help protect it from shock. Again, electrical components are fragile... make sure you are grounded properly. Touch the side of your case before handling components.

{{< figure src="/wp-content/uploads/2021/02/img%5F1748.jpeg?w=1024" alt="" caption="" >}}

The picture above is just me checking to make sure the notches lined up the way I thought, and checking that it has the right number of pins. No sense going further unless it all looks right, which it does.

To get the firmware out, I just took my time with my Swiss army knife, using a flat bottle opener to slowly wiggle it out a little bit on each end at a time. You want to do this slowly and rather carefully because you don't want to bend the pins. (NOTE: I did bend a couple pins a little, and was very careful to realign them properly in case I need to go back to the original firmware for any reason).

{{< figure src="/wp-content/uploads/2021/02/img%5F1750.jpeg?w=768" alt="" caption="" >}}

Above it me checking the alignment of the chip before I pushed it in. I took my time to make sure that the legs were all lined up and going to go into the IC socket. The first couple of times attempting to line it up they were on the outside of the socket, so again, just take your time and line it up. You really shouldn't have to bend any of the pins, but do keep in mind that they may be out of alignment. Once you're ready to push the chip in you want to apply a small amount of pressure across the top on both some so that it sets in straight and flat. This is the best way to make sure the pins don't bend, and get a solid connection with the socket.

{{< figure src="/wp-content/uploads/2021/02/img%5F1752.jpeg?w=1024" alt="" caption="" >}}

Here's a picture of putting the whole shebang back together.

{{< figure src="/wp-content/uploads/2021/02/img%5F1755.jpeg?w=1024" alt="" caption="" >}}

Everything back together and powered on! Display actually has a valid output... woot!

So yeah... for now I'll be using the headphone jack because there's no (well not much) noise there... I can at least make some sounds off of it and not getting a ground hum like I am off of the L/R outputs.

Gotta figure out what to tackle next, but it is nice to be able to use the q-links to modify CC parameters, will provide details on that next :D
