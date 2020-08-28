## HTML Challenges

**1. Render your first h1!**

_Developer notes: We do want to have our own text editor in the app to achieve this_

```
HTML
<h1> Hello world! </h1>
```
**2. Quiz: The anatomy of a tag**

_Developer notes: Use the diagram below to create a quiz_

<img src="https://i.ibb.co/GvBbL3p/quiz.png" alt="quiz" border="0">

- Where is the opening tag? Answer: A. Show an explaination about the `< >` in most cases representing an opening tag
- Where is the closing tag? Answer: C. Show an explaination about the importance of `</ >` when closing a tag
- Where do you see camelCase? Answer: A & C. Show the examples of camelCase with multiple words.
- Which section will be displayed as a string on your web page? Answer: B.

**3. Quiz: The anatomy of the HTML boiler plate**

<img src="https://i.ibb.co/CB76VxC/Screen-Shot-2020-04-07-at-10-37-08-AM.png" alt="Screen-Shot-2020-04-07-at-10-37-08-AM" border="0">

- Where do you put the content the user will see on the page? Answer: D
- What tag houses _all_ of the HTML code you will write? Answer: A
- Which tag holds the information that will be displayed in the tab of the browser? Answer: C
- Where does all of the metadata (such as fonts, links to stylesheets, etc.) live? Answer: B

**4. Practice with attributes**

- Create your first link! Write code that will link a user to the wikipedia site for Cholula hot sauce

_Developer notes: solution below_
```
<a href="https://en.wikipedia.org/wiki/Cholula_Hot_Sauce">More about Cholula!</a>
```
_Developer note: you can check their solution by ensuring they have the same opening and closing tags as above. The inner HTML that they submit is arbitrary_

- Change the font colors below. First paragraph yellow, second paragraph blue, third paragraph red.
```
<p>Yellow is a star, yellow is the sun, yellow is the moon when the day is done</p>
<p>Blue is the ocean, blue is the sky, blue is the berries i put in my pie</p>
<p>Red is an apple, red is a cherry, red is a rose, and a ripe strawberry</p>
```

_Developer notes: solution below_

<img src="https://i.ibb.co/z8n88F1/Screen-Shot-2020-04-08-at-11-40-58-AM.png" alt="Screen-Shot-2020-04-08-at-11-40-58-AM" border="0">

```
<p style="color:yellow">Yellow is a star, yellow is the sun, yellow is the moon when the day is done</p>
<p style="color:blue">Blue is the ocean, blue is the sky, blue is the berries i put in my pie</p>
<p style="color:red">Red is an apple, red is a cherry, red is a rose, and a ripe strawberry</p>
```

**5. Table Challenge**

Code the table below. Hint! You will need to do a little bit of research on `<th>` instead of `<td>`:

<img src="https://i.ibb.co/tm0kdJd/Screen-Shot-2020-04-08-at-10-44-31-AM.png" alt="Screen-Shot-2020-04-08-at-10-44-31-AM" border="0">

_Developer notes: solution below_

```
<table border=1>
   <tr>
     <th>First Name</th>
     <th>Last Name</th>
     <th>Email</th>
   </tr>
   <tr>
     <td>Ricky</td>
     <td>Pickle</td>
     <td>ricky@myname.com</td>
   </tr>
   <tr>
     <td>Jax</td>
     <td>Lewis</td>
     <td>jax@myname.com</td>
   </tr>
</table>
```

**6. List Challenge**

Create the code for a webpage that will display the following recipe for simple cookies:

<img src="https://i.ibb.co/NrKvBsP/Screen-Shot-2020-04-09-at-11-10-46-AM.png" alt="Screen-Shot-2020-04-09-at-11-10-46-AM" border="0">

_Developer notes: solution below_

```
<ul>
  <li>Easy cookies!
    <ol>
      <li>Cookie mix</li>
      <li>Oil</li>
      <li>Water</li>
      <li>Eggs</li>
    </ol>
  </li>
</ul>
```

<a href="https://github.com/rachaelstanislaw/learn-pre-work/blob/master/HTML/html_lectures.md">Back to lectures</a>

<a href="https://github.com/rachaelstanislaw/learn-pre-work">Back to Table of Contents</a>
