---
layout: post
title: 用聲調符號性粵拼嚟標漢字
lang-ref: jytuping-tones-marks
---

調整CanCLID嘅[Inject Jyutping](https://github.com/CanCLID/inject-jyutping)瀏覽器擴展，我創建咗一個新嘅瀏覽器擴展用於粵拼註釋，佢用以下嘅音標系統：

| 代表數字同符號 | 1¯ | 2´ | 3  | 4` | 5ˇ | 6. |
|-------------|---|---|---|---|---|---|
| 傳統聲調名 |陰平、高陰入 |陰上|陰去、低陰入 |陽平|陽上|陽去、陽入  |
| 例子 | <span style="font-size:250%;">一</span> | <span style="font-size:250%;">碗</span> | <span style="font-size:250%;">半</span> | <span style="font-size:250%;">牛</span> | <span style="font-size:250%;">腩</span> | <span style="font-size:250%;">飯</span> |
| 粵拼 |jat1 | wun2 |bun3 | ngau4 | naam5 | faan6 |
| 聲調符號性粵拼 |jāt | wún |bun | ngàu | nǎam | fạan |

以越南文、漢語拼音、同埋耶魯粵語拼音為基礎，亦試緊 Unicode 嘅支持，我揀上面嘅音標。喺瀏覽器擴展嘅未來版本中，我希望允許用户揀自己所想嘅音標。

喺視覺上區分音調嘅方面，有聲調符號性粵拼減少雜亂同漢字中間嘅空間。對比數字性粵拼，可以令閱讀體驗更加有效果。

### 用聲調符號性粵拼嘅註釋例子
<p><ruby class="inject-jyutping">人<rp>(</rp><rt lang="yue-Latn">jàn</rt><rp>)</rp></ruby><ruby class="inject-jyutping">人<rp>(</rp><rt lang="yue-Latn">jàn</rt><rp>)</rp></ruby><ruby class="inject-jyutping">生<rp>(</rp><rt lang="yue-Latn">sāang</rt><rp>)</rp></ruby><ruby class="inject-jyutping">出<rp>(</rp><rt lang="yue-Latn">cēot</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嚟<rp>(</rp><rt lang="yue-Latn">lài</rt><rp>)</rp></ruby><ruby class="inject-jyutping">就<rp>(</rp><rt lang="yue-Latn">zạu</rt><rp>)</rp></ruby><ruby class="inject-jyutping">係<rp>(</rp><rt lang="yue-Latn">hại</rt><rp>)</rp></ruby><ruby class="inject-jyutping">自<rp>(</rp><rt lang="yue-Latn">zị</rt><rp>)</rp></ruby><ruby class="inject-jyutping">由<rp>(</rp><rt lang="yue-Latn">jàu</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嘅<rp>(</rp><rt lang="yue-Latn">ge</rt><rp>)</rp></ruby>，<ruby class="inject-jyutping">喺<rp>(</rp><rt lang="yue-Latn">hái</rt><rp>)</rp></ruby><ruby class="inject-jyutping">尊<rp>(</rp><rt lang="yue-Latn">zyūn</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嚴<rp>(</rp><rt lang="yue-Latn">jìm</rt><rp>)</rp></ruby><ruby class="inject-jyutping">同<rp>(</rp><rt lang="yue-Latn">tùng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">權<rp>(</rp><rt lang="yue-Latn">kyùn</rt><rp>)</rp></ruby><ruby class="inject-jyutping">利<rp>(</rp><rt lang="yue-Latn">lẹi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">上<rp>(</rp><rt lang="yue-Latn">sǒeng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">一<rp>(</rp><rt lang="yue-Latn">jāt</rt><rp>)</rp></ruby><ruby class="inject-jyutping">律<rp>(</rp><rt lang="yue-Latn">lẹot</rt><rp>)</rp></ruby><ruby class="inject-jyutping">平<rp>(</rp><rt lang="yue-Latn">pìng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">等<rp>(</rp><rt lang="yue-Latn">dáng</rt><rp>)</rp></ruby>。<ruby class="inject-jyutping">佢<rp>(</rp><rt lang="yue-Latn">kěoi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">哋<rp>(</rp><rt lang="yue-Latn">dẹi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">具<rp>(</rp><rt lang="yue-Latn">gẹoi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">有<rp>(</rp><rt lang="yue-Latn">jǎu</rt><rp>)</rp></ruby><ruby class="inject-jyutping">理<rp>(</rp><rt lang="yue-Latn">lěi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">性<rp>(</rp><rt lang="yue-Latn">sing</rt><rp>)</rp></ruby><ruby class="inject-jyutping">同<rp>(</rp><rt lang="yue-Latn">tùng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">良<rp>(</rp><rt lang="yue-Latn">lòeng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">心<rp>(</rp><rt lang="yue-Latn">sām</rt><rp>)</rp></ruby>，<ruby class="inject-jyutping">而<rp>(</rp><rt lang="yue-Latn">jì</rt><rp>)</rp></ruby><ruby class="inject-jyutping">且<rp>(</rp><rt lang="yue-Latn">cé</rt><rp>)</rp></ruby><ruby class="inject-jyutping">應<rp>(</rp><rt lang="yue-Latn">jīng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">該<rp>(</rp><rt lang="yue-Latn">gōi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">用<rp>(</rp><rt lang="yue-Latn">jụng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">兄<rp>(</rp><rt lang="yue-Latn">hīng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">弟<rp>(</rp><rt lang="yue-Latn">dại</rt><rp>)</rp></ruby><ruby class="inject-jyutping">間<rp>(</rp><rt lang="yue-Latn">gāan</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嘅<rp>(</rp><rt lang="yue-Latn">ge</rt><rp>)</rp></ruby><ruby class="inject-jyutping">關<rp>(</rp><rt lang="yue-Latn">gwāan</rt><rp>)</rp></ruby><ruby class="inject-jyutping">係<rp>(</rp><rt lang="yue-Latn">hại</rt><rp>)</rp></ruby><ruby class="inject-jyutping">嚟<rp>(</rp><rt lang="yue-Latn">lài</rt><rp>)</rp></ruby><ruby class="inject-jyutping">互<rp>(</rp><rt lang="yue-Latn">wụ</rt><rp>)</rp></ruby><ruby class="inject-jyutping">相<rp>(</rp><rt lang="yue-Latn">sōeng</rt><rp>)</rp></ruby><ruby class="inject-jyutping">對<rp>(</rp><rt lang="yue-Latn">deoi</rt><rp>)</rp></ruby><ruby class="inject-jyutping">待<rp>(</rp><rt lang="yue-Latn">dọi</rt><rp>)</rp></ruby>。
</p>

## 下載瀏覽器擴展 
- [火狐下載](https://addons.mozilla.org/en-US/firefox/addon/inject-jyutping-diacritics/)
- [谷歌瀏覽器下載](https://chrome.google.com/webstore/detail/inject-jyutping-with-tone/ljoecadmcgpclnfpdghdpcneldiinbkp?hl=en&authuser=0)
- [GitHub Repo](https://github.com/kennitochang/inject-jyutping)
