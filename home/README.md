# Sample home.html page documentation


Contents of the documentation

Steps | Title
------------ | -------------
1 | Preparing basic html structure
2 | Adding Scripts and Styles with <head></head> tags
3 | Adding basic styling to custom.css
4 | Design Section 1
5 | Design Section 2
6 | Design Section 3



### Step 1:Preparing basic html structure
```
<html>
<head>
<title> <!-- Give appropriate title to the page  --> </title>
<!-- Required scripts and styles -->
</head>
<body>
<!-- Page contents -->
</body>
</html>
```
### Step 2:Adding Scripts and Styles with ```<head></head>``` tags
```
<meta charset="utf-8">
<meta http-equiv="X-UA-Compatible" content="IE=Edge"/>
<meta name="viewport" content="width=device-width,minimum-scale=1,initial-scale=1">
<link rel="stylesheet" type="text/css" href="custom.css">
<script custom-element="amp-font" src="https://cdn.ampproject.org/v0/amp-font-0.1.js" async></script>
<script custom-element="amp-sidebar" src="https://cdn.ampproject.org/v0/amp-sidebar-0.1.js" async></script>
<script custom-element="amp-accordion" src="https://cdn.ampproject.org/v0/amp-accordion-0.1.js" async></script>
<script src="https://cdn.ampproject.org/v0.js" async></script>

```

### Step 3:Adding basic styling to custom.css
```
html{
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased
}
body{
    font-family:Georgia, serif;
    font-size:100%;
    line-height:1.5;
    color:#121212;
    background:rgba(51,51,51,0.05)
}
.main-body{
    background:#ffffff;
    max-width:37.5rem;
    margin:0 auto;
    
    overflow-x:hidden;
}
html,body{
    text-rendering:optimizeSpeed
}
h1,h2,h3,h4,h5,h6{
    margin:0
}
p{
    font-size:1rem;
    font-weight:300;
    margin-top:0;
    margin-bottom:0.5rem
}
h3{
    font-size:1rem;
    line-height:1.5rem;
    font-weight:normal;
    margin-bottom:0.4375rem
}


a{
    color:#005689;
    cursor:pointer;
    text-decoration:none
}
a:hover,a:focus{
    text-decoration:underline
}
a:active{
    color:#4bc6df;
    text-decoration:none
}

menu,ol,ul{
    padding:0;
    margin-left:1.5625rem
}
nav ul,nav ol{
    list-style:none;
    list-style-image:none
}

```
# Step 4: Design Section 1
![Image of Section1](https://github.com/iwilfried/AMP-MAG/blob/master/images/section1.PNG)







