**1. ID vs. Class Color Activity**

Look at this HTML table:

```
<h1>My Pets:</h1>
<table border=1>
  <tr id="tableHeads">
    <th>Name</th>
    <th>Type</th>
    <th>Age</th>
  </tr>
  <tr class="dog">
    <td>Juneau</td>
    <td>Dog</td>
    <td>4</td>
  </tr>
  <tr class="dog">
    <td>Luna</td>
    <td>Dog</td>
    <td>3</td>
  </tr>
  <tr class="cat">
    <td>Lily</td>
    <td>Cat</td>
    <td>9</td>
  </tr>
  <tr class="dog">
    <td>Jema</td>
    <td>Dog</td>
    <td>6</td>
  </tr>
  <tr id="lizard">
    <td>Colette</td>
    <td>Lizard</td>
    <td>12</td>
  </tr>
  <tr class="cat">
    <td>Stu</td>
    <td>Cat</td>
    <td>1</td>
  </tr>
</table>
```

The styling we have so far for this table looks like this:

<img src="/assets/mypets.png">

We would like you to add CSS to make it look like this:

<img src="/assets/mypetsstyled.png">

Use the following color palette of protected CSS color names to fill in the blanks of the proceeding CSS code:

<img src="/assets/colorpalette.png">

```css
body {
  background-color: mintcream;
}
h1 {
  font-family: 'Pacifico', cursive;
  ___________: ___________;
}
table {
  font-family: 'Baloo Paaji 2', cursive;
  background-color: ____________;
}

__dog {
  ___________: ___________;
}
__cat {
  ___________: ___________;
}

__tableHeads {
  ___________: ___________;
}
__lizard {
  ___________: ___________;
}
```

_Developr notes: solution below:_

```css
body {
  background-color: mintcream;
}
h1 {
  font-family: 'Pacifico', cursive;
  color: olivedrab;
}
table {
  font-family: 'Baloo Paaji 2', cursive;
  background-color: papayawhip;
}

.dog {
  color: steelblue;
}
.cat {
  color: yellowgreen;
}

#tableHeads {
  color: orange;
}
#lizard {
  color: mediumvioletred;
}
```

<a href="https://github.com/rachaelstanislaw/learn-pre-work/blob/master/CSS/css_lectures.md">Go back to lectures</a>

<a href="https://github.com/rachaelstanislaw/learn-pre-work">Back to Table of Contents</a>
