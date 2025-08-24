---
_last_editor_used_jetpack: block-editor
_oembed_4a0023e18f5e443fd04da48daebdd89a: <div class="embed-youtube"><iframe title="SP404 mk2 Guide and Office Hours" width="750" height="422" src="https://www.youtube.com/embed/c_JQWYbgOWc?feature=oembed" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></div>
_oembed_82ed1e73148cc246eedb848006072bd9: <div class="embed-youtube"><iframe title="SP404 mk2 Guide and Office Hours" width="750" height="422" src="https://www.youtube.com/embed/ofDXDEQbozM?feature=oembed" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></div>
_oembed_a0fa8b3f90925b1811f6487104fdd212: <div class="embed-youtube"><iframe title="SP404 mk2 Guide and Office Hours" width="500" height="281" src="https://www.youtube.com/embed/ofDXDEQbozM?feature=oembed" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe></div>
_oembed_a5a29fce0d808287e1b7560a4678431e: <div class="embed-youtube"><iframe title="SP404 mk2 Guide and Office Hours" width="500" height="281" src="https://www.youtube.com/embed/c_JQWYbgOWc?feature=oembed" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe></div>
_oembed_b639b2ce6e87aa2fc19743239104494a: <div class="embed-youtube"><iframe title="SP404 mk2 Guide and Office Hours" width="500" height="281" src="https://www.youtube.com/embed/ofDXDEQbozM?feature=oembed" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></div>
_oembed_cd3bc8dc29c464196a614887bda2d885: <div class="embed-youtube"><iframe title="SP404 mk2 Guide and Office Hours" width="580" height="326" src="https://www.youtube.com/embed/ofDXDEQbozM?feature=oembed" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe></div>
_oembed_d5b4930451b4f4f67c00a089c90595dd: <div class="embed-youtube"><iframe title="SP404 mk2 Guide and Office Hours" width="500" height="281" src="https://www.youtube.com/embed/c_JQWYbgOWc?feature=oembed" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></div>
_oembed_ead548adadd2fa39103755f2c37b82d7: <div class="embed-youtube"><iframe title="SP404 mk2 Guide and Office Hours" width="580" height="326" src="https://www.youtube.com/embed/c_JQWYbgOWc?feature=oembed" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe></div>
_oembed_time_4a0023e18f5e443fd04da48daebdd89a: "1727692487"
_oembed_time_82ed1e73148cc246eedb848006072bd9: "1727692484"
_oembed_time_a0fa8b3f90925b1811f6487104fdd212: "1678305721"
_oembed_time_a5a29fce0d808287e1b7560a4678431e: "1678305722"
_oembed_time_b639b2ce6e87aa2fc19743239104494a: "1711607771"
_oembed_time_cd3bc8dc29c464196a614887bda2d885: "1678305720"
_oembed_time_d5b4930451b4f4f67c00a089c90595dd: "1711607771"
_oembed_time_ead548adadd2fa39103755f2c37b82d7: "1678305720"
_publicize_done_22315546: "1"
_publicize_done_external:
  twitter:
    "23256661": https://twitter.com/NearTao/status/1633558714740543488
_publicize_job_id: "82141560372"
_wpas_done_23256661: "1"
author: neartao
categories:
  - uncategorized
date: "2023-03-08T20:01:58+00:00"
guid: https://neartao.wordpress.com/?p=3856
parent_post_id: null
post_id: "3856"
publicize_twitter_user: NearTao
timeline_notification: "1678305720"
title: SP404 mk2 Polyphony
url: /2023/03/08/sp404-mk2-polyphony/
wordads_ufa: s:wpcom-ufa-v3-beta:1678305863

---
Well... I finally decided to get back to working on the guide again... and I'm giving a try streaming a bit of the process while also trying to solve some problems. Here are two streams that probably should have been one, but I just need to get used to having a bit of dead air or something.

## Stereo Samples Panned Mono Left

The first video shows the creation of a pattern using stereo samples, and I pan them left. We do not get to 32 pads playing, as the first 16 pads are still playing in stereo using up all 32 notes of polyphony.

https://youtube.com/live/ofDXDEQbozM?feature=share

## Mono Samples

The second video shows the creation of a pattern using mono samples, and playing them actually allows all 32 pads to play, which is great!

https://youtube.com/live/c\_JQWYbgOWc?feature=share

## Conclusion

For now it seems pretty clear that if you are solely sampling or resampling on the mk2, you are going to be stuck with 16 notes of stereo polyphony, wether you are sampling in mono or stereo, they come in as stereo samples, and will use 2 notes of polyphony regardless of how you pan them.  It’s not the end of the world, but it can be a bit restrictive, and indicates that Roland really should add some stereo to mono option, likely in the **\|START/END\|** menu, sometime in the future (post 2.01).

If you really need 32 notes of polyphony, you’ll have to use the Roland mk2 application, or use your computer to convert/load samples onto your SD Card and make sure that they are mono.  Right now, those are your two options.

## Resources

If you'd like to get the test project I put together, feel free to download it and play around.

[PROJECT\_13](/wp-content/uploads/2023/03/project_13.zip) [Download](/wp-content/uploads/2023/03/project_13.zip)
