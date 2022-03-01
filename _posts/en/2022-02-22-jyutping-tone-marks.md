---
layout: post
title: Annotating Text with Tone-Marked Jyutping
lang-ref: jytuping-tones-marks
---

_All views are my own._

I recently came across CanCLID's [Inject Jyutping](https://github.com/CanCLID/inject-jyutping) browser extension. The basic idea is to annotate Chinese characters with the associated Cantonese pronunciation in [jyutping](https://en.wikipedia.org/wiki/Jyutping), the _de facto_ standard romanization for Cantonese in academia and education devised by the Linguistic Society of Hong Kong. However, I unfortunately found it difficult to use due to an often-cited issue with Jyutping, which is that it uses numbers to represent tones, making it appear cluttered and sometimes difficult to interpret. 


One alternative to represent tones using tone marks, also known diacritics, small markings attached to existing Roman letters. This is the approach used by the [Vietnamese alphabet](https://en.wikipedia.org/wiki/Vietnamese_alphabet) and also to represent tones in Mandarin [pinyin](https://en.wikipedia.org/wiki/Pinyin). Tone marks have the benefit of condensing text and providing visual and mnemonic cues guiding the reader's pronunciation of words. These benefits are well-appreciated by users of both Vietnamese and pinyin.

As it stands, the Linguistic Society of Hong Kong (see [jyutping.org](https://jyutping.org)) is yet to release an official proposal for adding tone marks. In my current study of Cantonese, I have adopted a set of my own tone marks for personal use. I am certainly [not](https://www.reddit.com/r/Cantonese/comments/7r4y5b/random_idea_vietnamese_tone_marks) [the](http://www.cantonese.sheik.co.uk/phorum/read.php?1,127274,131154) [only](https://www.amazon.com/Cantonese-Everyone-English-Chinese/dp/9620718615) [person](https://www.facebook.com/CantoneseABC) to have done so. Here, I provide an example of how tone marks might be useful in a browser extension for annotating text. The system of tone marks I employed is not official by any means, and I hope that in publishing this extension I can help spur discussion around the possible introduction of tone marks to jyutping.

## Comparison of "Numbered" vs "Marked" Jyutping annotation

Based on CanCLID's browser extension, I created a browser extension for jyutping annotation that uses the following system:

| Tone Number | 1 | 2 | 3 | 4 | 5 | 6 |
|-------------|---|---|---|---|---|---|
| Description  | high level | high rising | mid level | low falling | low rising | low level |
| Tone Mark   | <span style="font-size:250%;">ō</span> | <span style="font-size:250%;">ó</span> | <span style="font-size:250%;">o</span> | <span style="font-size:250%;">ò</span> | <span style="font-size:250%;">ǒ</span> | <span style="font-size:250%;">ọ</span> |
| Example   | 一 jāt | 碗 wún | 半 bun | 牛 ngàu | 腩 nǎam | 飯 fạan |
| Visualization   | ![](/assets/images/jat_tone.png) | ![](/assets/images/wun_tone.png) | ![](/assets/images/bun_tone.png) | ![](/assets/images/ngau_tone.png) | ![](/assets/images/naam_tone.png) | ![](/assets/images/faan_tone.png) |

The six tones of Cantonese can be remembered using the mnemonic 一碗半牛腩飯 (one and a half bowls of beef brisket rice).


At a small cost in terms of the ability to distinguish tones visually, tone-marked jyutping reduces the amount of clutter and space between annotated Chinese characters. It provides a more compact reading experience for learning Cantonese and/or jyutping.

| ![A poem annotated with numbered jyutping.](/assets/images/jyutping-number-annotation.png) | ![A poem annotated with marked jyutping.](/assets/images/jyutping-tonemark-annotation.png) |
|-|-|
| | |

A discussion of Cantonese tones and a rationale for choosing these tone marks is given in the Appendix. In future versions of the browser extension, I hope to allow users to select their own tone marks if they wish.

## Download Link
- [Download for Firefox](https://addons.mozilla.org/en-US/firefox/addon/inject-jyutping-diacritics/)
- Download for Chrome (pending review)



## Appendix: Choice of Tone Marks
Cantonese is generally accepted by linguists to have six tones (seven in some cases, although the "seventh tone" is largely merging into the first tone). I have included the commonly accepted descriptions of each tone with similar tones from (Hanoi) Vietnamese and Mandarin. These groupings are somewhat subjective.

| Tone Number | Description | Yale | Closest Vietnamese Tone\* | Closest Mandarin Tone |
|-------------|-------------|------|---------------------------|-----------------------|
| 1           | high level  | ā    | X                         | ā (T1)                |
| 2           | high rising | á    | á (sắc)                   | á (T2)                |
| 3           | mid level   | a    | a (ngang)                 | X                     |
| 4           | low falling | àh   | à (huyền), ả (hỏi)        | ǎ (T3)                |
| 5           | low rising  | áh   | X                         | X                     |
| 6           | low level   | ah   | ạ (nặng)                  | X                     |

<small>\* Note that Vietnamese tones' production and perception depends on both pitch and [phonation](https://en.wikipedia.org/wiki/Phonation). For these comparisons, we rely on pitch contour only, as phonation is a negligible factor in Cantonese tones. Thus, these comparisons might not accurately represent how speakers of Vietnamese and Cantonese might perceive tones from the other language.</small>

The tone marks I chose were based off of four principles:

- Familiarity and compatibility with existing systems, namely Vietnamese, pinyin, and the Yale romanization with tone marks. This is difficult to define, but tone marks which appear in other systems should produce the same sounds in Cantonese whenever possible.
- Tone marks that are easy to interpret.
- Visual distinctness of tone marks.
- Using [precomposed Unicode characters](https://en.wikipedia.org/wiki/List_of_precomposed_Latin_characters_in_Unicode) for tones that appear in lexical words. Generally, we need tone marks that are available for all vowels _aeiou_ and for the low tones (4-6) plus the changed tone (2) on the letter _n_. The remaining tone marks for syllabic _m_ and _n_ are desirable but not crucial for distinguishing most shades meaning (unfortunately the support for diacritics on syllabic _m_ is quite poor).

For tones 1-3 and 6, it is easy to satisfy all of these criteria.

1. The macron (ā) is used by the Yale romanization and pinyin for a high level tone, and it does not appear in Vietnamese (which has no high level tone of the same height as that of Cantonese), and is thus a natural choice for the first tone.

2. The acute accent (á) is used universally by all three systems for a high rising tone, and is thus natural for the second tone. The mark visually resembles a rising tone.

3. For the third tone, Yale and Vietnamese both use an unmarked vowel to represent a mid-level tone, and Mandarin uses it for a neutral tone. Cantonese does not have a neutral tone, although words with the third tone are often used similar to those in Mandarin with a neutral tone (e.g. for the possessive marker 嘅, equivalent to 的, and a high percentage of final particles). Thus, an unmarked syllable is the natural choice.

6. Neither pinyin nor Yale has an equivalent tone mark for the low-level tone (equivalent to tone 6 - Yale uses the letter _h_ to indicate this, and Mandarin does not have an equivalent tone). Vietnamese has a glottalized tone with a similar contour, for which it uses a dot below (ạ). Vietnamese words with this tone are generally etymologically related to Cantonese words with tone 6, making this tone mark a natural choice for tone 6. Visually, a dot below can be thought of as the antithesis to the macron above (ā), as indicating a downward shift in pitch rather than an upward shift.

The remaining two tones (4 and 5) pose more of a quandary, as the closest tones in the other systems are more disparate. Based on the criteria of emphasizing precomposed Unicode characters, we only have a few options, namely the haček (ǎ), grave (à), and tilde (ã) accents. We can also consider the circumflex (â), which has appeared in other proposals, since although there is no precomposed character with _n_, it is still possible to type an _n_ with a circumflex easily using the ABC-Extended keyboard on Mac OS.

Under the visual distinctiveness criterion, the tilde (ã) is a poor choice due to its strong visual similarity with the macron (ā) in many typefaces.

The circumflex (â) is also a poor choice, because in Vietnamese and (rarely) Hanyu Pinyin, it appears over certain vowels to indicate difference in vowel _quality_ rather than tone. The Vietnamese alphabet contains distinct vowels _â_, _ô_, and _ê_, while pinyin contains _ê_ for a small set of words. This could result in confusion to users of these other systems as to what marks indicate tone and what marks indicate an entirely different vowel.

The only remaining choices are the haček (ǎ) and the grave (à). While arguments could be made for either assignment to tones 4 and 5, I believe the arguments are stronger for having tone 4 = à and 5 = ǎ. For one, a grave (à) accent makes much more sense for a falling tone than it does for a rising tone, and is used for falling tones in all three systems. Secondly, while in most cases the Mandarin tone indicated in pinyin by a haček (ǎ) is closer to the Cantonese low falling tone in many scenarios, it can also be pronounced closer to the low rising tone in other senarios (such as in isolation). Finally, words with the low rising tone are generally etymologically related to Mandarin words which use the haček in pinyin, which could be helpful to speakers of Mandarin.
