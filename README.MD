html & css tutorial
https://www.youtube.com/watch?v=y3UH2gAhwPI

https://www.youtube.com/user/thenewboston

http://www.w3school.com.cn/tags/tag_doctype.asp

https://www.youtube.com/watch?v=VvB4gDYhcgo&list=PL46F0A159EC02DF82&index=39

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

max image size (or min size)
```
<style type="text/css">
    img {max-height: 200px;
        max-width:200px;}
</style>

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

## form
```
    <form>
        <!-- use name to differenentiate boxs -->
        <!-- maxlength limit text inputed
        value: the default text inside -->
        Username:<input type="text" name="username" size="30" maxlength="3" value="Enter your name"/>
        male:<input type="radio" name="sex" >
        female:<input type="radio" name="sex" value="female">
        <!-- male female has same name, so browser know in same group, so can only
        slect one -->
``` 

checkbox
```
        <p>select the food you want</p>

        Bacon <input type="checkbox" name="food" value="bacon">
        ham<input type="checkbox" name="food" value="ham">
        tuna <input type="checkbox" name="food" value="tuna">
```

dropbox
```
    <form>
        what do you want to do?
            <select name="activities">
                    <option value="guitar"> play guitar </option>
                    <option value="tennis"> play tennis </option>
                    <option value="swim"> go swimming </option>
                </select>
    </form>
```

text area
```
    <form>
        tell me yourself:
        <br/>
        <textarea name="bio" rows="4" cols="60">
            your bio
        </textarea>
    </form>
```

password and file upload
```
    <form>
        password:<input type="password" name="pw"/>
        <p>now submit a file</p>
        <input type ="file" name="userfile"/>
    </form>
```
you have to use javascript to upload multiple files 

submit
```
    <form action="dosomething" method="post">
   
        <br/>
        <input type="submit" value="submit the file"/>
        <!-- submit create a button, value is the text on it -->
    </form>
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
## position
absolute: free control from left top corner
relative: top, left relative from original position
outside box relative, inside box absolute
fix: element stay in same place when screening

# Style sheet
in folder create .css file

then in every page of HTML's head out side style tag
```
<link rel="stylesheet" type = "text/css" href="filename.css"/>
```

# post web site


# Javascript


# comments
```
// comments here
```

```
/*
multiline 
comments
*/
```

# basic statements

## print
```
document.write("something here");
```

## prompt
```
// question and default text
    var pie = prompt("Enter your name:","defalt text");
    document.write("hello ", pie);
```

## function
define and run
```
function funky(){
    alert("ouch")
}

funky();
```

button elicit function
```
<script type="text/javascript">
    document.write("javascript testing");

    function funky(){
    alert("ouch")
    }
</script>
<form>
    <input type="button" value = "botton text" onclick="funky()"/>
</form>
</body>
```
## if statement
```
        var apples = 34;
        var hotdog =53;

        if (apples == 34){
            document.write("it works");
        }
        else{

        }
```

and: &&
or: ||
## switch
```
var girl = "natalie"
switch(girl){
    case "natalie":
    document.write("hey natalie");
    break;
    case "ashley":
    document.write("hey ashley");
    break;
    default:
    document.write("default choice");
}
```
## for loop
```
for (x=0; x<3;x++){
    document.write(x+"<br/>hello<br/>");
}
```
do ... while loop
```
var x = 5;
do{
    document.write("<br/>"+x+"hello");
    x++;
}while(x<10);
```
# variable
```
var x =23;
```

strings
```
var s = "\"hello world\"";
document.write(s);
```
\ escape sign

```
var b = true;
document.write(b);

var n = null;
document.write(n);


```

# event handler

## onClick
```
<form>
    <!-- onClick is event handler, with javascript code inside, use single quote forstring -->
    <input type="button" value="touch me" onClick=
    "alert('hahahah');
    alert('hahahah x 2');"
    />
</form>
```

## onMouseOver
```
<a href="http://google.com" onMouseOver="alert('gametime');">google</a>
```
## onMouseOut
```
<a href="http://google.com" onMouseOut="alert('gametime');">google</a>
```

