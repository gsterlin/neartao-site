---
_last_editor_used_jetpack: block-editor
_publicize_done_22315546: "1"
_publicize_done_22890294: "1"
_publicize_done_external:
  twitter:
    "23256661": https://twitter.com/NearTao/status/1465328688107606019
_publicize_job_id: "65915325331"
_thumbnail_id: "3587"
_wpas_done_23256661: "1"
_wpas_done_24391465: "1"
author: neartao
categories:
  - music-production
cover:
  alt: IMG_3271
  image: /wp-content/uploads/2021/11/img_3271.jpeg
date: "2021-11-29T14:35:54+00:00"
guid: https://neartao.wordpress.com/?p=3585
parent_post_id: null
post_id: "3585"
publicize_tumblr_url: http://.tumblr.com/post/669197596038938624
publicize_twitter_user: NearTao
tags:
  - roland-sp-404-mk2
timeline_notification: "1638196557"
title: Roland SP-404 mk2 Firmware 1.13 Bugs, Issues, Concerns, Oddities, and Feature Requests
url: /2021/11/29/roland-sp-404-mk2-firmware-1-13-bugs-issues-concerns-oddities-and-feature-requests/

---
These notes are all for SP 404 mk2 firmware 1.13.

Bugs

- In pattern mode there is a slight gap between the end of a pattern and the start back to 1.1.1.
- In pattern mode edit, you cannot adjust the start position of the pattern, only the end position.
- Exported samples do not contain the project they were from, just named “<bank 1-10> <pad> <sample name> Sample”.  The bank should be a-j to match naming, it should include the project, and there ought to be a way to name the sample.
- Exporting samples will overwrite whatever you have on the SD card without warning you that there is already a sample there.

Issues

- The pattern mode gap bug makes it difficult to sample a perfect loop with either resampling, or skip back.  The best option I have found is to double the length of the pattern and then resample or use skip back to work on the first half.
- You cannot record samples while playing a pattern.  As soon as you hit REC it wants to record into the pattern regardless of which screen you are in.
- I have not be able to figure out how to exit pattern record mode without stopping everything, which forces you to hard stop whatever you have playing.
- When you are in pattern record mode you cannot enable bus FX.
- EFX are a pain to edit, and require a bit of menu diving, there are only sixteen favorites that you need to menu dive to edit, and bypass.  I’m not sure why these aren’t part of the Bus FX to move around/through, but it is annoying.
- Probably a setting someplace, but every time I resample the sample gets quieter and requires a normalize to bring it back up to level.
- Once you resample your Bus FX are disabled, would be nice if there were a setting for the new sample to just not be routed through Bus FX instead of disabling the Bus FX.
- There is no way that I have found to change quantization on a pattern once you have recorded it… you need to rerecord it which is annoying.
- There is no Redo after undoing a pattern note entry.
- Chromatic does not work in pattern mode, forcing you to resample or use skip back to record a single note used chromatically.
- Chromatic mode does not support custom scales, so you’ll need to know which pads are for your scale and which ones not to use.
- Chromatic mode cannot be customized to play the notes that you want.
- Start/End does well, but could use a snap to 0.  For the moment I have been using Envelope with a attack of 1 and/or release of 1 to hide the pops and clicks as appropriate.
- Personally think this is a bug, but GATE does not honor a release setting, so you cannot have a gated note have a nice subtle tail.  This implementation may be intentional, but I think it is wrong.
- The controls on the FX are rather inconsistent, which I’m mostly okay with, but a fair number of them do not have Dry/Wet independent controls… so for example, you do not have a Reverb that can have a 100% wet, and 0% dry setting.  For Reverb, you just get level to control the amount of reverb, but no way to reduce the level of the dry signal… boo.

Concerns

- The Value knob gets used \*a lot\*, not sure how long it will last.  Hopefully a long time.
- You only get 10 mute groups per project.  I suspect that this will make things a bit more confusing if you are planning on using all of the banks, and don’t take good notes.  I’d prefer to see 16 mute groups, as having one per pad bank and a few spare would be super helpful.  Just remember to take notes on what is what folks.
- I’d like to see under record settings for resampling a way to create a perfect loop.  You can kind of wing this with pattern mode and just recording a longer sample and then retriggering the resampled sample in the pattern, but I think there’s a great opportunity here for making this a mini looper that doesn’t quite have a workflow it would need to do it.  Or I need to think outside of the box more.
- It would be nice if you could set the velocity for FIXED VELOCITY, instead of it always being max… I know you can use 16 VELOCITY… but then you’re bouncing between samples… so meh.
- Probably a setting for this already I need to dive into… but I’m finding resampling is always quieter than what I was playing, so I then need to normalize the sample again to get it back to the level that I want.  This might be the setting under GAIN Noise Gate (which is -12db for now)… need to experiment.
- Remain button doesn’t show you any information about the battery when powered… what’s the voltage left, time left, anything?
- Chop exporting samples to pads… I haven’t figured out to only export the chops that I want yet and ignore whatever else is there that I do not want.  It may be able to do this, but it definitely seems fiddly.
- No way to convert a sample from stereo to mono that I have found.  Would be nice to be able to do this.

Oddities

- It is just strange that there are 3 FX that are only present on INPUT SETTINGS. Auto Pitch, Vocoder, and Guitar Amp Sim are only available as INPUT FX Settings.  I could definitely see uses for them in the rest of the MFX, and my guess is they will show up there eventually.
- The online only manual sucks… why is there no freaking PDF?  Change my mind.

Feature Requests

- Add in the three INPUT FX into the other MFX… please.
- Have GATE use the ENVELOPE release setting to trail off the sample if the release is anything other than 0.
- Would love to have an FX to cancel center channel or only keep center channel.
- A way to name samples, even if you have to use the VALUE knob would be super handy… I’m old school and don’t mind doing the three letter GTR, PNO, BAS, shorts… and being able to add in note names into the sample would be helpful.  Heck… if it even output the assigned sample and BPM value in the name when you exported… \*chef’s kiss\*.
