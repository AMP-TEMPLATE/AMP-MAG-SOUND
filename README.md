AMP-MAG

|RULE                                                     	                      | DESCRIPTION                     	|
|-------------------------------------------------------------------------------------|----------------------------------------	|
| Start with the <span style="background-color:grey"><!doctype html> doctype.         |  Standard for HTML.  	                | 
| Contain a top-level '<html ⚡>' tag <br />(<html amp> is accepted as well)          |  Identifies the page as AMP content.    |
| Contain '<head>' and '<body>' tags.                                                 | Optional in HTML but not in AMP.        |
| Contain a <meta charset="utf-8"> tag as the first<br />child of their <head> tag    | Identifies the encoding for the page    |

  
  
  

  

  
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
