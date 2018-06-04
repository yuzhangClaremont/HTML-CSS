html & css tutorial
https://www.youtube.com/watch?v=y3UH2gAhwPI

https://www.youtube.com/user/thenewboston

# tags
<p> praragraph
<img> image
<!doctype html> tell browser what type of doc looking at 
<!-- a comment of start of this file -->

# head: where the browser info, titles

```
    <head>
        <title>
            first web title
        </title>
    </head>
```

# body: contents
```
    <body>
        i am the body
    </body>
```
## header title
h1>h2>h3....>h6
```
        <h6>
            NGOs
        </h6>
        search the NGOs near you
```
## paragraph
use <p></p> to make browser know new lines
```
        <p>  # new line
            recent news:

            PFLAG China
        </p>
        
        <p>the meetups near you</p> #not new line
        <p>Chunyu meetings locally</p>
```

or use line break
```
<br/>
```

and horizontal rule ```<hr/>```

## basic style
### bald
```
    <strong>PFLAG China</strong>
```
### italisize
```
    <em>recent news:</em>
```
## link
```
<a href="www.google.com">this is the link name</a>
<a href= "login.html">login </a> <!-- as long as in same folder-->
```
to creat the link in the same page as navigator

```
<p><a href = "#meetup">meetup</a></p>

...
<p><a name = "meetup"></a>the meetups near you</p>
```

link to email? 
```
<a href="mailto:yzhang@students.pitzer.edu">Email Yun</a>
```

## tooltips
```
<a href="http://www.pflag.org.cn/" title="LGBTQ NGO"><strong>PFLAG China</strong></a>
```

## image 
put in same folder as html
```
<a href="http://www.google.com"><img src = "PitzerHeadshot.jpg" height=/></a>
```
make the pic as a link too

resize image
```
<a href="http://www.google.com"><img src = "PitzerHeadshot.jpg" height="150
    "/></a>
```
## table
```
<table border=".1"> <!-- table line-->
    <tr></tr><!-- table row 1-->
        <th>name</td> <!-- table head column 1-->
        <th>next move</th>
    <tr></tr>
        <td>O</td> <!-- table data column 1-->
        <td>X</td>
</table>
```
