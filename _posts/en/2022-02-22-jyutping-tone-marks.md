---
layout: post
title: Annotating Text with Tone-Marked Jyutping
lang-ref: jytuping-tones-marks
---

I recently came across CanCLID's [Inject Jyutping](https://github.com/CanCLID/inject-jyutping) browser extension. The basic idea is to annotate Chinese characters with the associated Cantonese pronunciation in [jyutping](https://en.wikipedia.org/wiki/Jyutping), the _de facto_ standard romanization for Cantonese in academia and education. However, I unfortunately found it difficult to use due to an often-cited issue with Jyutping, which is that it uses numbers to represent tones, causing a high degree of clutter and excessive spacing between characters which can make the original text hard to read. 


One alternative to represent tones using tone marks, also known diacritics, small markings attached to existing Roman letters. This is the approach used by the [Vietnamese alphabet](https://en.wikipedia.org/wiki/Vietnamese_alphabet) and also to represent tones in [pinyin](https://en.wikipedia.org/wiki/Pinyin), the near-universal standard for representing Mandarin Chinese pronunciations. Tone marks have the benefit of condensing text and providing visual and mnemonic cues guiding the reader's pronunciation of words. These benefits are well-appreciated by users of both Vietnamese and pinyin.

As it stands, the Linguistic Society of Hong Kong (see [jyutping.org](https://jyutping.org)) is yet to release an official proposal for adding tone marks. In my current study of Cantonese, I have adopted a set of my own tone marks for personal use. I am certainly [not](https://www.reddit.com/r/Cantonese/comments/7r4y5b/random_idea_vietnamese_tone_marks) [the](http://www.cantonese.sheik.co.uk/phorum/read.php?1,127274,131154) [only](https://www.amazon.com/Cantonese-Everyone-English-Chinese/dp/9620718615) [person](https://www.facebook.com/CantoneseABC) to have done so. Here, I detail the system I chose, and an example of how tone marks might be useful in a browser extension for annotating text. This system of tone marks is not official by any means, and I hope that in publishing this I can help to spur discussion around the introduction of tone marks to jyutping.

## Comparison of "Numbered" vs "Marked" Jyutping annotation

| ![A poem annotated with numbered jyutping.](/assets/images/jyutping-number-annotation.png) | ![A poem annotated with marked jyutping.](/assets/images/jyutping-tonemark-annotation.png) |
|-|-|
| | |

At a small cost in terms of the ability to distinguish tones, tone-marked jyutping reduces the amount of clutter and space between annotated Chinese characters. It provides a more natural reading experience for anyone wishing to study jyutping and/or Cantonese.

## Cantonese Tones
Cantonese is generally accepted by linguists to have six tones (seven in some cases, although the "seventh tone" is largely merging into the first tone).

| Tone Number | Description | Yale | Closest Vietnamese Tone\* | Closest Mandarin Tone |
|-------------|-------------|------|---------------------------|-----------------------|
| 1           | high level  | ā    | X                         | ā                     |
| 2           | high rising | á    | á                         | á                     |
| 3           | mid level   | a    | a                         | X                     |
| 4           | low falling | àh   | à, ả                      | ǎ                     |
| 5           | low rising  | áh   | X                         | X                     |
| 6           | low level   | ah   | ạ                         | X                     |

\* Hanoi pronunciations. Note that Vietnamese tones are often perceived through vowel phonotation and tone contour, rather than pitch and tone countour as in Cantonese. For these comparisons, we rely exclusively on pitch and tone contour. Thus, these comparisons might not accurately represent how speakers of either language might perceive tones from the other language.

## Choice of Tone Marks

The tone marks I chose were based off of four principles:

- Familiarity and compatibility with existing systems, namely Vietnamese, pinyin, and the Yale romanization with tone marks. This is difficult to define, but tone marks which appear in other systems should produce the same sounds in Cantonese whenever possible.
- Tone marks that are easy to interpret.
- Visual distinctness of tone marks.
- Using [precomposed unicode characters](https://en.wikipedia.org/wiki/List_of_precomposed_Latin_characters_in_Unicode) for lexical items. Generally, we need tone marks that are available for all vowels _aeiou_ and for the low tones (4-6) plus the changed tone (2) on the letter _n_. 

For tones 1-3 and 6, it is easy to satisfy all of these criteria.

1. The macron (ā) is used by the Yale romanization and pinyin for a high level tone, and it does not appear in Vietnamese (which has no high level tone of the same height as that of Cantonese), and is thus a natural choice for the first tone.

2. The acute accent (á) is used universally by all three systems for a high rising tone, and is thus natural for the second tone. The mark visually resembles a rising tone.

3. For the third tone, Yale and Vietnamese both use an unmarked vowel to represent a mid-level tone, and Mandarin uses it for a neutral tone. Cantonese does not have a neutral tone, although words with the third tone are often used similar to those in Mandarin with a neutral tone (e.g. for the possessive marker 嘅, equivalent to 的, and a high percentage of final particles). Thus, an unmarked syllable is the natural choice.

6. Neither pinyin nor Yale has an equivalent tone mark for the low-level tone (equivalent to tone 6 - Yale uses the letter _h_ to indicate this, and Mandarin does not have an equivalent tone). Vietnamese has a glottalized tone with a similar contour, for which it uses a dot below (ạ). Vietnamese words with this tone are generally etymologically related to Cantonese words with the same tone, making it a natural choice. Visually, a dot below can be thought of as the antithesis to the macron above (ā), as indicating a downward shift in pitch rather than an upward shift.

The remaining two tones (4 and 5) pose more of a quandary, as the closest tones in the other systems are more disparate. Based on the criteria of emphasizing precomposed Unicode characters, we only have a few options, namely the haček (ǎ), grave (à), and tilde (ã) accents. We can also consider the circumflex (â), which has appeared in other proposals, since although there is no precomposed character with _n_, it is still possible to type an _n_ with a circumflex easily using the ABC-Extended keyboard on Mac OS.

Under the visual distinctiveness criterion, the tilde (ã) is a poor choice due to its strong visual similarity with the macron (ā) in many typefaces.

The circumflex (â) is also a poor choice, because in Vietnamese and (rarely) Hanyu Pinyin, it appears over certain vowels to indicate difference in vowel _quality_ rather than tone. The Vietnamese alphabet contains distinct vowels _â_, _ô_, and _ê_, while pinyin contains _ê_ for a small set of words. This could result in confusion to users of these other systems as to what mark indicates tone and which indicates an entirely different vowel.

The only remaining choices are the haček (ǎ) and the grave (à). While arguments could be made for either assignment to tones 4 and 5, I believe the arguments are stronger for having tone 4 = à and 5 = ǎ. For one, a grave (à) accent makes much more sense for a falling tone than it does for a rising tone, and is used for falling tones in all three systems. Secondly, while in most cases the Mandarin tone indicated in pinyin by a haček (ǎ) is closer to the Cantonese low falling tone in many scenarios, it can also be pronounced closer to the low rising tone in other senarios (such as in isolation). Finally, words with the low rising tone are generally etymologically related to Mandarin words which use the haček in pinyin, which could be helpful to speakers of Mandarin.

 Based on this train of reasoning, we arrive at the following system:

| 1 | 2 | 3 | 4 | 5 | 6 |
|---|---|---|---|---|---|
| ā | á | a | à | ǎ | ạ |


## Browser Extension
- [Download for Firefox](https://addons.mozilla.org/en-US/firefox/addon/inject-jyutping-diacritics/)

