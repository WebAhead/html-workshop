# Introduction to HTML

![html5 logo](https://user-images.githubusercontent.com/22002193/69446950-26f68b00-0d5e-11ea-96dd-eb217f407b56.jpg)

##  Contents

- Origin of HTML
- What is HTML?
  - Tag exploration
- HTML Structure
- How does HTML work?
- Fundamentals of HTML

## Origin of HTML

HTML - Hyper Text Markup Language is a language that was created by Tim Berners-Lee. Berners-Lee was putting together his first elementary browsing and authoring system for the Web and created a quick little hypertext language that would serve his purposes.

HTML was text-based and anyone could use any editor or word processor to create or convert documents for the Web. The developers started implementing new features in their browsers and started releasing advanced versions of HTML.

## What is HTML?

A markup language is a computer language that is used to apply layout and formatting conventions to a text document. Markup language makes the text more interactive and dynamic. It can turn text into images, tables, links, etc.

![html blocks](https://user-images.githubusercontent.com/22002193/69431669-dde40e00-0d40-11ea-9eca-eebebf65e58f.jpg)

HTML describes the structure of a Web page, this structure consists of a series of elements that tell the browser how to display the content.

HTML elements are represented by tags that label pieces of content such as "heading", "paragraph", "table", and so on...

Let's look at an example:
https://codepen.io/shiryz/pen/pooBWVW?editors=1000#0

## Task

Try it yourself, add the following line to the pen:

```html
<p>My car is very grumpy</p>
```

### Tag exploration

Let's explore our paragraph element a bit further:

![paragraph tag](https://user-images.githubusercontent.com/22002193/69439165-10950300-0d4f-11ea-99cf-3509e06cf8f9.png)

The main parts of our element are:

1. The opening tag - `<p>`: This consists of the name of the element (in this case, p which is short for paragraph), wrapped in opening and closing angle brackets `<>`. This states where the element begins or starts to take effect.
2. The closing tag - `</p>`: This is the same as the opening tag, except that it includes a forward slash before the element name `</>`. This states where the element ends. **if you do not include a closing tag** you will see erros and weird behaviour.
3. The content: This is the content of the element, which in this case is just text.
4. The element: The opening tag + the closing tag + the content equals the element.



### Task: Build a basic HTML page

- open your favourite editor and create a file called `my-first-page.html`
- type `html` in the page and press the `tab` key for the html5 option, this will automatically generate an html page for you.

The result should look like the following:

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title></title>
  </head>
  <body></body>
</html>
```

> We will explore all the tags later

- In the `<body>` tag add an `<h1>`

> Headings are defined with the `<h1>` to `<h6>` tags.

Your code should look something like this:

```html
<body>
  <h1>The Main Heading</h1>
</body>
```

- Right click on your html file and click on `open in browser` or `open with live server`, this should open the browser with the result of this file. You should see the h1 heading with `The Main Heading` on the page.


- Let's explore this a bit more, in the browser, open the inspector. You can do so by either pressing `f12` or right clicking on the page and then inspect or pressing `ctrl+shift+i`.

![](https://i.imgur.com/NF8zVdf.png)

  - You should be able to see the elements you created before (raw html), in the elements tab. You can edit/delete/add elements here like you did in your editor. _Notice_ that such changes will not be saved in your file and will only affect the browser, if you wish to save them then you will have to actually do it from the file itself.

  - In your editor, add a `div` tag to your file.

    > Find out more about [`div`](https://www.w3schools.com/tags/tag_div.asp)

- Add some more elements to your `div`, after each step refresh your browser to see the changes:
  - Add an `h2` tag that has the content `Subheading`. 
  - Add a `p` tag with the content `First paragraph`.
  - Add an [`img`](https://www.w3schools.com/tags/tag_img.asp) with the following image url as it's source or src -> `https://avatars1.githubusercontent.com/u/59686503?s=200&v=4`. 
     > **Important**: some html elements don't require a closing     tag, since nothing else can be put inside of them. Image is one such element.
     > 
     > More about [elements](https://developer.mozilla.org/en-US/docs/Glossary/Empty_element) that shouldn't be closed.
   - Add a second `div` (nested div).
   - In the second `div` add another `p` tag with the content `Second paragraph`.
 #### Comments are used to leave messages for other developers without affecting the code itself. To add a comment in an html file use the following syntax: `<!--` your comment goes in here `-->`, or press `ctrl + /`
  - Now add a comment to your file just below the main heading.
  - The result should look something like this (_only use this in case you are stuck or done_):
    <details>
     <summary>Code result</summary>
     
    ```html
    <div>
        <h1>The Main Heading</h1>
        <!-- My smart comment! -->
        <h2>Subheading</h2>
        <p>Paragraph</p>
        <img src="https://avatars1.githubusercontent.com/u/59686503?s=200&v=4" alt="Image">
        
        <div>
            <p>Second Paragraph</p>
        </div>
    </div>
    ```
    </details>
      <details>
      <summary>Result in browser</summary>
        <div>
          <h1>The Main Heading</h1>
          <h2>Subheading</h2>
          <p>Paragraph</p>
          <img src="https://avatars1.githubusercontent.com/u/59686503?s=200&v=4" alt="Image" alt="Image">
          <div>
            <p>Second Paragraph</p>
          </div>
        </div>
      </details>
### Task 2: Add more elements to your HTML page  

- Read about ways of creating [ordered](https://www.w3schools.com/tags/tag_ol.asp) and [unordered](https://www.w3schools.com/tags/tag_ul.asp) lists in html. In your file add two new `div`s and create one list in each of them. The lists should look like this:  

My to-do list:
1. (_insert your tasks here_) 
2.  
3.  

  Three people sitting next to me:  
  - (_insert their names_)
  -  
  -  

### Task 3 - Build a webpage to match the _mockup_
> In design, a mockup is  a mid- to high-fidelity representation of the product’s appearance that shows the basics of its functionality

Create a new HTML file (let's call it exercise.html) and try to create a webpage that will look exactly like this mockup (you can click on the image to open it in a new tab, if you'd like to see a larger version of it). Mind the instructions.
![](https://i.imgur.com/UsMwmXa.png)

##### Instructions  
- Use only HTML (even if you know CSS).
- You can choose another picture of Narhwal, this picture is just an example.
- The picture should be a link leading to an article about Narwhal (use whatever article you would like).
- The name _Mac's Mission_ should lead to https://www.macsmission.org/.  

<details>
     <summary>Hints</summary>  
  
  - Read about HTML [links](https://www.w3schools.com/html/html_links.asp)  
  
  - Read about HTML [tags](https://www.w3schools.com/tags/tag_hr.asp) (`<em>`, `<strong>`, `<hr>`, `<sub>`, `<s>`, `<br>` ) 
  
  - Read about HTML [forms](https://www.w3schools.com/html/html_forms.asp)  
  
  </details>
  
<details>
     <summary>See the solution (only when done!)</summary>  
  
  https://codepen.io/kira-abl/pen/mddYrjj?editors=1000
  
</details>

### Task 4 - Tables

In html a table is defined with the `<table>` tag. Each row is defined with the `<tr>` tag (**t**able **r**ow). A **t**able **h**eader is defined with the `<th>` tag. Each cell is defined with the `<td>` (**t**able **d**ata) tag.

* Read more about [tables](https://www.w3schools.com/html/html_tables.asp), and in a new .html file build a table that will have the following information in it:

![](https://i.imgur.com/u9jlXqU.png)

## Advanced HTML

  
#### HTML `<title>` Tag

The `<title>` tag is required in all HTML documents, it defines the title of the document and is used by search engines. This tag is always added between the `<head>` tags. Your document can only have one title.

* Add a title of your choice to your file. Don't forget to palce it between your `<head>` tags.  
  

#### HTML `<video>` Tag

The `<video>` tag specifies video, such as a movie clip.

```html
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
</video>
```
* Add a video to your file. If your user's browser doesn't support the `<video>` tag, show him a message saying he cannot view the video (Google is your friend). You can use this [MP4 file](http://mirrors.standaloneinstaller.com/video-sample/dolbycanyon.mp4). 


#### HTML `<script>` Tag

The <script> element either contains scripting statements, or it points to an external script file through the src attribute. Let's see a JavaScript function that is located between the `<script>` tags:  
  
  ```html
  <script>alert("Hello FACN8!");</script>
```

This function will show an alert window on your webpage. You will learn more about JavaScript later on, at this point it's important to understand that whatever is placed inside of `<script>` can be used to add interactivity to our pages. This tag is usually placed at the bottom of the `<body>` element. 

* Add a script showing an alert window to your page. If your user has scripts disabled in his browser, show him a message saying he cannot view scripts. 


### Additional Resources  
- HTML tutorial and references - [w3schools](https://www.w3schools.com/html/default.asp)  
- Another HTML [tutorial](https://www.codecademy.com/learn/learn-html)  
- HTML documentation on [MDN](https://developer.mozilla.org/en-US/docs/Web/HTML)  
- Introduction to HTML5, a free course on [Coursera](https://www.coursera.org/learn/html)
- HTML5 Coding Essentials and Best Practices, a free course on [edX](https://www.edx.org/course/html5-coding-essentials-and-best-practices)
- Arabic speaking free course on [Coursera](https://www.coursera.org/learn/website-coding-ar)
