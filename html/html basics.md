# HTML intro

04/05/2023

## Page Structure

<img src="img/html_page_structure.png" alt= "The HTML page structure">
* peep the boxes 

<br><br><br>
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

<br><br><br>
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
            
            note: if using width/height attributes, specs can be changed by a stylesheet. So if anything use inline style instead
            
            i.e.

            style="width:00px;height:00px;"

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

### **Note:** 
    You don't need to quote attribute values. But it is convention, you can single quote, double quote. Even no quote if you're crazy, though you can't have a space if that's the case.

* `<a href="pic/this">` 
* `<a href='pic/this'>`
* `<a href=pic/this>`
* ~~`<a href=pic this>`~~ 
    * no space with no quotes

<br><br><br>
<hr>
<br><br><br>

## **Links**

### **Gen**

* absolute path    
    * `<a href="https://website.com/"></a>`
* relative path
    * `<a href="/folder/website.html"></a>`

            Note: after opening an absolute path, the related pages can be linked relatively if they're stored in the same folder

* target attributes
    * `<a href="https://www.website.com/" target="_[target_attribute]">link text</a>`

            target attributes:
                * _self -> opens in current tab
                * _blank -> opens in new tab
                * _parent -> opens in parent frame
                * _top -> opens in full body of window
                    
                    though to be honest... I don't know the difference between _self/_parent/_top

* image as a link
    * place `<img>` tag within `<a>` tags
            
            <a href="https://www.website.com/">
                <img src="pic.png" alt="ex. pic">
            </a>

* link to email
    * `<a href="mailto:email@email.com">contact [____]</a>`
    * the magic is in the 'mailto:'
* button as a link
    * `<button onclick="document.location='default.asp'";>button name</button>`
    * `onclick` is java script
* link titles
    * `<a href= "https://www.website.com/" title="Open website">Website</a>`
    * gives extra info in the hover pop-up

### **Link CSS**

* Changing colors
    * link (unvisited link) - not underlined
    * visited - not underlined
    * hover - underlined
    * active - underlined

            <style>
                a:link{
                    color:color_name;
                    background-color:transparent;
                    text-decoration:none;
                }
                a:visited{
                    color:color_name;
                    background-color:transparent;
                    text-decoration:none;
                }
                a:hover{
                    color:color_name;
                    background-color:transparent;
                    text-decoration:none;
                }
                a:active{
                    color:color_name;
                    background-color:transparent;
                    text-decoration:none;
                }
            </style>

* Button styling
    * css 
    
            <style>
                a:link, a:visited {
                    background-color:color_name; 
                        /*sets block color*/
                    color:color_name; 
                        /*sets block text color*/
                    display:inline-block;
                        /*displays list items horizontally (not vertically)*/
                }
                a:hover,a:active{
                    background-color:color_name;
                        /*changes block color when hovering over it*/
                }
            </style>

### **Bookmarks or jump-to**
* set id attribute to make bookmark
    * `<h2 id="c2>Chapter 2</h>`
* link to said header
    * `<a href="#c4">To Chapter 2</a>`
* link a bookmark to a different page
    * `<a href="webpage.html#c4">To Chapter 2</a>`

<br><br><br>
<hr>
<br><br><br>

## _Styles aka **CSS**_    
<br>


### _Syntax_
* inline
    * within element tag
            
            `<tag_name style= "property:value;">`

* internal
    * within the `<head>` tag

            <head>
                <style>
                    p{
                        color:blue;
                    }
                </style>
            </head>

* external
    * in an external .css file

             p{
                color:blue;
            }
        
### _Link to external css_
* place link in `<head>` tag
* absolute path
    * `<link rel="stylesheet" href="https://website.com /css/styles.css">`
* relative path
    * `<link rel="stylesheet" href="/css/styles.css">`
    * **note:** if css file is in the same folder as the html file, the file name will suffice


### _Properties_
* background color
    * `background-color: color_name;`
* border
    * `border: 00px solid gray;`
* margin -> space outside border
    * `margin: 00px;`
* padding -> space between text and border
    * `padding: 00px 00px;`
    * pads space above/below
    * pads space left/right
* text alignment
    * `text-align:center;`
    * can also be right/left etc.
* text color
    * `color:color_name;`
* text fonts
    * `font-family:font_name;`
* text size
    * `font-size:00px;`

### _Colors_
    Supports: color names, or RGB, HEX, HSL, RGBA, or HSLA values.

#### _Attributes_
* background color
    * `style="background-color:blue;"`
* text color
    * `style="color:blue;"`
