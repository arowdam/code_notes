# HTML intro

04/05/2023

## Page Structure

<img src="img/html_page_structure.png" alt= "The HTML page structure">
* peep the boxes 

<hr>
<br><br><br>

## __Elements__

<br>

### __Structural elements__

* `<!DOCTYPE html>`
    * declares document as an HTML 5 one
* `<html></html>`
    * contains all other elements
* `<head></head>`
    * holds meta data
* `<body></body>`
    * holds display info


### __Double tag elements__

`<h1> </h1>`
* header tag-> (gets pulled by search engines)

`<p> </p>` 
* paragraph tag-> always starts a new line, and gets a margin
    * defaults to giving info on a single line. Even if you type multiple

`<a> </a>` 
* link tag

`<pre> </pre>`
* shows preformatted text
    * If you [enter] multiple lines in a `<pre>`, they'll be preserved

### __Single tag elements__

`<br>` 
* line break tag
    * can be placed mid text tag

`<img>`
* image tag

`<hr>`
* horizontal rule-> separates content with a literal line
    * can be mid line like `<br>`

### <b>Text formatting tags</b>
    all of these are double tagged

* bold: `<b>`
    * <b> it's bold </b>
* important text: `<strong>`
    * <strong> is bold but important </strong>
* italics: `<i>`
    * <i> italics </i>
* emphasized text: `<em>`
    * <em> screen readers pronounce this was oomph </em>
* marked text: `<mark>`
    * <mark> highlit </mark>
* smaller text: `<small>`
    * <small> did you set the belt to wumbo? </small>
* deleted text: `<del>`
    * <del> struck through </del>
* inserted text: `<ins>`
    * <ins> underlined </ins>
* subscript text: `<sub>`
    * <sub> the reddit tag </sub>
* superscript text: `<sup>`
    * <sup> the skater tag </sup>

### __Citation and Quotation tags__

* block quotes: `<blockquote>`
    * <blockquote> just toss a ton of words into this block so that we can have a block of a quote </blockquote>
* short quotes: `<q>`
    * <q> i like trains </q>
* abbreviations: `<abbr>`
    * <p> the <abbr title="doctor"> dr.</abbr> was tired.</p>
* contact info: `<address>`
    * <address>
        Written by Damisi <br>
        Email at: email.gmail.com <br>
        this is italics <br>
        Finland
    </address>
* define title: `<cite>`
    * <p> <cite> the alchemist </cite> by some one. At some time </p>
* bi-directional override: `<bdo>`
    * <bdo dir="rtl"> This can only be beaten by racecar! </bdo>

<hr>
<br><br><br>

## __Element Attributes__

<br>

* attributes are always declared in the start tag.


`<a></a>`     
* href: to show a hyperlink
* `<a href=""></a>`

`<img>`
* src: links pic to element
* `<img src="">`
* also: alt="" width="", height=""
    * alt: shows text if the image doesn't load
    * width/height control the img size
    * `<img src="" alt=""...>`
* note -> links can be local (peep above) or absolute (web links)

`<p></p>`
* style: inline css 
* `<p style="color:blue;"></p>`
* title: mouse over title
* `<p title=""></p>`

`<html></html>`
* lang: sets file language
* `<html lang="en"></html>` 
    * sets to English

### Note: 
    You don't need to quote attribute values. But it is convention, you can single quote, double quote. Even no quote if you're crazy, though you can't have a space if that's the case.

* `<a href="pic/this">` 
* `<a href='pic/this'>`
* `<a href=pic/this>`
* ~~`<a href=pic this>`~~ 
    * no space with no quotes

<hr>
<br><br><br>

## _Styles_
    this is a tiny list of inline style attributes

<br>

### Syntax

* `<tag_name style= "property:value;">`



### Properties
* fonts
    * `style="font-family:font_name;"`
* font size
    * `style="font-size:00px;"`
* background color
    * `style="background-color: color_name;"`
* text color
    * `style="color:color_name;"`
* text alignment
    * `style="text-align:center;"`
    * can also be right/left etc.

<hr>
<br><br><br>

## Misc.

<br>

### Comment
* `<!---->` : that's how you make one