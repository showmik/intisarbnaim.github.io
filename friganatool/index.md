# Furigana Tool


# Furigana Tool

**Furigana Tool** automates the process of writing HTML code for Furigana with *[ruby](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ruby)* syntax. It uses a modified version of the **[Gem](https://github.com/helephant/Gem)** library and adds a User Interface to it.

This tool was intended to be used along with the **[HTML Table Generator](https://github.com/showmik/html-table-generator)** for one of my projects.

## The Ruby Syntax

> "A ruby annotation is a small extra text, attached to the main text to indicate the pronunciation or meaning of the corresponding characters. This kind of annotation is often used in Japanese publications." — W3Schools

For example, let's consider the word *Furigana*:

[![Furigana](https://github.com/showmik/furigana-tool/raw/master/Docs/Fu_ri_ga_na_Furigana_Example.png)](https://github.com/showmik/furigana-tool/blob/master/Docs/Fu_ri_ga_na_Furigana_Example.png)

To create something like this in HTML, we can write:

```
<ruby><rb>振</rb><rt>ふ</rt><rb>り</rb><rt></rt><rb>仮</rb><rt>が</rt><rb>名</rb><rt>な</rt></ruby>
```

And the result would be this:

> 振ふり仮が名な



Or the word *Dai ni kan (Volume 2)*:

[![DaiNiKan](https://github.com/showmik/furigana-tool/raw/master/Docs/Dai_ni_can_Furigana_Example.png)](https://github.com/showmik/furigana-tool/blob/master/Docs/Dai_ni_can_Furigana_Example.png)

HTML:

```
<ruby><rb>第</rb><rt>たい</rt><rb>2</rb><rt></rt><rb>巻</rb><rt>かん</rt></ruby>
```

Resul:

> 第たい2巻かん

## Using the Furigana Tool

As you can guess, it was very tedious for me to write HTML code every time I wanted to use Furigana. This tool made it a lot easier. Now I just need to input the Kanji and Furigana, and it generates the code for me.



[![App_Interfaxe](https://github.com/showmik/furigana-tool/raw/master/Docs/FuriganaToolInterface01.png)](https://github.com/showmik/furigana-tool/blob/master/Docs/FuriganaToolInterface01.png) [![App_Interfaxe](https://github.com/showmik/furigana-tool/raw/master/Docs/furigana_fool_interface_02.png)](https://github.com/showmik/furigana-tool/blob/master/Docs/furigana_fool_interface_02.png)

