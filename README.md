Contents of the documentation

Steps | Title
------------ | -------------
1 | Preparing basic html structure
2 | Adding Scripts and Styles with <head></head> tags
3 | Adding basic styles 
4 | Design Section 1
5 | Design Section 2
6 | Design Section 3

![Image of Section1](https://github.com/iwilfried/Amp-Mag-Sound/blob/master/images/1.PNG)
![Image of Section1](https://github.com/iwilfried/Amp-Mag-Sound/blob/master/images/2.PNG)
### Step 1:Preparing basic html structure
```
<!doctype html>
<html AMP>
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
<link rel="canonical" href="https://sound-json.firebaseapp.com/">
<script custom-element="amp-font" src="https://cdn.ampproject.org/v0/amp-font-0.1.js" async></script>
<script custom-element="amp-sidebar" src="https://cdn.ampproject.org/v0/amp-sidebar-0.1.js" async></script>
<script custom-element="amp-accordion" src="https://cdn.ampproject.org/v0/amp-accordion-0.1.js" async></script>
<script src="https://cdn.ampproject.org/v0.js" async></script>

```

### Step 3:Adding basic styling within ```<style amp-custom></style>``` tags:
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
    margin-bottom:0.5rem;
    text-align: justify;
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
![Image of Section1](https://github.com/iwilfried/Amp-Mag-Sound/blob/master/images/header.PNG)

### Code:
```
 <header class="header">
    <nav>
      <div class="header_position">
        <a class="header_linkstyle" href="">
          <span class="header_drawcircle"></span>
          <span class="header_circletext">
            Read<br>Visit-Angkor<br>Blog</span>
          </span>
        </a>
      </div>
      <a href="" class="header_logo">
        <span class="header_logo">
          <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="180" height="55" viewBox="0 0 616 227" class="header_new_svg">
            <metadata><?xpacket begin="﻿" id="W5M0MpCehiHzreSzNTczkc9d"?>
              <x:xmpmeta xmlns:x="adobe:ns:meta/" x:xmptk="Adobe XMP Core 5.6-c142 79.160924, 2017/07/13-01:06:39        ">
              <rdf:RDF xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#">
              <rdf:Description rdf:about=""/>
            </rdf:RDF>
          </x:xmpmeta>                    
          <?xpacket end="w"?></metadata>
          <image width="612" height="223" xlink:href="data:img/png;base64,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"/>
        </svg>

      </span>
    </a>
    <ul class="ul_nav">
      <li class="li_nav">
        <a class="nav_link special_1" href="#" >
          Greetings
        </a>
      </li>
      <li class="li_nav">
        <a class="nav_link" href="#">
          Food
        </a>
      </li>
      <li class="li_nav">
        <a class="nav_link" href="#">
          Culture
        </a>
      </li>
      <li class="li_nav">
        <a class="nav_link" href="#">
          Lifestyle
        </a>
      </li>
    </ul>
 
    <button class="menu-burger" on='tap:sidebar1.toggle'>
      <span class="menu-burger_icon"></span>
    </button>

  </nav>
</header>

<amp-sidebar class="menu" layout="nodisplay" id="sidebar1">
  <div>
  <amp-img class="amp-close-image cross-btn"
  src="img/test.png"
  width="60"
  height="60"
  alt="close sidebar"
  on="tap:sidebar1.close"
  role="button"
  tabindex="0"></amp-img>
</div>
  <amp-accordion disable-session-states class="top_padding_20">
    <section>
      <h2 class="sidebarstyle padding_120 padding_15">Home</h2>
      <div class="side_menu_5">
        <ul>
          <li class="side_menu_3"><a href="#" class="side_menu_sub_link">Dialog</a></li>
          <li class="side_menu_3"><a href="#" class="side_menu_sub_link">Numbers</a></li>
        </ul>
      </div>
    </section>
    <section>
      <h2 class="sidebarstyle">Service</h2>
      <div class="side_menu_5">
        <ul>
          <li class="side_menu_3"><a href="#" class="side_menu_sub_link">How we Work</a></li>
        </ul>
      </div>
    </section>
    <section>
      <h2 class="sidebarstyle">Portfolio</h2>
      <div class="side_menu_5">
        <ul>
          <li class="side_menu_3"><a href="#" class="side_menu_sub_link">Find Answers Here</a></li>
        </ul>
      </div>
    </section>
    <section>
      <h2 class="sidebarstyle">Contact</h2>
      <div class="side_menu_5">
        <ul>
          <li class="side_menu_3"><a href="#" class="side_menu_sub_link">Article 1</a></li>
          <li class="side_menu_3"><a href="#" class="side_menu_sub_link">Article 2</a></li>
          <li class="side_menu_3"><a href="#" class="side_menu_sub_link">Article 3</a></li>
        </ul>
      </div>
    </section>
  </amp-accordion>

</amp-sidebar>


```
### Add classes within ```<style amp-custom></style>``` tags:
```
 .header{
    background-color:#e9eff1;
    border-bottom:0.0625rem solid #abc2c9;
    color:#121212;
    position:relative;
    max-width:37.5rem;
    margin:0 auto
  }
.header_position{
    left:-0.625rem;
    position:absolute;
    top:0
  }
  @media (min-width: 30em){
    .header_position{
      left:0
    }
  }
.header_linkstyle{
    color:#e9eff1
  }
.header_drawcircle{
    bottom:-0.75rem;
    left:0;
    overflow:hidden;
    position:absolute;
    right:0;
    top:0;
    -webkit-transition:-webkit-transform 250ms ease-out;
    transition:-webkit-transform 250ms ease-out;
    transition:transform 250ms ease-out;
    transition:transform 250ms ease-out, -webkit-transform 250ms ease-out;
    -webkit-transform-origin:top center;
    transform-origin:top center
  }
  .header_drawcircle:before{
    background:#121212;
    -webkit-border-radius:50%;
    border-radius:50%;
    bottom:0;
    content:'';
    display:block;
    left:0;
    padding-top:100%;
    position:absolute;
    right:0
  }
  .header_circletext{
    -webkit-box-sizing:border-box;
    -moz-box-sizing:border-box;
    box-sizing:border-box;
    display:block;
    padding:0.5625rem 1.25rem 0.1875rem;
    position:relative;
    font-size:0.8125rem;
    line-height:1.2;
    text-align:center;
    font-weight: bold;
  }
 .header_logo{
    display:-webkit-box;
    display:-webkit-flex;
    display:-ms-flexbox;
    display:flex;
    float:none;
    margin-left:auto;
    margin-bottom: 9px;
  }
  .ul_nav{
    height:1.875rem;
    margin:0;
    padding:0 0.625rem
  }
  @media (min-width: 30em){
    .ul_nav{
      padding-left:1.25rem;

    }
  }
 .li_nav{
    display:block;
    float:left;
    font-weight:500;
    font-family: Roboto;
  }
  .li_nav:first-child .nav_link{
    padding-left:0;
    
  }
  .li_nav:first-child .nav_link:before{
    content:none
  }
  .li_nav:nth-child(1){
    color:#c70000;
  }
  .li_nav:nth-child(2){
    color:#e05e00;
  }
  .li_nav:nth-child(3){
    color:#0084c6
  }
  .li_nav:nth-child(4){
    color:#bb3b80
  }
  .li_nav:nth-child(5){
    color:#bb3b80
  }
.nav_link{

    font-size:0.9375rem;
    font-weight:900;
    display:block;
    height:1.875rem;
    /*line-height:1;*/
    padding:0 0.55rem;
    position:relative;
    color:currentColor;
    cursor:pointer
  }
  @media (min-width: 22.5em){
    .nav_link{
     /* font-size:1rem*/
   }
 }
 .nav_link:before{
  content:'';
  display:block;
  left:0;
  bottom:0;
  position:absolute;
  border-left:0.0625rem solid #abc2c9;
  top:0.1875rem
}
.special_1
{
  border-bottom-color: #c70000;
  border-bottom-width: 3px;
  border-bottom-style: solid;
  display: inline;
  padding-bottom: 6px;
}
.menu-burger{
  background-color:#121212;
  top:1.5rem;
  -webkit-box-shadow:0 0 0 0.0625rem rgba(0,0,0,0.08);
  box-shadow:0 0 0 0.0625rem rgba(0,0,0,0.08);
  color:#e9eff1;
  cursor:pointer;
  height:2.5rem;
  min-width:2.5rem;
  position:absolute;
  border:0;
  -webkit-border-radius:50%;
  border-radius:50%;
  outline:none;
  right:0.3125rem
}
@media (min-width: 22.5em){
  .menu-burger{
    bottom:-0.375rem;
    height:3rem;
    min-width:3rem;
    top:auto
  }
}
@media (min-width: 30em){
  .menu-burger{
    right:3.1875rem
  }
}
.menu-burger_icon{
  margin-top:-0.0625rem;
  right:0;
  margin-left:auto;
  margin-right:auto
}
.menu-burger_icon,.menu-burger_icon:before,.menu-burger_icon:after{
  background-color:currentColor;
  content:'';
  height:0.125rem;
  left:0;
  position:absolute;
  width:1.25rem
}
.menu-burger_icon:before{
  top:-0.375rem
}
.menu-burger_icon:after{
  bottom:-0.375rem
}
.menu{
  background-color:#385574;
  color:white;
  width:80vw;
}
.menu div:first-of-type{
  overflow-y:scroll
}
.cross-btn
{
  float:right;
}
.top_padding_20 {
 margin-top: 20px;
}
.sidebarstyle
  {
    font-family:Roboto;
    text-align:center;
    background-color:#385574;
    color:white;
    border:none;
    font-weight: 100;
    font-weight:300;
    font-size:45px;
  }
  .padding_15 {
    padding-left: 15px;
}
.side_menu_5 {
 background-color:lightgray;
}
.side_menu_3 {
 list-style: none;
 margin-bottom: 8px;
}
.side_menu_sub_link{
 text-decoration: none;
 color:black;
 font-weight:100;
}
<style amp-boilerplate>body{-webkit-animation:-amp-start 8s steps(1,end) 0s 1 normal both;-moz-animation:-amp-start 8s steps(1,end) 0s 1 normal both;-ms-animation:-amp-start 8s steps(1,end) 0s 1 normal both;animation:-amp-start 8s steps(1,end) 0s 1 normal both}@-webkit-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@-moz-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@-ms-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@-o-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}</style><noscript><style amp-boilerplate>body{-webkit-animation:none;-moz-animation:none;-ms-animation:none;animation:none}</style></noscript>
```
# Step 5: Design Section 2

![Image of Section 2](https://github.com/iwilfried/Amp-Mag-Sound/blob/master/images/test.PNG)

### Code:
```
<div class="main-body">
  <div class="side-margins">
    <article id="article">
      <header>
        <div class="content__header">
          <div class="container">

            <div>
              <a href="#" class="side_menu_sub_link_1">Fashion</a>
              <a href="#" class="side_menu_sub_link_1">Food</a>
              <a href="#" class="side_menu_sub_link_1">Recipes</a>
              <a href="#" class="side_menu_sub_link_1">Love & Sex</a>
              <span [class]="visible ? 'show' : 'hide'" class="hide">
            <hr class="style1">
            
              <a href="#" class="side_menu_sub_link_1">Health & fitness</a>
              <a href="#" class="side_menu_sub_link_1">Home & garden</a>
              <a href="#" class="side_menu_sub_link_1">Women</a>
            
            <hr class="style1">
            
              <a href="#" class="side_menu_sub_link_1">Family</a>
              <a href="#" class="side_menu_sub_link_1">Travel</a>
              <a href="#" class="side_menu_sub_link_1">Money</a>
           
             </span>
               <a [class]="visible ? 'pink' : 'gray'" [text]="visible ? 'Less' : 'More'" on="tap:AMP.setState({visible: !visible})" class="side_menu_sub_link_1 gray">More</a>
            </div>

  
            <hr class="style1">
            <hr class="style1">
            <hr class="style1">
            <hr class="style1">

```
### Add External fontawesome stylesheet inside the ```<head></head>``` tags:
```
 <link href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet" integrity="sha384-wvfXpqpZZVQGK6TAh5PVlGOfQNHSoD2xbE+QkPxCAFlNEevoEH3Sl0sibVcOQVnN" crossorigin="anonymous">
 
```
### Add classes within ```<style amp-custom></style>``` tags:
```
.main-body{
    background:#ffffff;
    max-width:37.5rem;
    margin:0 auto;
    
    overflow-x:hidden;
  }
.side-margins
{
  margin-left: 0px;
}

.content__header{
  background-image:-webkit-repeating-linear-gradient(top, #dcdcdc, #dcdcdc 0.0625rem, transparent 0.0625rem, transparent 0.25rem);
  background-image:repeating-linear-gradient(to bottom, #dcdcdc, #dcdcdc 0.0625rem, transparent 0.0625rem, transparent 0.25rem);
  background-repeat:repeat-x;
  background-position:bottom;
  -webkit-background-size:0.0625rem 1.8125rem;
  background-size:0.0625rem 1.8125rem
}
.container
{
 padding-left:0.625rem;
 padding-right:0.625rem;
 -webkit-box-sizing:border-box;
 -moz-box-sizing:border-box;
 box-sizing:border-box
}
.side_menu_sub_link_1
{  
 padding-top: 10px;
 padding-left: 5px;
 display:inline-block;
 color:#000;
 font-family: Roboto;
 font-weight: bold;
}
hr.style1
{
  border-top: 1px solid #8c8b8b85;
  margin-bottom: -6px;
  margin-left: -11px;
  margin-right: -11px;
}
.pink
  {
    padding-top: 10px;
    padding-left: 10px;
    display: inline-block;
    font-family: Roboto;
    font-weight: bold;
    color:#bb3b80;
    text-decoration: none;
  }
  .gray
  {
    padding-top: 10px;
    padding-left: 10px;
    display: inline-block;
    font-family: Roboto;
    font-weight: bold;
    color:gray;
    text-decoration: none;
    
  }
  .gray:after
  {
    padding-top: 0px;
    padding-left: 3px;
    display: inline-block;
    color:gray;
    text-decoration: none !important;
    content:'\f107';
    font-family: Fontawesome; 
    font-size:20px; 
  }
```
# Step 6: Design Section 3

![Image of Section 2](https://github.com/iwilfried/Amp-Mag-Sound/blob/master/images/content.PNG)

### Code:
```
             <!-- sound card -->
            <div class="tabs-content">
              <amp-selector role="tablist" layout="container" class="" style="">

                <div role="tab" class="tabButton" selected option="a">Home</div>
                <div role="tabpanel" class="tabContent">
                  <div class="tint-block tint-block-top bg-body-1 home-card">
                    <div class="tint bg-red-light">

                      <div class="tint-position">
                        <h1 class="tint-header">
                          GREETINGS
                        </h1>
                        <span class="tint-span">
                          PRESENTING SAMPEAH IS A SIGN OF RESPECT AND POLITENESS.
                        </span>

                      </div>
                    </div>
                  </div>

                  <div class="content page-content-card page-content-card-bottom">
                    <h4 class="icon-heading uppercase ultrabold half-bottom">SAMPEAH</h4>
                    <p>
                      Sampeah is either used when you want to greet ( in KhmerL ->ផ៣បសវ joom reab sour) somebody or when you want to say goodbye (in Khmer:ផ៣បសវ ->joom reab lea). First of all, we need to place our both palms together like a lotus flower in front of our chest. Both are the formal way to gret and to say goodbye.
                      <amp-img alt="" src="img/s-07.png" height="145px"></amp-img>
                    </p>

                    <amp-list width="auto"
                    height="1790"
                    layout="fixed-height"
                    src="https://sound-json.firebaseapp.com/json/audio.json">
                    <template type="amp-mustache">
 
    <div id="widget" class="widget g-background-default g-shadow-inset">
      <p class="p1-text">{{title1}}</p>
      <p class="p2-text">{{title2}}</p>
      <p class="p3-text">{{title3}}</p>
      <p class="p4-text">{{title4}}</p>
      <div class="audio-container">
        <amp-audio  class="audio-player" width="auto" height="50" 
        src="{{url}}"  controlsList="nodownload" >
        <div fallback>
          <p>Your browser doesn’t support HTML5 audio</p>
        </div>
      </amp-audio>
    </div>
  </div>

</template>
</amp-list>
<div class="decoration"></div>
</div>      
</div>
</amp-selector>
</div>
<!-- sound card -->
</div>
</div>

</header>
</article>

</div>
</div>
```
### Add classes within ```<style amp-custom></style>``` tags:
```
 .tabs-content
  {
    padding-top:10px;
    margin:-10px;
  }

  .tabButton[selected] {
    display: none;
  }

  .tabButton {
    display: none;
  }
  .tabContent {
    display: none;
    width: 100%;
    order: 1; 
    border: 1px solid #ccc;
    padding: 5px;
    line-height: 24px;
  }

  .tabButton[selected]+.tabContent {
    display: block;
  }
.tint-block .tint{
    position:absolute;
    top:0px;
    left:0px;
    right:0px;
    bottom:0px;
    /* opacity:0.7;*/
    z-index:3;
    width:115%;
    height: 380px;
    background-image: linear-gradient( rgba(255, 0, 0, 0.49), rgba(195, 78, 63, 1) ),url(img/bg1.jpg);
    background-repeat:no-repeat;
    background-size:cover;
    background-position-x: -36px;
    background-position-y: -59px;

  }
  .tint-block{background-size:cover;}
.bg-body-1{background-position:150px right;}
  .tint-block-top{padding: 50px 0px 120px 0px;}
.home-card{
    padding: 260px 0px 120px 0px;
  }
.bg-red-light{background-color: #e74c3c; color:#FFFFFF;}
.tint-position
  {
    padding-top: 127px;padding-left: 17px;
  }
 .tint-header
  {
   font-family:Roboto;
   margin-top: -56px;
   margin-bottom: 12px;
   font-weight: 900;
 }

.tint-span
  {
    font-family: Roboto;
    font-size: 12px;
    float: left;
    width: 143px;
    font-weight: bold;
  }

  .page-content-card{
    font-family: Roboto;
    z-index: 97;
    position: relative;
    background-color: #fefefe;
    margin-left: 5px;
    margin-right: 16px;
    padding-top: 20px;
    padding-left: 10px;
    padding-right: 10px;
    /* border: solid 1px rgba(0,0,0,0.1); */
    margin-top: -169px;
    box-shadow: 0px 2px 5px 0px rgba(0,0,0,0.05);
  }

.uppercase{text-transform: uppercase;}
.ultrabold{font-weight:800;}

.half-bottom{margin-bottom: 3px;
  margin-top: -10px;}
p{
    line-height:20px; 
    font-weight:400; 
    color:#666666; 
    font-size:16px; 
    margin-bottom:15px;

  }
  .widget {
    width: 79%;
    background-repeat: no-repeat;
    background-position: 50%;
    background-size: 100px 60px;
    border-radius: 4px;
    border: 1px solid #e5e5e5;
    overflow: hidden;
    margin-bottom: 5%;
    margin-left: 8%;
  }
.g-background-default {
    background-color: #f5f5f5;
  }
  .g-shadow-inset {
    box-shadow: inset 0 0 0 1px hsla(0,0%,100%,.5);
  }

  .p1-text{
    font-size: 17px;
    padding: 20px 20px 0px;
    margin: auto;
    line-height: 1px;
  }
.audio-container{
    padding: 20px 20px;
  }
.decoration{
    height:1px; 
    background-color:rgba(0,0,0,0.1);
  }





```
### Add script and Roboto Font link for sound integration in the ```<head></head>``` section:
```
<script async custom-element="amp-audio" src="https://cdn.ampproject.org/v0/amp-audio-0.1.js"></script>
  <script async custom-element="amp-list" src="https://cdn.ampproject.org/v0/amp-list-0.1.js"></script>
  <script async custom-template="amp-mustache" src="https://cdn.ampproject.org/v0/amp-mustache-0.1.js"></script>
<link href='http://fonts.googleapis.com/css?family=Roboto:400,100,100italic,300,300italic,400italic,500,500italic,700,700italic,900italic,900' rel='stylesheet' type='text/css'>
```
