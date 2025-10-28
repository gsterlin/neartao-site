---
_last_editor_used_jetpack: block-editor
_oembed_72bfc6652973944b36fbba4f860cbc32: <div class="embed-soundcloud"><iframe title="Big Hammer by NearTao" width="500" height="400" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?visual=true&url=https%3A%2F%2Fapi.soundcloud.com%2Ftracks%2F1022865028&show_artwork=true&maxwidth=500&maxheight=750&dnt=1"></iframe></div>
_oembed_time_72bfc6652973944b36fbba4f860cbc32: "1617657265"
_publicize_done_22315546: "1"
_publicize_done_22890294: "1"
_publicize_done_external:
  twitter:
    "23256661": https://twitter.com/NearTao/status/1378868599121702912
_publicize_job_id: "56781242193"
_thumbnail_id: "2523"
_wpas_done_23256661: "1"
_wpas_done_24391465: "1"
author: neartao
categories:
  - binding-of-isaac
  - gaming
cover:
  alt: Screen Shot 2021-04-03 at 3.48.47 PM
  image: /wp-content/uploads/2021/04/screen-shot-2021-04-03-at-3.48.47-pm.png
date: "2021-04-05T00:34:22+00:00"
guid: https://neartao.com/?p=2520
parent_post_id: null
post_id: "2520"
publicize_tumblr_url: http://.tumblr.com/post/647582574736244736
publicize_twitter_user: NearTao
timeline_notification: "1617582867"
title: 'Running "The Binding of Isaac: Repentance" natively on Intel based Apple Hardware'
url: /2021/04/04/running-the-binding-of-isaac-repentance-natively-on-intel-based-apple-hardware/

---
Alright folks... normally I don't get into video games on this site, but since Repentance is not going to be supported on Intel based Apple hardware... well I figured I'd write up a tutorial to get you going.

For this "how to", you'll need to get Crossover for your Mac. Personally, I bought the $59.95 for one year support. Heck, I used to use this product to play games ten or so years ago, so I'm a bit familiar with it still. I had lapsed from using it because I had been using Bootcamp so much, but I have subsequently stopped upgrading my Parallels VM, and honestly, games run pretty poorly through Virtual Machines, and I didn't want to be booting into bootcamp to play games.

So... I crossed my fingers, and so far have had plenty of success! Also, I think you can get a 14 day trial license, so you don't necessarily have to pay money out of the gate. For those of you with M1 processors, I don't think this will work due to how WINE works, so if you wanted to give it a try I suppose you can, but I'd be shocked if you didn't need some form of QEMU or other processor emulation as well to get anything to work.

