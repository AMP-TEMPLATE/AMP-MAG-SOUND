AMP-MAG

|RULE                                                     	                      | DESCRIPTION                     	|
|-------------------------------------------------------------------------------------|----------------------------------------	|
| Start with the <!doctype html> doctype.                                             |  Standard for HTML.  	                | 
| Contain a top-level <html ⚡> tag <br />(<html amp> is accepted as well)            |  Identifies the page as AMP content.    |
| Contain <head> and <body> tags.                                                     | Optional in HTML but not in AMP.        |
| Contain a <meta charset="utf-8"> tag as the first child of their <head> tag    | Identifies the encoding for the page    |
| Contain a <script async <br>src="https://cdn.ampproject.org/v0.js"></script> tag<br> as the second child of their <head> tag.   | Includes and loads the AMP JS library.    |
|Contain a <link rel="canonical" <br>href="$SOME_URL"> tag inside their <head>  | Points to the regular HTML version of the AMP <br>  HTML document or to itself if no such HTML <br>version exists. Learn more in Make Your Page Discoverable.|
|Contain a <meta name="viewport" <br>content="width=device-width,minimum-scale=1"><br>tag inside their <head> tag. It's also recommended to include initial-scale=1 | Specifies a responsive viewport. Learn more in Create Responsive AMP Pages.|
	|   |   |
  
  
  
<br /><br /><br /><br /><br /><br />
  

  
  <style amp-boilerplate>body {
	-webkit-animation: -amp-start 8s steps(1, end) 0s 1 normal both;
	-moz-animation: -amp-start 8s steps(1, end) 0s 1 normal both;
	-ms-animation: -amp-start 8s steps(1, end) 0s 1 normal both;
	animation: -amp-start 8s steps(1, end) 0s 1 normal both
}

@-webkit-keyframes -amp-start {
	from {
		visibility: hidden
	}
	to {
		visibility: visible
	}
}

@-moz-keyframes -amp-start {
	from {
		visibility: hidden
	}
	to {
		visibility: visible
	}
}

@-ms-keyframes -amp-start {
	from {
		visibility: hidden
	}
	to {
		visibility: visible
	}
}

@-o-keyframes -amp-start {
	from {
		visibility: hidden
	}
	to {
		visibility: visible
	}
}

@keyframes -amp-start {
	from {
		visibility: hidden
	}
	to {
		visibility: visible
	}
}

</style>
<noscript>
  <style amp-boilerplate>body {
	-webkit-animation: none;
	-moz-animation: none;
	-ms-animation: none;
	animation: none
}
</style>
</noscript>