* border color
    * `style="border: 2px solid blue;"`

#### _RGB(A)_
* syntax: ###, ###, ###
* r- red, g- green, b- blue
    * on a scale of 0-255
* set the 3 values equal for gray
* the a stands for alpha which controls opacity

#### _HEX_
* syntax: #rrggbb
* rr- red, gg- green, bb- blue
    * starts at 00 -> 00-09, 0a-0f -> 10
    * after 9f -> a0-a9, aa-af -> b0
    * ends at ff
* set values equal for gray

#### _HSL(A)_
* syntax: hs1(hue, saturation, lightness)
* h- hue, s- saturation, l- lightness
    * h = degree on color wheel -> 0-360
    * s = percent (gray-color) -> 0-100%
    * l = percent (black-white) -> 0-100%
* the a stands for alpha which controls opacity


#### **Note:**
* color selection
    * blue -> color name
    * 0, 0, 255 -> RGB
    * 0000ff -> HEX
    * 240°, 100, 50 -> HSL

<br><br><br>
<hr>
<br><br><br>

## **`<Img>`**
**Attributes**

* width/height
    * `height:00px;width:00px;`
* Float images
    * direct images to to 'float' to x side of the text (right/left/etc.)
    * `float:left;`

**Image maps**

* add a `usemap="#.."` attribute
* add a `<map name="">`

* **shape types**
    * `rect`- x,y, x,y
    * <img src="img\img_sec\shape_rect.png" alt="rect shape"> 

            <area shape="rect" 
            coords="34,44,270,350" 
            href="laptop.htm">

            find opposite corners and rect tag fills the rest

    * `circle`- x,y radius
    * <img src="img\img_sec\shape_circ.png" alt="circle shape">

            <area shape="circle"
            coords="337,300, 44"
            href="coffee.htm">

            find center of circle and the radius

    * `poly`- x,y, x,y x,y...
    * <img src="img\img_sec\shape_poly.png">

            <area shape="poly"
            coords="140,121,181,116,204,160,204,222,191,270,140,329,85,355,58,352,37,322,40,259,103,161,128,147"
            href="croissant.htm">

            plot each and every point, and the poly shape fills it in

    * `default`- the entire file in `<img>` tag

            <img src="pic.png" alt="picture" usemap="#this_map">`
            `<map name="this_map">
                <area shape="rect" coords="0,0,100,100" alt="square" href="square.htm">
            </map>
    * javascript
        * onclick
            
                within area tag, you can add the `onclick` attribute and set it to a javascript function.

                <map name="map1">
                    <area shape="default" href="pic.png" onclick="a_function()">
                </map>

                <script>
                    function a_function() {
                        alert("post click response")
                    }

                Or any other action

**Background images**
  
* setting background image (via css)

        [element tag] {
            background-image: url('img_location.png');
        }

            note: to cover whole page, set to body tag

* related tags
    * background-repeat
        * by default, if the element is larger than the image, it'll repeat (either horizontally or vertically) till the space is filled.
    * background-size
        * cover -> fills the given element (open to repeating)
        * 100% 100% -> stretches height and width to fill element
    * background-attachment
        * fixed -> coupled with a body tag you can have a set background image that doesn't leave the screen when scrolling

            [tag naame] {
                background-repeat: no-repeat;
                background-attachment: fixed;
                background-size: cover;
            }

**`<picture >` element**

* holds multiple image sources
    * can be used to set the most suitable image for the device in regards to screen size or pixel density
    * and worst case you drop an auto width and even an `<img>` tag

            <picture>
                <source media="(min-width: 001px)" srcset="img.png">
                <source media="(min-width: 010px)" srcset="img2.png">
                <source media="(min-width: 100px)" srcset="img3.png">
                <img src="img4.png"> style="width:auto;">
            </picture>
    
<br><br><br>
<hr>
<br><br><br>

## **Tables**
* code example

<table>
    <tr>
        <th>column 1</th>
        <th>column 2</th>
        <th>column 3</th>
    </tr>
    <tr>
        <td>rand data1</td>
        <td>rand data2</td>
        <td>rand data3</td>
    </tr>
    <tr>
        <td>rand data4</td>
        <td>rand data5</td>
        <td>rand data6</td>
    </tr>
</table>
    

