![Header Image](https://raw.github.com/letydoesstuff/mastodon-nobird-emoji/main/images/header.jpg)

# Mastodon with Nobird Emoji

Replace all dead bird site Twemoji on your Mastodon instance with [Noto Emoji](https://github.com/googlefonts/noto-emoji)!

### A Timeline

- On 2017 September 17th, Mastodon adopted [Twemoji](https://github.com/twitter/twemoji), Twitter's open-source emoji library, to render all emoji in their native web client.<sup>[1](https://github.com/mastodon/mastodon/commit/846cd4e8381c891816cf814582304b534db4ee5f)</sup>
- On 2022 October 27th, Elon Musk bought Twitter. <sup>[2](https://www.latimes.com/business/story/2022-10-27/elon-musk-buys-twitter-44-billion)</sup>
- On 2022 November 4th, Elon Musk started laying off bunch of Twitter staff.<sup>[3](https://www.latimes.com/entertainment-arts/story/2022-11-04/twitter-layoffs-employee-tweets-elon-musk)</sup>
- On 2022 November 17th, Jason Sofonia, the designer of Twemoji, departed Twitter.<sup>[4](https://github.com/twitter/twemoji/issues/570#issuecomment-1352347394)</sup>
- On 2023 June 23rd, Elon Musk stopped updating the Twemoji repo with new emoji.<sup>[5](https://github.com/jdecked/twemoji/issues/8#issuecomment-1588997510)</sup>
- On 2023 September 5th, I decided I don't HECKIN' want Elon Musk's dumb emoji on Mastodon anyways.

### And Here We Are Now

It's just trading in one set of corpo artwork for another, but I'm happy to kick as many of those off my hardware as possible, and FOSS is FOSS at the end of the day.

Besides, Noto's cuter and now custom emoji I import from Google's [Emoji Kitchen](https://emoji.supply/kitchen) match the unicode emoji on my instance.

## FAQ

### Why did all the Noto Emoji disappear after I upgraded my Mastodon instance?

Upgrading your instance might have overwritten your modified `emoji` folder with Mastodon's stock images. Just rerun the Nobird Emoji install instructions for your Mastodon version, and they'll be back!

### Why do I still see Twemoji instead of Noto Emoji after restarting Mastodon?

Caching issues, probably. Try hard-refreshing your browser, clearing cache storage from your site data in browser settings, or purging cache further upstream if you're using a CDN like Cloudflare? Or just be patient and wait for cache to expire.

### Why don't some emoji look right?

Still caching issues, probably. But if you've already read through the stuff I wrote about that, it might be because you're talking about one of the emoji in the table below.

Twemoji included some emoji that Noto Emoji doesn't support, but I still needed to fill in those spots in Mastodon's files. Most of the missing files are just variations of profession and role emojis, so I just had those fall back to its generic Simpsons form. That said, it seems there was some tofu in Google's no tofu font after all.

| Missing from Noto Emoji | Replaced With |
|----|----|
| 🕴🏻‍♀️ Woman in Suit Levitating: Light Skin Tone<br>`U+1F574 U+1F3FB U+200D U+2640 U+FE0F` | 🕴🏻 Person in Suit Levitating: Light Skin Tone<br>`U+1F574 U+1F3FB` |
| 🕴🏻‍♂️ Man in Suit Levitating: Light Skin Tone<br>`U+1F574 U+1F3FB U+200D U+2642 U+FE0F` | 🕴🏻 Person in Suit Levitating: Light Skin Tone<br>`U+1F574 U+1F3FB` |
| 🕴🏼‍♀️ Woman in Suit Levitating: Medium-Light Skin Tone<br>`U+1F574 U+1F3FC U+200D U+2640 U+FE0F` | 🕴🏼 Person in Suit Levitating: Medium-Light Skin Tone<br>`U+1F574 U+1F3FC` |
| 🕴🏼‍♂️ Man in Suit Levitating: Medium-Light Skin Tone<br>`U+1F574 U+1F3FC U+200D U+2642 U+FE0F` | 🕴🏼 Person in Suit Levitating: Medium-Light Skin Tone<br>`U+1F574 U+1F3FC` |
| 🕴🏽‍♀️ Woman in Suit Levitating: Medium Skin Tone<br>`U+1F574 U+1F3FD U+200D U+2640 U+FE0F` | 🕴🏽 Person in Suit Levitating: Medium Skin Tone<br>`U+1F574 U+1F3FD` |
| 🕴🏽‍♂️ Man in Suit Levitating: Medium Skin Tone<br>`U+1F574 U+1F3FD U+200D U+2642 U+FE0F` | 🕴🏽 Person in Suit Levitating: Medium Skin Tone<br>`U+1F574 U+1F3FD` |
| 🕴🏾‍♀️ Woman in Suit Levitating: Medium-Dark Skin Tone<br>`U+1F574 U+1F3FE U+200D U+2640 U+FE0F` | 🕴🏾 Person in Suit Levitating: Medium-Dark Skin Tone<br>`U+1F574 U+1F3FE` |
| 🕴🏾‍♂️ Man in Suit Levitating: Medium-Dark Skin Tone<br>`U+1F574 U+1F3FE U+200D U+2642 U+FE0F` | 🕴🏾 Person in Suit Levitating: Medium-Dark Skin Tone<br>`U+1F574 U+1F3FE` |
| 🕴🏿‍♀️ Woman in Suit Levitating: Dark Skin Tone<br>`U+1F574 U+1F3FF U+200D U+2640 U+FE0F` | 🕴🏿 Person in Suit Levitating: Dark Skin Tone<br>`U+1F574 U+1F3FF` |
| 🕴🏿‍♂️ Man in Suit Levitating: Dark Skin Tone<br>`U+1F574 U+1F3FF U+200D U+2642 U+FE0F` | 🕴🏿 Person in Suit Levitating: Dark Skin Tone<br>`U+1F574 U+1F3FF` |
| 🕴️‍♀️ Woman in Suit Levitating<br>`U+1F574 U+FE0F U+200D U+2640 U+FE0F` | 🕴️ Person in Suit Levitating<br>`U+1F574 U+FE0F` |
| 🕴️‍♂️ Man in Suit Levitating<br>`U+1F574 U+FE0F U+200D U+2642 U+FE0F` | 🕴️ Person in Suit Levitating<br>`U+1F574 U+FE0F` |
| ⛷🏻 Skier, Type-1-2<br>`U+26F7 U+1F3FB` | ⛷️ Skier<br>`U+26F7 U+FE0F` |
| ⛷🏼 Skier, Type-3<br>`U+26F7 U+1F3FC` | ⛷️ Skier<br>`U+26F7 U+FE0F` |
| ⛷🏽 Skier, Type-4<br>`U+26F7 U+1F3FD` | ⛷️ Skier<br>`U+26F7 U+FE0F` |
| ⛷🏾 Skier, Type-5<br>`U+26F7 U+1F3FE` | ⛷️ Skier<br>`U+26F7 U+FE0F` |
| ⛷🏿 Skier, Type-6<br>`U+26F7 U+1F3FF` | ⛷️ Skier<br>`U+26F7 U+FE0F` |
|  Shibuya<br>`U+E50A` | Tofu<br>Modified from 🧈 Butter (`U+1F9C8`) |

If the emoji you're talking about aren't in that table, they're probably from [Unicode 15](https://emojipedia.org/emoji-15.0). 

Mastodon only supports emoji up to Unicode 14, so stuff that came out after won't render quite the same in their web client. Your browser will fall back to your system emoji font, and depending on the device you're using, you might see emoji in a different style or just tofu (􏿿 <- that's what this thing is called) in their place.

### Can you add support for Unicode 15 emoji?

No, [that's hard](https://github.com/mastodon/mastodon/discussions/23841).

### Can you make Nobird Emoji work with a different emoji library?

No, I'm lazy. Feel free to fork this though.

## Licenses and Attributions

Most images from Google's Noto Emoji are licensed under [Apache License, Version 2.0](https://github.com/googlefonts/noto-emoji/blob/main/LICENSE), minus the region flags and stuff cause those are [public domain](https://github.com/googlefonts/noto-emoji/blob/main/third_party/region-flags/LICENSE).

And a special thanks to [@iamcal](https://github.com/iamcal)'s [emoji-data](https://github.com/iamcal/emoji-data/tree/v15.0.1) for saving me from spending a dumb amount of time working out how to script photoshop to build an emoji spritesheet.