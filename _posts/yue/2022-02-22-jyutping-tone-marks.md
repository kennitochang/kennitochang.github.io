---
layout: post
title: 用聲調符號性粵拼嚟標漢字
lang-ref: jytuping-tones-marks
---

所有觀點都係我自己嘅
我最近遇到了 CanCLID 的 [Inject Jyutping](https://github.com/CanCLID/inject-jyutping) 瀏覽器擴展程序，它使用 [jyutping](https://en.wikipedia.org) 中的相關粵語發音來註釋漢字/wiki/Jyutping），粵語在學術界和教育界的_de facto_標準羅馬化。但是，由於 Jyutping 的一個備受爭議的特性，我發現該擴展很難使用，即它使用數字來表示音調。在這種情況下，使註解的數字顯得雜亂無章。

編號音調的一種替代方法是使用[越南語](https://en.wikipedia.org/wiki/Vietnamese_alphabet)和普通話[pinyin](https://en.wikipedia.org/wiki/拼音)。聲調標記的好處是可以產生更簡潔的文本，並提供視覺和記憶線索來指導讀者的單詞發音。這些好處受到越南語和拼音用戶的好評。

目前，香港語言學會（見 [jyutping.org](https://jyutping.org)）尚未發布正式建議添加聲調。到目前為止，我一直在使用自己的聲標系統來學習粵語。除咗我梗係有[其](https://www.reddit.com/r/Cantonese/comments/7r4y5b/random_idea_vietnamese_tone_marks)[他](http://www.cantonese.sheik.co.uk/phorum/read.php ?1,127274,131154)[人](https://www.amazon.com/Cantonese-Everyone-English-Chinese/dp/9620718615) [咁](https://www.facebook.com/CantoneseABC)做。

歸根結底，我相信在粵語標準中添加音標可能會大有裨益。當涉及到直接註釋文本時，正如我在下面討論的那樣，有聲標記的jyutping 比常規的數字jyutping 具有顯著的優勢。我使用的聲調系統是我自己的創造，雖然這不是這裡的主要重點——我希望在發布這個擴展時，我可以幫助激發關於未來將聲調引入註音的討論。

粵語的六聲可以用助記詞一碗半牛腩飯（一碗半牛腩飯）來記住。有關區分六種音調的練習，請參閱 [此處](https://jyutping.org/en/docs/tone/)。

## 使用變音符號注入 Jyutping

基於 CanCLID 的瀏覽器擴展，我創建了一個新的瀏覽器擴展用於 jyutping 註釋，它使用以下音標系統：

|音調 | 1¯ | 2' | 3 | 4` | 5ˇ | 6. |
|-------------|---|---|---|---|---|---|
|說明 |陰平、高陰入 |陰上|陰去、低陰入 |陽平|陽上|陽去、陽入  |
|示例 | <span style="font-size:250%;">一</span> | <span style="font-size:250%;">碗</span> | <span style="font-size:250%;">半</span> | <span style="font-size:250%;">牛</span> | <span style="font-size:250%;">腩</span> | <span style="font-size:250%;">飯</span> |
|玉屏 |jāt1 | wun2 |bun3 | ngau4 | naam5 | faan6 |
| Jyutping 與變音符號 |jāt | wún |bun | ngàu | nǎam | fạan |

我選擇上面的音標是基於與漢語拼音、越南語和耶魯拼音的類比，著眼於對 Unicode 的支持。在瀏覽器擴展的未來版本中，我希望允許用戶根據需要選擇自己的音標。

在視覺上區分音調的能力方面，有聲調的注音減少了帶註釋的漢字之間的雜亂和空間。與數字注音相比，它可以為帶註釋的粵語文本提供更緊湊的閱讀體驗。

### 使用音標jyutping的註釋示例
<p><ruby class="inject-jyutping">人<rp>(</rp><rt lang="yue-Latn">jàn</rt><rp>)</rp></ruby><ruby class="inject-jyutping">人<rp>(</rp><rt lang="yue-Latn">jàn</rt><rp>)</rp></ruby><ruby class="inject-jyutping">生<rp>(</rp><rt lang="yue-Latn">sāang</rt><rp>)</rp></ruby><ruby class="inject-jyutping">出<rp>(</rp><rt lang="yue-Latn">cēot</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嚟<rp>(</rp><rt lang="yue-Latn">lài</rt><rp>)</rp></ruby><ruby class="inject-jyutping">就<rp>(</rp><rt lang="yue-Latn">zạu</rt><rp>)</rp></ruby><ruby class="inject-jyutping">係<rp>(</rp><rt lang="yue-Latn">hại</rt><rp>)</rp></ruby><ruby class="inject-jyutping">自<rp>(</rp><rt lang="yue-Latn">zị</rt><rp>)</rp></ruby><ruby class="inject-jyutping">由<rp>(</rp><rt lang="yue-Latn">jàu</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嘅<rp>(</rp><rt lang="yue-Latn">ge</rt><rp>)</rp></ruby>，<ruby class="inject-jyutping">喺<rp>(</rp><rt lang="yue-Latn">hái</rt><rp>)</rp></ruby><ruby class="inject-jyutping">尊<rp>(</rp><rt lang="yue-Latn">zyūn</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嚴<rp>(</rp><rt lang="yue-Latn">jìm</rt><rp>)</rp></ruby><ruby class="inject-jyutping">同<rp>(</rp><rt lang="yue-Latn">tùng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">權<rp>(</rp><rt lang="yue-Latn">kyùn</rt><rp>)</rp></ruby><ruby class="inject-jyutping">利<rp>(</rp><rt lang="yue-Latn">lẹi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">上<rp>(</rp><rt lang="yue-Latn">sǒeng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">一<rp>(</rp><rt lang="yue-Latn">jāt</rt><rp>)</rp></ruby><ruby class="inject-jyutping">律<rp>(</rp><rt lang="yue-Latn">lẹot</rt><rp>)</rp></ruby><ruby class="inject-jyutping">平<rp>(</rp><rt lang="yue-Latn">pìng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">等<rp>(</rp><rt lang="yue-Latn">dáng</rt><rp>)</rp></ruby>。<ruby class="inject-jyutping">佢<rp>(</rp><rt lang="yue-Latn">kěoi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">哋<rp>(</rp><rt lang="yue-Latn">dẹi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">具<rp>(</rp><rt lang="yue-Latn">gẹoi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">有<rp>(</rp><rt lang="yue-Latn">jǎu</rt><rp>)</rp></ruby><ruby class="inject-jyutping">理<rp>(</rp><rt lang="yue-Latn">lěi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">性<rp>(</rp><rt lang="yue-Latn">sing</rt><rp>)</rp></ruby><ruby class="inject-jyutping">同<rp>(</rp><rt lang="yue-Latn">tùng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">良<rp>(</rp><rt lang="yue-Latn">lòeng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">心<rp>(</rp><rt lang="yue-Latn">sām</rt><rp>)</rp></ruby>，<ruby class="inject-jyutping">而<rp>(</rp><rt lang="yue-Latn">jì</rt><rp>)</rp></ruby><ruby class="inject-jyutping">且<rp>(</rp><rt lang="yue-Latn">cé</rt><rp>)</rp></ruby><ruby class="inject-jyutping">應<rp>(</rp><rt lang="yue-Latn">jīng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">該<rp>(</rp><rt lang="yue-Latn">gōi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">用<rp>(</rp><rt lang="yue-Latn">jụng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">兄<rp>(</rp><rt lang="yue-Latn">hīng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">弟<rp>(</rp><rt lang="yue-Latn">dại</rt><rp>)</rp></ruby><ruby class="inject-jyutping">間<rp>(</rp><rt lang="yue-Latn">gāan</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嘅<rp>(</rp><rt lang="yue-Latn">ge</rt><rp>)</rp></ruby><ruby class="inject-jyutping">關<rp>(</rp><rt lang="yue-Latn">gwāan</rt><rp>)</rp></ruby><ruby class="inject-jyutping">係<rp>(</rp><rt lang="yue-Latn">hại</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嚟<rp>(</rp><rt lang="yue-Latn">lài</rt><rp>)</rp></ruby><ruby class="inject-jyutping">互<rp>(</rp><rt lang="yue-Latn">wụ</rt><rp>)</rp></ruby><ruby class="inject-jyutping">相<rp>(</rp><rt lang="yue-Latn">sōeng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">對<rp>(</rp><rt lang="yue-Latn">deoi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">待<rp>(</rp><rt lang="yue-Latn">dọi</rt><rp>)</rp></ruby>。
</p>

## 下載瀏覽器擴展 
- [火狐下載](https://addons.mozilla.org/en-US/firefox/addon/inject-jyutping-diacritics/)
- 谷歌瀏覽器下載(仲未畀人批准)
- [GitHub Repo](https://github.com/kennitochang/inject-jyutping)
