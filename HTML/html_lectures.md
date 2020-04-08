## HTML Lecture Content

### Module 1: Intro to HTML Elements & Structure ###
**1. History of HTML**

Hyper Text Markup Language: structure and content of a page. Not the styling, not the functionality. Basically the skeleton.
In the early days of the internet, there was no standardized way of sending information and documents. Internet was mostly used for communication between colleges and universities as well as the military. If I wanted any formatting to happen with my document, I needed to be able to break that down to smaller pieces. Thus, HTML was made to handle it around 1989/1990.
Some headers, some things are bolded or important italicized, some bullet points, bigger and smaller text, etc
Eventually moved onto more broad uses. Remember myspace? Probably used HTML/CSS to edit your page

**2. What is a tag?**

HTML tags are the hidden keywords within a web page that define how your web browser must format and display the content. HTML tags typically fall into the following format: 

<img src="https://i.ibb.co/68xfFyB/Screen-Shot-2020-04-06-at-10-54-09-AM.png" alt="Screen-Shot-2020-04-06-at-10-54-09-AM" border="0">

There are hundreds of tags in HTML! You can look to MDN (Mozilla Developer Network) ar W3 Schools to see all of the tags available. Don't feel obligated by any means to memorize these. There are a few that you will use often (div, h1, p, etc.) and some that you will likely never use! At this point, just get familiar with the anatomy of a typical HTML tag.

<a href= "https://developer.mozilla.org/en-US/docs/Web/HTML/Element" target="_blank"> MDN HTML Tags </a>

**3. HTML Boiler Plate**

In your text editor (Atom of VS Code), if you type `HTML` and hit `tab`, the text editor will generate an HTML boiler plate. Let's break down what it is you're looking at in the boiler plate: 

<img src="https://i.ibb.co/HgYhW3h/Screen-Shot-2020-04-06-at-11-46-29-AM.png" alt="Screen-Shot-2020-04-06-at-11-46-29-AM" border="0">

It is important to understand what each tag in the boiler plate is responsible for! But for now, we will be working inside of the `body` tag.

*Developer Note: our in-app text editor will already be set to "HTML" where necessary. This is purely for their own knowledge. We are not spending a lot of time on the boiler plate, we just want to introduce it. Tags, indentation, and attributes are going to be a much larger chunk of the HTML pre-work.*

**4. What is an HTML attribute?**

HTML attributes are special words used inside the opening tag to control the element's behaviour. HTML attributes are a modifier of an HTML element type. For example, an `<a>` tag defines a hyperlink on your page. Techniaclly, the `<a>` tag is a complete tag on it's own. However, we need to add an `href` attribute to tell the hyperlink _where_ we want to go once it's clicked. An entire `<a>` tag will look something like this:

```
<a href="www.google.com">Click this link to go to Google!</a>
```

Above, we see the `<a>` tag, the `href` attribute inside of the _opening_ tag, a URL defined inside of the `href` attribute, some text for the user to click on, and a closing `</a>` tag! Voila!

Let's look at another example. An `<img>` tag will render an image. But the tag alone cannot do the job, we need to add an attribute! Here, we will add a `src` attribute which will include the URL of the image we want to render. 

```
<img src="www.image_source_goes_here.com">
```

Notice how the `<img>` tag doesn't close? That's becuase it is a self-closing tag! Since there is no _inner HTML_ in an image, this tag doesn't required a closing tag. To take a deeper dive on inner HTML, make sure you join Jumpstart!

One more example. A `<p>` tag represents a _paragraph_. You can change how the text in your paragraph looks by using a `style` attribute!

```
<p style="color:blue">I'm blue da ba dee da ba daa</p>
```

To recap, in all of our examples, the attribute is _modifying_ the HTML element in some way.

### Module 2: Tables ###
Let's use a `<table>` tag to build the table below!

<img src="https://i.ibb.co/946kd1H/Screen-Shot-2020-04-08-at-10-25-17-AM.png" alt="Screen-Shot-2020-04-08-at-10-25-17-AM" border="0">

1. First, we will need to code opening and closing `<table>` tags.

```
<table>
</table>
```

2. Next we will need to tell the table how many rows we would like. We do this by _nesting_ `<tr>` (table row) tags inside of the `<table>` tags. The table we hope to make will have three rows.

```
<table>
  <tr></tr>
  <tr></tr> 
  <tr></tr>
</table>
```

3. Now we need to tell the table how many columns we will need. We do this my _nesting_ `<td>` (table data) tags inside of the `<tr>` tags. Each `<td>` tag represents a cell in the row. We know we want the table to be three cells wide. First things first though, we need to stay organized since our table is getting more complicated! We are going to drop all of the closing `</tr>` tags down to a new line _before_ adding in our `<td>`'s. This will make it very clear to us where exactly each row ends. 

```
<table>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr> 
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
</table>
```

Look how clean that is! Each nested section is indented a single `tab` over and we can clearly see where all of our elements begin and end!

4. We probably want our table to contain some data right? Let's drop some text inside of the cells in the table. 

```
<table>
  <tr>
    <td>1</td>
    <td>2</td>
    <td>3</td>
  </tr>
  <tr>
    <td>4</td>
    <td>5</td>
    <td>6</td>
  </tr> 
  <tr>
    <td>7</td>
    <td>8</td>
    <td>9</td>
  </tr>
</table>
```

5. Lastly, we will want to add a border so that we can outline the table and all of it's cells. We do this by adding an _attribute_ to the opening `<table>` tag.

```
<table border=1>
  <tr>
    <td>1</td>
    <td>2</td>
    <td>3</td>
  </tr>
  <tr>
    <td>4</td>
    <td>5</td>
    <td>6</td>
  </tr> 
  <tr>
    <td>7</td>
    <td>8</td>
    <td>9</td>
  </tr>
</table>
```

Great work! Practice coding out the HTML table below:

<img src="https://i.ibb.co/tm0kdJd/Screen-Shot-2020-04-08-at-10-44-31-AM.png" alt="Screen-Shot-2020-04-08-at-10-44-31-AM" border="0">

_Developers note: this should take them to a challenge :)_

<a href="https://github.com/rachaelstanislaw/learn-pre-work/blob/master/HTML/html_challenges.md">Go to challenges</a>

<a href="https://github.com/rachaelstanislaw/learn-pre-work">Back to Table of Contents</a>
