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
.margin-top-14
{
  margin-top:14px;
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
           <amp-img
  src="img/test.png"
  height="54" width="180" class="margin-top-14"></amp-img>
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
    text-decoration: none;
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
