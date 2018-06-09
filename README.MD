html & css tutorial
https://www.youtube.com/watch?v=y3UH2gAhwPI

https://www.youtube.com/user/thenewboston

http://www.w3school.com.cn/tags/tag_doctype.asp

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
### bold
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

## Lists (Bullet points)
```
<ul> <!--unordered list-->
    <li>bullet point 1</li>
    <li>bullet point 2</li>
    <li>bullet point 3</li>
</ul>

<ol> <!--ordered list-->
    <li>bullet point 1</li>
    <li>bullet point 2</li>
    <li>bullet point 3</li>
</ol>
```
## Span to affect part of text
```
<p> <span>Chunyu meetings</span> locally Chunyu meetings locallyChunyu meetings locallyChunyu meetings locallyChunyu meetings locally
            Chunyu meetings locallyChunyu meetings locally</p>
```


# CSS
must be at head
```
    <head>
        <!--css style must be at head-->
        <style type="text/css"> 
            p {
                color: rgb(223, 75, 30);
               font-family:Arial;
               line-height: 170%;
               } 
        </style><!-- p tage become new color-->
        <title>
            first web title
        </title>
    </head>
```

## css bold and iterlisize
```
    ul{
        font-weight:bold;
    }
    ol{
        font-style: italic;
    }
```

## text location
center
```
h1{
    color: orangered;
    text-align:center;
}
```

indent
```
p {
    color: rgb(223, 75, 30);
    font-family:Arial;
    line-height: 170%;
    text-indent: 25px;
    } 
```

## background color
```
        <style type="text/css">
            body{
                background-color: rgb(100,100,100);
                color:white; <!-- change all color except the one menully changed in HTML-->
            } 
        </style>
```
## backgroud image
```
<style type="text/css">
body{
        background-image: url(la.jpg);

        background-repeat: no-repeat;
        background-repeat: repeat-x;
        /* shift 30px to the right 60px down */
        background-position: 60px 100px;
        background-position: 50% 50%;
    }
</style>
```

## text paddings
```
            h1{
                color: orangered;
                text-align:center;
                /* padding background color */
                background-color: pink; 
                padding:20px;
                padding-bottom:70px;
            }
```
## border
```
        border-color:aquamarine;
        border-width: 5px;
        border-style: groove;
        border-top-style: inherit;
```
# Style sheet
in folder create .css file

then in every page of HTML's head out side style tag
```
<link rel="stylesheet" type = "text/css" href="filename.css"/>
```

