AMP-MAG
# Required mark-up
### AMP HTML documents MUST  

<br />


|RULE                                                     	                      | DESCRIPTION                     	|
|-------------------------------------------------------------------------------------|----------------------------------------	|
| Start with the `<!doctype html>` doctype.                                             |  Standard for HTML.  	                | 
| Contain a top-level `<html ⚡>` tag <br>(`<html amp>` is accepted as well)            |  Identifies the page as AMP content.    |
| Contain `<head>` and `<body>` tags.                                                     | Optional in HTML but not in AMP.        |
| Contain a `<meta charset="utf-8">` tag as the first child of their `<head>` tag    | Identifies the encoding for the page    |
| Contain a  <script async src="https://cdn.ampproject.org/v0.js"></script> tag as the second child of their `<head>` tag.   | Includes and loads the AMP JS library.    |
|Contain a <link rel="canonical" href="$SOME_URL"> tag inside their `<head>`  | Points to the regular HTML version of the AMP <br>  HTML document or to itself if no such HTML <br>version exists. Learn more in `Make Your Page Discoverable`.|
|Contain a <meta name="viewport" content="width=device-width,minimum-scale=1"> tag inside their `<head>` tag. It's also recommended to include initial-scale=1 | Specifies a responsive viewport. Learn more in `Create Responsive AMP Pages`.|
| Contain the `AMP boilerplate code` in their `<head> tag.`  |  CSS boilerplate to initially hide the content until AMP JS is loaded. | 
  

  
 ``` 
 <style amp-boilerplate>
 	body {
		
        }
```


``` @-webkit-keyframes -amp-start {
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
```
