# Exam: HTML & CSS

### Getting Started
 - Fork this repository under your own account
 - Commit your progress frequently and with descriptive commit messages
 - All your answers and solutions should go in this repository

### What can I use?
 - You can use any resource online, but **please work individually**
 - Instead of copy-pasting your answers and solutions, write them in your own words.


# Tasks

## 1. Build a design (~90 minutes) [10 points]
Build the following profile cards according to the design provided.   
Follow the design as closely as possible.   
Commit an HTML and a CSS file to this repository.
![design](exercise-1.png)

### Assets
John Duck | Jane Duck | Pencil icon
--------- | --------- | -----------
![duck](duck.jpg) | ![duck](duck2.jpg) | ![pencil-icon](edit-icon.png)   

### Other data
  - Name font size: 28 pixels
  - Text size: 14 pixels
  - Font family: Arial, sans-serif

### Acceptance criteria
The task is accepted if:
  - The result follows design [2p]
  - The code follows style guide [1p]
  - The CSS & HTML are valid [1p]
  - The HTML considers semantic responsibilities [2p]
  - The code avoids code duplication [2p]
  - The CSS has meaningful and short selectors [2p]

Extra points for if:
  - the result is centered on the page [2p]


## 2. Understand code (~15 minutes) [2 points]
Read the following code snippet:   
What is the distance between the top-left corner of the document body and the yellow box?   
Give a detailed explanation below!   
Add your answer to this readme file, commit your changes to this repository.
```HTML
<!DOCTYPE html>
<html>
  <head>
    <style>
      body {
        padding: 0px;
        margin: 0px;
      }
      .foo {
        top: 20px;
        left: 20px;
        width: 100px;
        height: 100px;
        position: absolute;
        background: blue;
      }
      .bar {
        top: 20px;
        left: 20px;
        width: 30px;
        height: 30px;
        position: absolute;
        background: yellow;
      }
    </style>
  </head>
  <body>
    <div class="foo">
      <div class="bar"></div>
    </div>
  </body>
</html>
```
#### Your answer: The distance is 40px from the top and 40px from the left. The yellow box is the bar class, which has an absolute position. It means its top left corner is from 20px from its parent's top left corner. The yellow box's parent is the foo class div, which has also an absolute position, relative to its parent, which is the body. So foo's top-left corner in from 20px from the body's top-left corner. The distances add up, hence the 40px. None of the elements have border or margin, therefor no extra pixels needs to be added.


## 3. Explain concepts (~15 minutes) [4 points]
Add your answer to this readme file, commit your changes to this repository.


### Explain the difference between `display: block` and `display: inline` in CSS! What is `display: inline-block`?
#### Your answer: The display property controls how the element behaves. A block element by default takes up as much horizontal space as it can and as much vertical space as its content needs, though we can set its height and width. An inline element stays in line, does not break the text flow. Even if we apply padding or margin, it does not push the text out horizontally, only vertically. The inline-block combines the advantages of both: the element stays in line, but we can apply both width and height and it pushes the content away according to the settings.


### What is the difference between a `<section>` and an `<article>` element? Name one good example of using an `<article>`.
#### Your answer: A section can be used for thematic grouping of contents, it is good for styling purposes also. The content of an article could stand alone, it could be meaningful without the other content of the site. A good example of using <article> might be at the wikipedia site containing the actual information (for example the biography of Margaret Hamilton). Or at a blog a new post can be within article tags.
