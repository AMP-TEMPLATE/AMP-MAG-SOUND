AMP-MAG

| Tables                                	|          Are      	|  
|-----------------------------------------|:-------------:	    |
| Start with the <!doctype html> doctype 	|  Standard for HTML 	| 
| Contain a top-level <html ⚡> tag 
(<html amp> is accepted as well) 	|    Identifies the page as AMP content   	|   
| Contain <head> and <body> tags 	| Optional in HTML but not in AMP 	| 
  
  
  
  
Start with the <!doctype html> doctype.	Standard for HTML.
Contain a top-level <html ⚡> tag 
(<html amp> is accepted as well).	Identifies the page as AMP content.
  
Contain <head> and <body> tags.	Optional in HTML but not in AMP.
Contain a <meta charset="utf-8"> tag as the first child of their <head> tag.	Identifies the encoding for the page.
Contain a <script async src="https://cdn.ampproject.org/v0.js"></script> tag as the second child of their <head> tag.	Includes and loads the AMP JS library.
Contain a <link rel="canonical" href="$SOME_URL"> tag inside their <head>.	Points to the regular HTML version of the AMP HTML document or to itself if no such HTML version exists. Learn more in Make Your Page Discoverable.
Contain a <meta name="viewport" content="width=device-width,minimum-scale=1"> tag inside their <head> tag. It's also recommended to include initial-scale=1.	Specifies a responsive viewport. Learn more in Create Responsive AMP Pages.
Contain the AMP boilerplate code in their <head> tag.	CSS boilerplate to initially hide the content until AMP JS is loaded.