If you're going to follow along, you're going to need to either use a trial license or purchase a license one way or another for Crossover. Codeweavers makes this supported product, and you can pick it up at [https://www.codeweavers.com](https://www.codeweavers.com). Once you've purchased your license, you'll be able to download the software. Personally, the lifetime license seems a bit excessive at nearly $500, especially for Mac users who I figure are not going to have much need for this product once they move over to the M1 and beyond based products. Buyer beware? For me, while I use Linux a lot, it hasn't really been a primary gaming system for me.

Installing CrossOver

Once you've got the file downloaded, go ahead and install it. Personally, I just unpacked the file and copied the application to my Applications folder. Once copied, I opened it up and then added the license through the prompt by logging into my CodeWeavers account. Again, if you're just going to check out the trial, then feel free to put it into trial mode. Unfortunately I didn't capture any screenshots for these steps, but it should be pretty self explanatory.

Install Windows Application

The main trick of CrossOver is simulating a Windows environment so that your programs can make API calls out and have CrossOver handle them. So to get CrossOver to do it's magic we're going to tell it to install a Windows application along with all the components necessary to actually run it.

{{< figure src="/wp-content/uploads/2021/04/screen-shot-2021-04-03-at-3.48.47-pm-1.png?w=1024" alt="" caption="" >}}

Go ahead and click "Install a Windows Application" to get started. You'll then be brought to the screen below to select an application. I just typed in Steam and then selected the dropdown "Steam" from the list.

{{< figure src="/wp-content/uploads/2021/04/screen-shot-2021-04-03-at-3.49.00-pm.png?w=1024" alt="" caption="" >}}

This should then bring you to a screen that gives you some information about the application.

{{< figure src="/wp-content/uploads/2021/04/screen-shot-2021-04-03-at-3.49.13-pm.png?w=1024" alt="" caption="" >}}

Once you believe you are ready to move forward, just click Continue on the bottom right of the window.

{{< figure src="/wp-content/uploads/2021/04/screen-shot-2021-04-03-at-3.49.29-pm.png?w=1024" alt="" caption="" >}}

You're now going to see something like the image above. This is showing you all of the additional content that needs to be installed in order to support Steam so that it can run on your Mac. There are going to be a few pop ups that you'll need to select "continue" or otherwise approve licenses in order to install.

{{< figure src="/wp-content/uploads/2021/04/screen-shot-2021-04-03-at-3.49.41-pm.png?w=760" alt="" caption="" >}}

For example, above you can see that I needed to say "Yes" to accept the Verdana font installation.

{{< figure src="/wp-content/uploads/2021/04/screen-shot-2021-04-03-at-3.50.09-pm.png?w=1024" alt="" caption="" >}}

Similarly I needed to go through the Microsoft XML Parser Setup Wizard to get this content installed inside the bottle for Steam.

{{< figure src="/wp-content/uploads/2021/04/screen-shot-2021-04-03-at-3.50.26-pm.png?w=1024" alt="" caption="" >}}

Again, assuming you accept the EULA, go ahead and accept it, it is necessary to run Steam. I might have missed a license screen or two, but hopefully you get the idea. I just wanted to make sure you it is clear that this is normal behavior of the CrossOver and Steam installation process.

Installing Steam

If you've installed Steam before, all of these dialogues will look familiar. If you're ready to install Steam just hit Next.

{{< figure src="/wp-content/uploads/2021/04/screen-shot-2021-04-03-at-3.50.46-pm.png?w=994" alt="" caption="" >}}

This will lead you to an Updating Steam dialogue box that shows you that it is downloading updates.

{{< figure src="/wp-content/uploads/2021/04/screen-shot-2021-04-03-at-3.51.03-pm.png?w=790" alt="" caption="" >}}

When it is done, CrossOver will let you know that the Steam installation is complete.

{{< figure src="/wp-content/uploads/2021/04/screen-shot-2021-04-03-at-3.51.17-pm.png?w=1024" alt="" caption="" >}}

Running Steam

You should now see a screen similar to what I captured below. This is showing you the applications that you have installed in the Steam bottle. Go ahead and double click on Steam to start it.

{{< figure src="/wp-content/uploads/2021/04/screen-shot-2021-04-04-at-8.25.45-pm.png?w=1024" alt="" caption="" >}}

You'll be presented with a screen to either log into an existing account, or create a new account. Either way, get yourself logged in.

{{< figure src="/wp-content/uploads/2021/04/screen-shot-2021-04-03-at-3.51.46-pm.png?w=858" alt="" caption="" >}}

Now you're probably going to see a screen that looks something like below. It looks like you have no games, and when you go to Library you'll likewise see nothing. I believe that this has been a common and longstanding issue with Steam running through CrossOver for a while now, but I'm not quite sure for how long that it has been an issue.

{{< figure src="/wp-content/uploads/2021/04/screen-shot-2021-04-03-at-3.52.49-pm.png?w=1024" alt="" caption="" >}}

I tried increasing my window size in an attempt to resolve this. But that didn't help, the rendering section was still black. To resolve this I tried tweaking a few settings in CrossOver, but none of them ultimately helped. Instead what I did was to go to View and then select "Small Mode" from the dropdown, and suddenly I could see all of my games again. I'm not sure of a workflow to purchase games through the Steam app, but you can certainly purchase them through the webpage if necessary.

{{< figure src="/wp-content/uploads/2021/04/screen-shot-2021-04-03-at-4.01.04-pm.png?w=465" alt="" caption="" >}}

Here you can see I have the option to "Install Game", and assuming you have it in your library, go ahead and install it. Once it is installed, you can double click on the icon in order to start the game.

{{< figure src="/wp-content/uploads/2021/04/screen-shot-2021-04-03-at-4.01.16-pm.png?w=473" alt="" caption="" >}}

Below you can see here is my first game getting it running on Mac!

{{< figure src="/wp-content/uploads/2021/04/screen-shot-2021-04-03-at-4.04.06-pm.png?w=1024" alt="" caption="" >}}

Conclussion

I'm sure there are other ways to get Repentance to work on a Mac, but I wanted to write this up for anybody who might be excited to play the game, but isn't exactly enthused that Mac is no longer supported. For you, I hold my glass up high, and hope you're able to get some joy out of the game!
