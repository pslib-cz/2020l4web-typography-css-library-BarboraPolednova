# Typography CSS library
**Author:** *Barbora Polednová*
## Demo site
Link to **[demo](http://www.github.io)** site for preview.
## Dependecies
### CSS files & Scripts
```
 <link rel="stylesheet" href="./typography_style_format.css">
```
 This is the main CSS file, which includes typography and styling for the **html** tags. It needs to be placed in the head of your project.

 ```
 <link rel="stylesheet" href="./gallery_format.css">
 <script src="https://unpkg.com/smartphoto@1.1.0/js/smartphoto.min.js"></script>
 <link rel="stylesheet" href="https://unpkg.com/smartphoto@1.1.0/css/smartphoto.min.css" />
```
For **image formating** and **image gallery usage** this fragment has to be copied in head.

 ```
 <script>
    new SmartPhoto(".thumbnails figure a");
</script>
```
To make this whole thing work, this **scrpit** needs to be placed right **under the body** of your code.
## Implementation
#### Place the code as your head of your project:
```
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Typography template</title>
    <link rel="stylesheet" href="./typography_style_format.css">
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap"
        rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Fjalla+One&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="./author.css">
    <script src="https://unpkg.com/smartphoto@1.1.0/js/smartphoto.min.js"></script>
    <link rel="stylesheet" href="https://unpkg.com/smartphoto@1.1.0/css/smartphoto.min.css" />
    <link rel="stylesheet" href="./gallery_format.css">
</head>
```

#### Place the following script right under the body of your project:
 ```
 <script>
    new SmartPhoto(".thumbnails figure a");
</script>
```

#### For complete function of image gallery, the **html structure** for images must look as it follows:
*(the class **thumbnails** is required for **figure** and **img** tags)
 ```
 <div class="thumbnails">
                <figure>
                    <a href="./images/sindy-sussengut-UqktoFudIOw-unsplash.jpg">
                        <img src="./images/sindy-sussengut-UqktoFudIOw-unsplash.jpg" alt="img caption" />
                        <div>
                            <p>Image caption 2</p>
                        </div>
                    </a>
                </figure>
            </div>
```
## Usage
A minimalist CSS Typography Library for online blog usage with images and simple interactive image gallery, based on styling HTML tags, such as:
* h1, h2, h3, h4, h5, h6
* p
* strong, b, emphasis, i
* a 
* ul/ol lists
* tables and table data
  * table
  * th
  * td
* code fragments
  * code
  * pre
* quoting and citation
  * blockquote
  * cite
  *headers & footers of citation
* images
  * figure
## Components
### Main header of page
```
 <header class="author_introduction">
        <h1 class="titulek">Typography Template</h1>
        <p class="author"><strong>Author:</strong> Barbora Polednová</p>
        <p class="date"><strong>Date:</strong> 25.09.2020</p>
    </header>
    <br>
```

### Header of article
```
<main>
    <article>
         <header>
            <h1>This is h1 heading</h1>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ea quibusdam placeat quidem rerum, corporis
                    sequi cupiditate id velit ullam quas reprehenderit iste, aliquid laborum odio dolores nulla,
                    explicabon,des oq
                    in unde?</p>
        </header>
    </article>
</main>
```

### Image in article
```
<article>
     <div class="thumbnails">
         <figure>
             <a href="./../image.jpg">
             <img src="./../image.jpg" alt="img caption" />
                 <div>
                    <p>Image caption 1</p>
                 </div>
             </a>
         </figure>
     </div>
</article>
```

### Lists in article
```
<article>
    <h3>This is ordered list</h3>
        <ol>
            <li>list item</li>
            <li>list item</li>
            <li>list item</li>
        </ol>
        <ol>
            <ol>
                <li>list item</li>
            </ol>
            <li>list item</li>
            <li>list item</li>
        </ol>
</article>
```

### Citation in article
```
<article>
    <h3>This is how quoting and citing looks like</h3>
        <blockquote>
            <h5>Heading of a cite</h5>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt, sequi esse! Illum impedit ipsam
                    voluptas nobis fugiat ut reprehenderit minima repudiandae, recusandae earum sequi, sint dolore unde
                    quisquam aspernatur ducimus.</p>
            <footer>- Lorem citation, 2020</footer>
        </blockquote>
</article>
```

### Table in article
```
<article>
    <table>
        <thead>
            <tr>
                <th>First Name</th>
                <th>Surname</th>
                <th>Age</th>
                <th>Gender</th>
                <th>Known For</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Oprah</td>
                <td>Winfrey</td>
                <td>66</td>
                <td>Female</td>
                <td>television production, acting, talk show hosting</td>
            </tr>
            <tr>
                <td>Morgan</td>
                <td>Freeman</td>
                <td>83</td>
                <td>Male</td>
                <td>acting, directing, narrating</td>
            </tr>
        </tbody>
    </table>
</article>
```

### Code fragment in article
```
<article>
    <pre><code>
        .thumbnails figure.info a:hover::before {
            color: white;
            background-color: gray;
        }
                
        img, figure > a, figure {
            /* width: 80%; */
            width: 50em;
            margin: auto;
        }                
    </code></pre>
</article>
```

### Footer
```
<article>
    <footer>
        <p>Created by <a href="index.html">Barbora Polednová</a> for WEB | Autumn 2020 | ©</p>
    </footer>
</article>
```
