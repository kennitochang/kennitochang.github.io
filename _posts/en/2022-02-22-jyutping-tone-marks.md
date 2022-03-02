---
layout: post
title: Annotating Text with Tone-Marked Jyutping
lang-ref: jytuping-tones-marks
---

_All views are my own._

I recently came across CanCLID's [Inject Jyutping](https://github.com/CanCLID/inject-jyutping) browser extension, which annotates Chinese characters with the associated Cantonese pronunciation in [jyutping](https://en.wikipedia.org/wiki/Jyutping), the _de facto_ standard romanization for Cantonese in academia and education. However, I found the extension hard to use due to a much-debated feature of Jyutping, which is that it uses numbers to represent tones. In this case, the numbers made annotations appear cluttered. 

One alternative to numbered tones is representing tones using tone marks (aka diacritics) as in [Vietnamese](https://en.wikipedia.org/wiki/Vietnamese_alphabet) and Mandarin Chinese [pinyin](https://en.wikipedia.org/wiki/Pinyin). Tone marks have the benefit of producing more condensed text and providing visual and mnemonic cues guiding the reader's pronunciation of words. These benefits are well-appreciated by users of both Vietnamese and pinyin.

As it stands, the Linguistic Society of Hong Kong (see [jyutping.org](https://jyutping.org)) is yet to release an official proposal for adding tone marks. Up until now, I have been using my own system of tone marks to study Cantonese. I am certainly [not](https://www.reddit.com/r/Cantonese/comments/7r4y5b/random_idea_vietnamese_tone_marks) [the](http://www.cantonese.sheik.co.uk/phorum/read.php?1,127274,131154) [only](https://www.amazon.com/Cantonese-Everyone-English-Chinese/dp/9620718615) [person](https://www.facebook.com/CantoneseABC) to have done so.

Ultimately, I believe adding tone marks to the jyutping standard could be widely beneficial. When it comes to directly annotating text, as I discuss below, tone-marked jyutping has signifcant advantages over regular, numeric jyutping. The system of tone marks I employ is my own creation, although that isn’t the main focus here — I hope that in publishing this extension I can help spur discussion around the future introduction of tone marks to jyutping.

The six tones of Cantonese can be remembered using the mnemonic 一碗半牛腩飯 (one and a half bowls of beef brisket rice). For practice distinguishing the six tones, see [here](https://jyutping.org/en/docs/tone/).

## Inject Jyutping with Diacritics

Based on CanCLID's browser extension, I created a new browser extension for jyutping annotation that uses the following system of tone marks:

| Tone Number | 1 | 2 | 3 | 4 | 5 | 6 |
|-------------|---|---|---|---|---|---|
| Description  | high level | high rising | mid level | low falling | low rising | low level |
| Example   | <span style="font-size:250%;">一</span> | <span style="font-size:250%;">碗</span> | <span style="font-size:250%;">半</span> | <span style="font-size:250%;">牛</span> | <span style="font-size:250%;">腩</span> | <span style="font-size:250%;">飯</span> |
| Jyutping   | jat1 | wun2 | bun | ngau4 | naam5 | faan6 |
| Jyutping with Diacritics  | jāt | wún | bun | ngàu | nǎam | fạan |
| Visualization   | ![](/assets/images/jat_tone.png) | ![](/assets/images/wun_tone.png) | ![](/assets/images/bun_tone.png) | ![](/assets/images/ngau_tone.png) | ![](/assets/images/naam_tone.png) | ![](/assets/images/faan_tone.png) |

I chose the tone marks above based on analogy with Hanyu Pinyin, Vietnamese, and Yale romanization, with an eye towards Unicode support. In future versions of the browser extension, I hope to allow users to select their own tone marks if they wish.

At a small cost in terms of the ability to distinguish tones visually, tone-marked jyutping reduces the amount of clutter and space between annotated Chinese characters. It provides a more compact reading experience for studying Cantonese and/or jyutping.

### Example of annotation using tone-marked jyutping
<p><ruby class="inject-jyutping">人<rp>(</rp><rt lang="yue-Latn">jàn</rt><rp>)</rp></ruby><ruby class="inject-jyutping">人<rp>(</rp><rt lang="yue-Latn">jàn</rt><rp>)</rp></ruby><ruby class="inject-jyutping">生<rp>(</rp><rt lang="yue-Latn">sāang</rt><rp>)</rp></ruby><ruby class="inject-jyutping">出<rp>(</rp><rt lang="yue-Latn">cēot</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嚟<rp>(</rp><rt lang="yue-Latn">lài</rt><rp>)</rp></ruby><ruby class="inject-jyutping">就<rp>(</rp><rt lang="yue-Latn">zạu</rt><rp>)</rp></ruby><ruby class="inject-jyutping">係<rp>(</rp><rt lang="yue-Latn">hại</rt><rp>)</rp></ruby><ruby class="inject-jyutping">自<rp>(</rp><rt lang="yue-Latn">zị</rt><rp>)</rp></ruby><ruby class="inject-jyutping">由<rp>(</rp><rt lang="yue-Latn">jàu</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嘅<rp>(</rp><rt lang="yue-Latn">ge</rt><rp>)</rp></ruby>，<ruby class="inject-jyutping">喺<rp>(</rp><rt lang="yue-Latn">hái</rt><rp>)</rp></ruby><ruby class="inject-jyutping">尊<rp>(</rp><rt lang="yue-Latn">zyūn</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嚴<rp>(</rp><rt lang="yue-Latn">jìm</rt><rp>)</rp></ruby><ruby class="inject-jyutping">同<rp>(</rp><rt lang="yue-Latn">tùng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">權<rp>(</rp><rt lang="yue-Latn">kyùn</rt><rp>)</rp></ruby><ruby class="inject-jyutping">利<rp>(</rp><rt lang="yue-Latn">lẹi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">上<rp>(</rp><rt lang="yue-Latn">sǒeng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">一<rp>(</rp><rt lang="yue-Latn">jāt</rt><rp>)</rp></ruby><ruby class="inject-jyutping">律<rp>(</rp><rt lang="yue-Latn">lẹot</rt><rp>)</rp></ruby><ruby class="inject-jyutping">平<rp>(</rp><rt lang="yue-Latn">pìng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">等<rp>(</rp><rt lang="yue-Latn">dáng</rt><rp>)</rp></ruby>。<ruby class="inject-jyutping">佢<rp>(</rp><rt lang="yue-Latn">kěoi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">哋<rp>(</rp><rt lang="yue-Latn">dẹi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">具<rp>(</rp><rt lang="yue-Latn">gẹoi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">有<rp>(</rp><rt lang="yue-Latn">jǎu</rt><rp>)</rp></ruby><ruby class="inject-jyutping">理<rp>(</rp><rt lang="yue-Latn">lěi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">性<rp>(</rp><rt lang="yue-Latn">sing</rt><rp>)</rp></ruby><ruby class="inject-jyutping">同<rp>(</rp><rt lang="yue-Latn">tùng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">良<rp>(</rp><rt lang="yue-Latn">lòeng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">心<rp>(</rp><rt lang="yue-Latn">sām</rt><rp>)</rp></ruby>，<ruby class="inject-jyutping">而<rp>(</rp><rt lang="yue-Latn">jì</rt><rp>)</rp></ruby><ruby class="inject-jyutping">且<rp>(</rp><rt lang="yue-Latn">cé</rt><rp>)</rp></ruby><ruby class="inject-jyutping">應<rp>(</rp><rt lang="yue-Latn">jīng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">該<rp>(</rp><rt lang="yue-Latn">gōi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">用<rp>(</rp><rt lang="yue-Latn">jụng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">兄<rp>(</rp><rt lang="yue-Latn">hīng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">弟<rp>(</rp><rt lang="yue-Latn">dại</rt><rp>)</rp></ruby><ruby class="inject-jyutping">間<rp>(</rp><rt lang="yue-Latn">gāan</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嘅<rp>(</rp><rt lang="yue-Latn">ge</rt><rp>)</rp></ruby><ruby class="inject-jyutping">關<rp>(</rp><rt lang="yue-Latn">gwāan</rt><rp>)</rp></ruby><ruby class="inject-jyutping">係<rp>(</rp><rt lang="yue-Latn">hại</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嚟<rp>(</rp><rt lang="yue-Latn">lài</rt><rp>)</rp></ruby><ruby class="inject-jyutping">互<rp>(</rp><rt lang="yue-Latn">wụ</rt><rp>)</rp></ruby><ruby class="inject-jyutping">相<rp>(</rp><rt lang="yue-Latn">sōeng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">對<rp>(</rp><rt lang="yue-Latn">deoi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">待<rp>(</rp><rt lang="yue-Latn">dọi</rt><rp>)</rp></ruby>。
</p>

## Download Links
- [Download for Firefox](https://addons.mozilla.org/en-US/firefox/addon/inject-jyutping-diacritics/)
- Download for Chrome (pending review)
- [GitHub Repo](https://github.com/kennitochang/inject-jyutping)
