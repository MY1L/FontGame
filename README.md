<a href="https://github.com/MY1L/icense"><img src="https://github.com/MY1L/icense/raw/main/Seal.svg" align="right" width="120" height="64"/></a>

如果你是从[能否自撰个共工符号`u1F77D`「🝽」放统一码里推及全球？](https://www.bilibili.com/video/BV1Gd4y1R7Mj/)找来下载相应字体的，链接改了，请[移步这里](https://github.com/MY1L/Unicode/releases/tag/NotoUni7)。

----

<h1 align="center">噗叽 | Poop</h1>
<p align="center">
<a href="https://afdian.net/@FairyFloss" target="_blank">
<img src="https://user-images.githubusercontent.com/58043328/227652884-7dfc1e74-b947-4dcb-ab4d-b50ca8799e06.png">
</a><br/>为𠷡镀金，画蛇添足<br/>
<img src="https://user-images.githubusercontent.com/58043328/227654992-f7a817bb-8ae5-4762-896c-8a40738fb3b6.gif">
</p>

这是一套从三体动画获得灵感的圆体字重可变字体，支持丰富的排版特性，但非常之答辩。当你使用的时候自然会明白的。

这也是开源字体，欢迎协作，帮忙做字体的人会在这里列出以[致谢](#致谢)。

<h3 align="center"><a href="https://github.com/MY1L/FontGame/releases"><strong>»»» 这边下载 «««</strong></a></h3>

2023年3月25日 初发布，同日三体动画完结

## 我想现在就知道它答辩在哪里。等等，什么是可变字体？
你已经看到动画了，它的笔画是可以无级变化粗细的（即“字重”）。在最粗和最细之间，想要多粗多细都可以随意调整。

注意大多粗体不是细体的直接加粗。为了避免糊作一团，笔画会在加粗过程中避让。

和灵感的答辩原型一样，凡是横画多的字都会残缺横笔。嗯，是故意不小心的。

这还是个特意抽象的字体——意思是一些字形字义相近的字符被合并了，不分大小写，0跟o都不分。相信使用过程中你一定会高呼字体的名称。

开个玩笑，这些字符不分的问题会在之后的版本解决。

### 但我家软件不支持可变字体😣
我做了3个不可变的普通字体，固定3种字重，一般软件也能用。

## 支持的奇妙OpenType特性
GSUB features: calt, ccmp, fwid, pwid, salt, zero；GPOS features: kern

`calt` **上下文替换**，根据上下文，在不改变字义的前提下调整字形。

`ccmp` **字形分/合**，按预设条件组合或拆分字形。

`kern` **字偶间距**，调整字与字之间的空间，让仿佛中间有空格的“A V”靠近为“AV”。

> 以上特性一般浏览器无需设置默认开启。以下特性需要软件支持和开启设置。目前各大浏览器应该都支持，[在网页CSS里添加相应代码即可](https://developer.mozilla.org/zh-CN/docs/Web/CSS/CSS_Fonts/OpenType_fonts_guide "OpenType字体特性指南 - CSS | MDN")。

`fwid` **全角宽度**，本字体用于将ASCII符号（即你关闭输入法直接按键盘输出的英文及标点）替换成全角的。

`pwid` **比例宽度**，是`fwid`的逆向操作，比如把“５１４”字形替换成“514”。

`salt` **样式替换**，用于替换字的写法。本字体这些汉字拥有变体，支持的软件可以启用之。为了方便过时软件，也可以从私用区等复制：儿(康熙部首:⼉)、元`u5143`(`uE143`)、叽`u53FD`(`uE3FD`)、无(康熙部首:⽆)、小(罕见字：𡭔)

`zero` **斜杠零**，将`0`替换成有斜杠的，形如`∅`，这样就可以区分o了。

为免误会顺带一提：字体特性只会改变字形，字码当然不变。

### 那么这些特性有什么用呢？
利用`calt`，在字体发现2个西文标点“…”相遇时（……，一般与西文A的底部基线对齐），自动替换为与汉字居中的“⋯”，形成中文省略号。在字体发现与西文基线对齐的冒号“:”被数字或数学符号夹在中间时，会替换成与数字居中对齐的比号“∶”。分号“;”也可以。
> 请参见我2019年的文章：[修改与自制字体：更好地显示时间/比分](https://www.bilibili.com/read/cv4146730)

利用`ccmp`，在字体发现有且仅有2个“—”相遇时（——），自动合并为一个“⸺”中间相连左右不顶格的破折号，看着似乎和中文省略号差不多？但是`ccmp`能合又能分，在多于2个“—”的情况下又会拆开，避免出现“⸺ —”这种断半边的难堪情况。
> 请参见我2020年的文章：[——若破折号不在统一码中该怎么办……](https://www.bilibili.com/read/cv8280047#reply8280047)

所以，这是个**Font Game**。

### 但我家软件也不支持这些特性😣
其实你可以从上文直接复制替换后的符号，粘贴到你的软件里。

## 包含汉字，但只包含一点点
至少支持这么些字：金雲丶为主儿兀刂剑冖凵及大天口叮叽合啪噗饴小丨丫中亅事丸丿乀九一丁七丅三下不无八六二于云五亖元几力个人亻什体依便化全十讠谈艹艺辶造干开异宀实女形屎扌打托抛拍捡氵汁汗海添纟给绵坨〇囗国圈木本案日智球慧曰百钅镀毒画米答蛇里量辩足𡭔𠷡の

以及答辩特有的共用字形（没时间做了，以后补）：的=の，屎=💩（💩上的表情改成😑了），四=亖，圈=⭕，拳=👊=〇，□=口，π=兀。因为共用字形的关系，如果你看见字体软件报告本字体**包含2万汉字**，那不必奇怪。

还支持其它一些绘文字，如：👐

顺带，本字体的logo在`uF8FF`()

未来会尽量补充汉字，你可以要求我优先做急用汉字乃至不是字的符号。咦？你会制作字体？这是开源字体，欢迎你来加字。

## 已知问题
过于答辩。具体的明天再写。

## 未来计划
修正已知问题。扩展可变轴。

## 致谢
- `kern`主要是**玊玉**帮忙写的。

既然看到这，也可以在[论坛][disc]闲聊。源文件也在那边。

## 支持声明 | Support & Disclaimer
由于是免费发布的，我对字体不作任何保证，不承担任何责任，无法提供商业级技术支持，但我有兴趣听取在我能力范围内的意见并尝试解决问题，可[在此向我反馈][isss]。（As this font is distributed at no cost, I am unable to provide a commercial level of personal technical support. I am interested in hearing from you, however, and will try to resolve problems that are reported to me. You can [send feedback to me here][isss].）

<p align="right">（本页出现的“我”均为<strong>綿雲飴里</strong>，<a href="https://afdian.net/@FairyFloss">向我打赏或约稿请点这~</a>）</p>

[isss]: ../../issues
[disc]: ../../discussions