* code breakdown

        <body>
            <table>
                <tr> /*stands for table row*/
                    <th>column 1</th> /*stands for table header*/
                    <th>column 2</th>
                    <th>column 3</th>
                </tr>
                <tr>
                    <td>rand data1</td> /*stands for table data*/
                    <td>rand data2</td>
                    <td>rand data3</td>
                </tr>
                <tr>
                    <td>rand data1</td>
                    <td>rand data2</td>
                    <td>rand data3</td>
                </tr>
            </table>
        </body>

* extra tags within `<table>`
    
<style>
    table, th, td {
        border: 1px solid green;
        border-collapse: collapse;
        border-style: dotted;
    }
</style>

<table style="width: 90%">
    <tr>
        <th>tag</th>
        <th>desc.</th>
    </tr>
    <tr>
        <td>caption</td>
        <td>table caption</td>
    </tr>
    <tr>
        <td>colgroup</td>
        <td>specifies a group of column(s) for formatting</td>
    </tr>
    <tr>
        <td>col</td>
        <td>specifies properties for each column in a 'colgroup' element </td>
    </tr>
    <tr>
        <td>thead</td>
        <td>groups header content</td>
    </tr>
    <tr>
        <td>tbody</td>
        <td>groups body content</td>
    </tr>
    <tr>
        <td>tfoot</td>
        <td>groups footer content</td>
    </tr>
</table>

**Borders**

        table, th, td {
            border: 1px solid [color_name];
            border-collapse: collapse;
        }
            * first style sets border around said table and elements
            * second style makes it so that their isn't a double border around said elements
        th, td {
            background-color: [color_name];
            border-color: [color_name];
            border-style: dotted;
        }
            * styles only effect header and data cells, not the table border
            * first sets color within cells
            * second sets the color of the border
            * third can alter the style of the lines
                * values
                    * dotted / dashed / solid / double / groove / ridge / inset / outset / none / hidden
        
**Table sizes**

    table {
        width: 90%;
        height: 200px;
    }
        * sets the height and width of the table.
            * the same can be done to the individual th / td elements

**Table headers**

* horizontal headers
<table>
    <tr>
        <th>HorHead1</th>
        <th>HorHead2</th>
        <th>HorHead3</th>
    </tr>
    <tr>
        <td>rand data1</td>
        <td>rand data2</td>
        <td>rand data3</td>
    </tr>
    <tr>
        <td>rand data4</td>
        <td>rand data5</td>
        <td>rand data6</td>
    </tr>
</table>

* vertical headers
<table>
        <tr>
            <th>HorHead1</th>
            <td>rand data1</td>
            <td>rand data2</td>
        </tr>
        <tr>
            <th>HorHead2</th>
            <td>rand data3</td>
            <td>rand data4</td>
        </tr>
        <tr>
            <th>HorHead3</th>
            <td>rand data5</td>
            <td>rand data6</td>
        </tr>
    </table>

* alignment
    * peep instyle by the second heaader
<table>
        <tr>
            <th>HorHead1 and the jonts</th>
            <td>rand data1</td>
            <td>rand data2</td>
        </tr>
        <tr>
            <th style="text-align:right;">HorHead2</th>
            <td>rand data3</td>
            <td>rand data4</td>
        </tr>
        <tr>
            <th>HorHead3</th>
            <td>rand data5</td>
            <td>rand data6</td>
        </tr>
    </table>

* multi columns
    * via the colspan attribute
<table>
    <tr>
        <th colspan="2">DoubleHorHead1</th>
        <th>HorHead2</th>
    </tr>
    <tr>
        <td>rand data1</td>
        <td>rand data2</td>
        <td>rand data3</td>
    </tr>
    <tr>
        <td>rand data4</td>
        <td>rand data5</td>
        <td>rand data6</td>
    </tr>
</table>

* table captions (via element)
<table>
    <caption>Table caption</caption>
    <tr>
        <th>HorHead1</th>
        <th>HorHead2</th>
        <th>HorHead3</th>
    </tr>
    <tr>
        <td>rand data1</td>
        <td>rand data2</td>
        <td>rand data3</td>
    </tr>
    <tr>
        <td>rand data4</td>
        <td>rand data5</td>
        <td>rand data6</td>
    </tr>
</table>

<br><br><br>
<hr>
<br><br><br>

## **Misc**.

<br>

### **Comments**
* `<!---->` : that's how you make one

### **Favicon**

        <head>
            <link rel="icon" type="image/x-icon" href="/img/favicon.png">
        </head>

* sets favicon, i.e. the image in the tab bar.
    * supported image formats: ico/png/gif/jpeg/svg

### **Page title**

    <head>
        <title>Title name</title>
    </head>
* sets title, i.e. the text in the tab bar
    * important for being found by the search engine

