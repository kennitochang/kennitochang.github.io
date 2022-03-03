--- layout: post
title: 用聲調符號性粵拼嚟標漢字
lang-ref: jytuping-tones-marks
---
所有觀點都係我自己嘅

我最近遇到CanCLID嘅[Inject Jyutping](https://github.com/CanCLID/inject-jyutping)瀏覽器擴展程序，即係使用事實上喺學術界同教育界標準哋所用嘅[粵拼](https://zh-yue.wikipedia.org/wiki/%E9%A6%99%E6%B8%AF%E8%AA%9E%E8%A8%80%E5%AD%B8%E5%AD%B8%E6%9C%83%E7%B2%B5%E8%AA%9E%E6%8B%BC%E9%9F%B3%E6%96%B9%E6%A1%88)嚟標漢字。不過，由於粵拼嘅一個備受爭議嘅特性，即係使用數字嚟表示音調，我認為係少少難用嘅。即係因為註解嘅數字顯得烏喱馬扠。

編號音調嘅一種替代方法係模仿[越南語](https://zh-yue.wikipedia.org/wiki/%E8%B6%8A%E5%8D%97%E5%9C%8B%E8%AA%9E%E5%AD%97)同普通話[拼音](https://zh-yue.wikipedia.org/wiki/%E6%BC%A2%E8%AA%9E%E6%8B%BC%E9%9F%B3)。聲調標記嘅好處係可以產生更簡潔嘅文本，並提供視覺和記憶線索來指導讀者嘅單詞發音。這些好處受到越南語和拼音用戶嘅好評。

目前，香港語言學學會（見 [jyutping.org](https://jyutping.org)）仲未發布正式建議添加聲調。依家，我用緊自己嘅聲標系統嚟學習粵語。除咗我之外，梗係有[其](https://www.reddit.com/r/Cantonese/comments/7r4y5b/random_idea_vietnamese_tone_marks)[他](http://www.cantonese.sheik.co.uk/phorum/read.php ?1,127274,131154)[人](https://www.amazon.com/Cantonese-Everyone-English-Chinese/dp/9620718615) [咁](https://www.facebook.com/CantoneseABC)做。

歸根結底，我相信在粵語標準中添加音標可能會大有裨益。當涉及到直接註釋文本時，正如我在下面討論嘅那樣，有聲標記嘅jyutping 比常規嘅數字jyutping 具有顯著嘅優勢。我使用嘅聲調系統係我自己嘅創造，雖然這唔係這裡嘅主要重點——我希望在發布這個擴展時，我可以幫助激發關於未來將聲調引入註音嘅討論。

粵語嘅六聲可以用助記詞一碗半牛腩飯（一碗半牛腩飯）來記住。有關區分六種音調嘅練習，請參閱 [此處](https://jyutping.org/en/docs/tone/)。

## 使用變音符號注入 Jyutping

基於 CanCLID 嘅瀏覽器擴展，我創建了一個新嘅瀏覽器擴展用於 jyutping 註釋，它使用以下音標系統：

|音調 | 1¯ | 2' | 3 | 4` | 5ˇ | 6. |
|-------------|---|---|---|---|---|---|
|說明 |陰平、高陰入 |陰上|陰去、低陰入 |陽平|陽上|陽去、陽入  |
|示例 | <span style="font-size:250%;">一</span> | <span style="font-size:250%;">碗</span> | <span style="font-size:250%;">半</span> | <span style="font-size:250%;">牛</span> | <span style="font-size:250%;">腩</span> | <span style="font-size:250%;">飯</span> |
|玉屏 |jāt1 | wun2 |bun3 | ngau4 | naam5 | faan6 |
| Jyutping 與變音符號 |jāt | wún |bun | ngàu | nǎam | fạan |

我選擇上面嘅音標係基於與漢語拼音、越南語和耶魯拼音嘅類比，著眼於對 Unicode 嘅支持。在瀏覽器擴展嘅未來版本中，我希望允許用戶根據需要選擇自己嘅音標。

在視覺上區分音調嘅能力方面，有聲調嘅注音減少了帶註釋嘅漢字之間嘅雜亂和空間。與數字注音相比，它可以為帶註釋嘅粵語文本提供更緊湊嘅閱讀體驗。

### 使用音標jyutping嘅註釋示例
<p><ruby class="inject-jyutping">人<rp>(</rp><rt lang="yue-Latn">jàn</rt><rp>)</rp></ruby><ruby class="inject-jyutping">人<rp>(</rp><rt lang="yue-Latn">jàn</rt><rp>)</rp></ruby><ruby class="inject-jyutping">生<rp>(</rp><rt lang="yue-Latn">sāang</rt><rp>)</rp></ruby><ruby class="inject-jyutping">出<rp>(</rp><rt lang="yue-Latn">cēot</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嚟<rp>(</rp><rt lang="yue-Latn">lài</rt><rp>)</rp></ruby><ruby class="inject-jyutping">就<rp>(</rp><rt lang="yue-Latn">zạu</rt><rp>)</rp></ruby><ruby class="inject-jyutping">係<rp>(</rp><rt lang="yue-Latn">hại</rt><rp>)</rp></ruby><ruby class="inject-jyutping">自<rp>(</rp><rt lang="yue-Latn">zị</rt><rp>)</rp></ruby><ruby class="inject-jyutping">由<rp>(</rp><rt lang="yue-Latn">jàu</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嘅<rp>(</rp><rt lang="yue-Latn">ge</rt><rp>)</rp></ruby>，<ruby class="inject-jyutping">喺<rp>(</rp><rt lang="yue-Latn">hái</rt><rp>)</rp></ruby><ruby class="inject-jyutping">尊<rp>(</rp><rt lang="yue-Latn">zyūn</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嚴<rp>(</rp><rt lang="yue-Latn">jìm</rt><rp>)</rp></ruby><ruby class="inject-jyutping">同<rp>(</rp><rt lang="yue-Latn">tùng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">權<rp>(</rp><rt lang="yue-Latn">kyùn</rt><rp>)</rp></ruby><ruby class="inject-jyutping">利<rp>(</rp><rt lang="yue-Latn">lẹi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">上<rp>(</rp><rt lang="yue-Latn">sǒeng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">一<rp>(</rp><rt lang="yue-Latn">jāt</rt><rp>)</rp></ruby><ruby class="inject-jyutping">律<rp>(</rp><rt lang="yue-Latn">lẹot</rt><rp>)</rp></ruby><ruby class="inject-jyutping">平<rp>(</rp><rt lang="yue-Latn">pìng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">等<rp>(</rp><rt lang="yue-Latn">dáng</rt><rp>)</rp></ruby>。<ruby class="inject-jyutping">佢<rp>(</rp><rt lang="yue-Latn">kěoi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">哋<rp>(</rp><rt lang="yue-Latn">dẹi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">具<rp>(</rp><rt lang="yue-Latn">gẹoi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">有<rp>(</rp><rt lang="yue-Latn">jǎu</rt><rp>)</rp></ruby><ruby class="inject-jyutping">理<rp>(</rp><rt lang="yue-Latn">lěi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">性<rp>(</rp><rt lang="yue-Latn">sing</rt><rp>)</rp></ruby><ruby class="inject-jyutping">同<rp>(</rp><rt lang="yue-Latn">tùng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">良<rp>(</rp><rt lang="yue-Latn">lòeng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">心<rp>(</rp><rt lang="yue-Latn">sām</rt><rp>)</rp></ruby>，<ruby class="inject-jyutping">而<rp>(</rp><rt lang="yue-Latn">jì</rt><rp>)</rp></ruby><ruby class="inject-jyutping">且<rp>(</rp><rt lang="yue-Latn">cé</rt><rp>)</rp></ruby><ruby class="inject-jyutping">應<rp>(</rp><rt lang="yue-Latn">jīng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">該<rp>(</rp><rt lang="yue-Latn">gōi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">用<rp>(</rp><rt lang="yue-Latn">jụng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">兄<rp>(</rp><rt lang="yue-Latn">hīng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">弟<rp>(</rp><rt lang="yue-Latn">dại</rt><rp>)</rp></ruby><ruby class="inject-jyutping">間<rp>(</rp><rt lang="yue-Latn">gāan</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嘅<rp>(</rp><rt lang="yue-Latn">ge</rt><rp>)</rp></ruby><ruby class="inject-jyutping">關<rp>(</rp><rt lang="yue-Latn">gwāan</rt><rp>)</rp></ruby><ruby class="inject-jyutping">係<rp>(</rp><rt lang="yue-Latn">hại</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嚟<rp>(</rp><rt lang="yue-Latn">lài</rt><rp>)</rp></ruby><ruby class="inject-jyutping">互<rp>(</rp><rt lang="yue-Latn">wụ</rt><rp>)</rp></ruby><ruby class="inject-jyutping">相<rp>(</rp><rt lang="yue-Latn">sōeng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">對<rp>(</rp><rt lang="yue-Latn">deoi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">待<rp>(</rp><rt lang="yue-Latn">dọi</rt><rp>)</rp></ruby>。
</p>

## 下載瀏覽器擴展 
- [火狐下載](https://addons.mozilla.org/en-US/firefox/addon/inject-jyutping-diacritics/)
- 谷歌瀏覽器下載(仲未畀人批准)
- [GitHub Repo](https://github.com/kennitochang/inject-jyutping)