## onLoad
```
<body onLoad="alert('webpage finished loaded');">
</body>
```

## onUnload not working?
```
<body onUnload="alert('goodbye');">
```

# Object

string object
```
var tuna = "this is a tuna";
document.write("<br/>tuna length:"+tuna.length);
```

Constructor
```
<head>
    <script type="text/javascript">
    // person constructor function
        function person (name, age){
            this.names = name;
            this.Age = age;
        }

        var host = new person("Yun", 27);
    </script>

</head>
```

use object
```
<body onUnload="alert('goodbye');">
    
<script type="text/javascript">
    document.write(host.Age);
.
.
```

Object initializer, faster than constructor

in head script tag
```
 guest = {name:"David", age:26};
 ```

 methods
 ```
     <script type="text/javascript">
    // person constructor function
        function person (name, age){
            this.names = name;
            this.Age = age;
            // bornyear is function but no perameter
            this.bornYear = bornyear;

        }
    // person function return born year
        function bornyear(){
            var bornyear = 2018-this.Age;
            return bornyear;
        }

        var host = new person("Yun", 27);
```

use method
```
<body onUnload="alert('goodbye');">
    
<script type="text/javascript">
    document.write(host.bornYear()+"<br/>");
```

## Math obejct
```
 document.write(Math.E, "<br/>");
```
pi
```
Math.PI;
```

sqrt
```
Math.sqrt(n);
```

## Date object
grab current date and time

```
function printTime(){
    var now = new Date();
    var hours = now.getHours();
    var mins = now.getMinutes();
    var seconds = now.getSeconds();
    document.write(hours+":"+mins+':'+seconds+"<br/>");
}

// date object
function tuna(){
    document.write("tuna <br/>");
}
// run this function every 1000ms
setInterval("printTime()",1000);
```
# Form object, form validation and javascript
```
<form>
    username: <input type="text"/>
    password: <input type="password"/>
    <input type="submit" value="submit!"/>
</form>
<script type="text/javascript">
    document.write(document.forms.length, "<br/>");// 2 forms in forms array
    document.write(document.forms[1].length);// login form array has 3 elements
    var x = document.forms[1]
</script>
```
access form element
```
<form name="login">
    username: <input type="text" name="username"/>
    password: <input type="password" name="ppassword"/>
    <input type="submit" value="submit!"/>
</form>
<script type="text/javascript">
    document.write(document.forms.length, "<br/>");// 2 forms in forms array
    document.write(document.forms[1].length);// login form array has 3 elements
    var x = document.forms[1]
    var pw = document.forms[1].elements[1].name;// ppassword
    var usern = document.login.username.name;
    document.write(usern);
</script>c
```

## form validation
```
<!-- // form validation -->
<form name="yunsForum">
    <input type="checkbox" name="box"/>
    <input type="button" value ="press me" onClick="validator()">
</form>

<script type="text/javascript">
function validator(){
    // true if checked, false else
    if (document.yunsForum.box.checked){
        alert("you sure check");
    }
    else{
        alert("no you not checked yet");
    }
}
</script>
```

# Data structure

## Array
```
<script type="text/javascript">
    var people = new Array("name1","Mike","Amy");

    document.write(people[2])
```

```
    var things = new Array(3);
    things[0] = "kunming";

// size can be not fixed!!
    var a = new Array();
    a[0] = 0;
    a[13] =13;
    document.write(a[2], a[13]); // undefined, 13
```

array lenth
```
a.lenth
```

concatenate
```
a.concat(b)
```

array join to string
```
// join array to string
var string1 =  people.join('+');
document.write(string1,"<br/>");
```
//reverse array
```
    //reverse array
    people.reverse();
```
push
```
    people.push("1","2","3");
```

sort
number> upper head> lower head
```
    //sort in alphebet order
    people.sort();
```

pop out last element of array
```
    // pop out last element of array
    document.write(people.pop(),"<br/>",people,"<br/>");
```

## dictionary? associative array?
associative array
```
// dict? Associative Array
    var assoArray = new Array();
    assoArray["key1"] = "value1";
    assoArray["key2"] = "value2";
    document.write(assoArray["key2"], "<br/>");
```

