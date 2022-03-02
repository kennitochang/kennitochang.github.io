---
layout: post
title: Annotating Text with Tone-Marked Jyutping
lang-ref: jytuping-tones-marks
---

_All views are my own._

I recently came across CanCLID's [Inject Jyutping](https://github.com/CanCLID/inject-jyutping) browser extension. The basic idea is to annotate Chinese characters with the associated Cantonese pronunciation in [jyutping](https://en.wikipedia.org/wiki/Jyutping), the _de facto_ standard romanization for Cantonese in academia and education devised by the Linguistic Society of Hong Kong. However, I unfortunately found it difficult to use due to an often-cited issue with Jyutping, which is that it uses numbers to represent tones, making it appear cluttered and sometimes difficult to interpret. 


One alternative to represent tones using tone marks, also known diacritics, small markings attached to existing Roman letters. This is the approach used by the [Vietnamese alphabet](https://en.wikipedia.org/wiki/Vietnamese_alphabet) and also to represent tones in Mandarin [pinyin](https://en.wikipedia.org/wiki/Pinyin). Tone marks have the benefit of condensing text and providing visual and mnemonic cues guiding the reader's pronunciation of words. These benefits are well-appreciated by users of both Vietnamese and pinyin.

As it stands, the Linguistic Society of Hong Kong (see [jyutping.org](https://jyutping.org)) is yet to release an official proposal for adding tone marks. In my current study of Cantonese, I have adopted a set of my own tone marks for personal use. I am certainly [not](https://www.reddit.com/r/Cantonese/comments/7r4y5b/random_idea_vietnamese_tone_marks) [the](http://www.cantonese.sheik.co.uk/phorum/read.php?1,127274,131154) [only](https://www.amazon.com/Cantonese-Everyone-English-Chinese/dp/9620718615) [person](https://www.facebook.com/CantoneseABC) to have done so. Here, I provide an example of how tone marks might be useful in a browser extension for annotating text. The system of tone marks I employed is not official by any means, and I hope that in publishing this extension I can help spur discussion around the possible introduction of tone marks to jyutping.

## Inject Jyutping with Diacritics

Based on CanCLID's browser extension, I created a new browser extension for jyutping annotation that uses the following system of tone marks:

| Tone Number | 1 | 2 | 3 | 4 | 5 | 6 |
|-------------|---|---|---|---|---|---|
| Description  | high level | high rising | mid level | low falling | low rising | low level |
| Example   | <span style="font-size:250%;">一</span> | <span style="font-size:250%;">碗</span> | <span style="font-size:250%;">半</span> | <span style="font-size:250%;">牛</span> | <span style="font-size:250%;">腩</span> | <span style="font-size:250%;">飯</span> |
| Jyutping   | jat1 | wun2 | bun | ngau4 | naam5 | faan6 |
| Jyutping with Diacritics  | jāt | wún | bun | ngàu | nǎam | fạan |
| Visualization   | ![](/assets/images/jat_tone.png) | ![](/assets/images/wun_tone.png) | ![](/assets/images/bun_tone.png) | ![](/assets/images/ngau_tone.png) | ![](/assets/images/naam_tone.png) | ![](/assets/images/faan_tone.png) |

The six tones of Cantonese can be remembered using the mnemonic 一碗半牛腩飯 (one and a half bowls of beef brisket rice).


At a small cost in terms of the ability to distinguish tones visually, tone-marked jyutping reduces the amount of clutter and space between annotated Chinese characters. It provides a more compact reading experience for learning Cantonese and/or jyutping.

| ![A poem annotated with numbered jyutping.](/assets/images/jyutping-number-annotation.png) | ![A poem annotated with marked jyutping.](/assets/images/jyutping-tonemark-annotation.png) |
|-|-|
| | |

The tone marks were chosen based on analogy with Hanyu Pinyin, Vietnamese, and Yale romanization, with an eye towards Unicode support. For a further explanation of Cantonese tones, see [here](https://jyutping.org/docs/tone/). In future versions of the browser extension, I hope to allow users to select their own tone marks if they wish.

## Download Link
- [Download for Firefox](https://addons.mozilla.org/en-US/firefox/addon/inject-jyutping-diacritics/)
- Download for Chrome (pending review)
