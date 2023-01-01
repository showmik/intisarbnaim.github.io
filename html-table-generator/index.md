# HTML Table Generator


**HTML Table Generator** is a WPF application that takes user input and generates HTML table code, making the process much easier.

## Backstory

I was working on an ebook file that I planned to read on my Kindle. The file had numerous Japanese dialogues and vocabularies that needed to be turned into an HTML table for the kindle to display properly.
I also had to use HTML [ruby](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ruby) syntax to ensure that it supported Furigana.

Coding this by hand was very tedious and close to impossible. So, I decided to make a tool that could automate the process. The HTML Table Generator is the result of that, along with another tool, the **[Furigana Tool](https://intisarbnaim.com/furigana-tool/)**.

## How to Use

{{< image src="/images/DialogueFromGenki.png" alt="A Dialogue from Genki" width="550">}}

Suppose the case, this dialogue, which is from the Japanese textbook *[Genki](https://en.wikipedia.org/wiki/Genki:_An_Integrated_Course_in_Elementary_Japanese)*, needed to be included in an ebook file so that the kindle could read it properly.

Formatting it into an HTML table would do the job and the code (excluding Furigana and styling) would look something like this:

``` html
<table>
    <tr>
       <td>だけし:<br/>Takeshi</td>
       <td>こんにちは。きむら たけしです。<br/>Konnichiwa. Kimura Takeshi desu.</td>
    </tr>
    <tr>
       <td>メアリー:<br/>Mearii</td>
       <td>メアりー・ハートです。あのう、りゅうがくせいですか。<br/>Mearii Haato desu. Anoo, ryuugakusee desu ka.</td>
    </tr>
    <tr>
       <td>だけし:<br/>Takeshi</td>
       <td>いいえ、にほんじんです。<br/>iie, nihonjin desu.</td>
    </tr>
    <tr>
       <td>メアリー:<br/>Mearii</td>
       <td>そうですか。なんねんせいですか。<br/>Soo desu ka. Nannensee desu ka.</td>
    </tr>
    <tr>
       <td>だけし:<br/>Takeshi</td>
       <td>よねんせいです。<br/>Yonensee desu.</td>
    </tr>
</table>

```
<br>

To do the same with this **HTML Table Generator**:

* First, input how many rows and columns you need. In this case, It is two columns and five rows. Also check on the romaji support check box and then click on **Generate**.

	{{< image src="/images/AppInterface01-table-generator.png" width="280" alt="AppInterface01" >}}
  
* It will generate a new window containing input text boxes corresponding to the number of rows and columns you entered. Fill up these boxes with proper input and then click **Run**.
  
	{{< image src="/images/AppInterface02-table-generator.png" width="550" alt="AppInterface02" >}}
  
* It will generate another window with the final table code. You can copy the whole thing by clicking on **Copy**. 

	{{< image src="/images/AppInterface03-table-generator.png" width="550" alt="AppInterface03">}}

* After adding some style, it looks something like this:

	{{< image src="/images/kindle-table.jpg" width="400" alt="kindle">}}
	
## Download

> {{<link href="https://github.com/showmik/html-table-generator/releases/tag/1.0.0.3" content="HTML Table Generator 1.0.0.3">}}

