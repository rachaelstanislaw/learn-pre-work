# CSS Lectures #

## Intro to CSS

**1. What's CSS?**

CSS, or Cascading Stylesheets, hold all the code that makes your webpage beautiful! If HTML is the skeleton and JavaScript is the muscular system, CSS is the skin! It is the outer appearance of our program. The following are some really beautiful web pages:

<img src="/assets/woven.gif">

- <a href="https://wovenmagazine.com">Woven Magazine</a>


<img src="/assets/amanda.gif">

- <a href="https://amandamartocchio.com/">Amanda Martocchio Architecture</a>


<img src="/assets/mikiya.gif">

- <a href="https://www.mikiyakobayashi.com/">Mikiya Kobayashi</a>


<img src="/assets/planet1.gif">

- <a href="https://www.onepercentfortheplanet.org/issues">1% For the Planet</a>


<img src="/assets/welcom.gif">

- <a href="https://www.franshalsmuseum.nl/nl/?gclid=EAIaIQobChMIgcWyzbLm6AIVtz6tBh3v0gr1EAAYAiAAEgKRWfD_BwE">Frans Hals Museum</a>


You can be as creative as you want with CSS, the sky is the limit. But first, let's start with the basics.

**2. CSS Syntax**

The syntax for a CSS file is as follows:

```css
body {                          /* A reference to the section you are styling followed by opening brace */
  background-color: #fff88f;    /* Styling written in key:value pairs, followed by a semicolon */
  color: pink                   
}                               /* Closing brace */
```
Here we are saying, "Every element in the `body` tag will have a yellow background color and pink font color." But what the heck is a `key:value` pair?? A _key:value_ pair in CSS code is a protected keyword (such as `color`, which represents font color) followed by a colon, and the value you'd like to apply (in this case, the protected color word `pink`).

Like HTML, there are a ton of styling referneces to use in your key:value pairs and they do not need to be memorized. Here's a list of them!

<a href="https://www.w3schools.com/cssref/">CSS Styling References</a>

Don't worry too much on the content of the CSS styling here. Just know that this basic syntax will apply to all of the elements that you end up styling. You can have as many lines of styling code as you'd like within the curly braces. 

**3. Styling HTML Classes and ID's**

Remember _HTML attributes_? The attributes _class_ and _id_ will be paramount when it comes to styling your webpages. 

- A _class_ attribute should be applied to multiple HTML elements that you'd like to all be styled to same way
- An _id_ attribute should be applied to a single HTML element that will have unique styling

For example:
```
<body>

  <h1>Fun with colors!</h1>

  <ul>
    <li class="purple">Purple 1</li>
    <li class="purple">Purple 2</li>
    <li class="purple">Purple 3</li>
    <li id="blue">Blue</li>
    <li id="orange">Orange</li>
    <li id="green">Green</li>
  </ul>

  <img src="woven.gif">

</body>
```
Inside of our `body` tag, we have a header followed by a list of colors. We want all of our purple items to have the same styling, but the rest of the colors should be more unique. For our purples, we have added the attribute `class` and assigned all of them the same thing `"puple"`. For blue, orange, and green, we have added the attribute `id` and assigned them unique values. An `id` value can only be used once in an HTML markup.

So what does the correlating CSS file look like then?

```css
.purple {
  color: purple
}


#blue {
  color: rgb(52, 81, 227)
}
#orange {
  color: #ffaf2e
}
#green {
  color: #45bf53
}
```

Here's the result:

<img src="https://i.ibb.co/bsYDyYj/Screen-Shot-2020-04-14-at-11-20-52-AM.png" alt="Screen-Shot-2020-04-14-at-11-20-52-AM" border="0">

Classes tags are targeted with the syntax above. A `.` then the name of the class. ID's are targeted with a `#` then the name of the ID. Notice how we have started to group all of the id's being targeted and separating them from the class. This helps us to stay organized. 

As we mentioned to earlier, in this example we are altering the font colors of these sections of HTML. There are multiple ways to refer to a color in CSS. 
- A protected word like purple, pink, or blue. While there are a lot of protected color words in CSS, the perfect color you are looking for may not be included and you'll probably need to be more specific. <a href="https://www.w3schools.com/cssref/css_colors.asp">CSS Colors</a>
- The hex code for a color
<img src="/assets/hex.gif">

- The RGB code for a color
<img src="/assets/rgb.gif">

**3. Style by Tag**

You can also style your HTML by its tag. Like in the example on CSS sytnax:

```css
body {                      
  background-color: #fff88f;     
  color: pink                   
}                               
```
We are targeting the entire `body` tag of our HTML markup. Maybe we want all of our paragraphs to have the same styling? It would be a waste of time to write out a class for each `p` tag if we can just target the tag itself:
```css
p {
  background-color: LemonChiffon;
  color: LightSeaGreen;
  border: 1px dotted RosyBrown;
  border-radius: 25px;
  font-size: 150%;
  text-align: center;
}                          
```
The code above would produce paragraphs that look like this:
<img src="https://i.ibb.co/s6m1fFw/Screen-Shot-2020-04-14-at-11-22-31-AM.png" alt="Screen-Shot-2020-04-14-at-11-22-31-AM" border="0">

<a href="https://github.com/rachaelstanislaw/learn-pre-work/blob/master/CSS/css_challenges.css">Go to challenges</a>

<a href="https://github.com/rachaelstanislaw/learn-pre-work">Back to Table of Contents</a>
