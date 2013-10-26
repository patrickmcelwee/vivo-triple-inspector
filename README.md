vivo-triple-inspector
=====================

Inspect VIVO triples related to a specified VIVO uri. Two files:

# Usage

1. inspector-request.html  Present a form to a user where the user can 
type in a VIVO URI.  Submit the form via a GET to inspector-results.html
1. inspector-results.html Receive a VIVO URI via a GET, create a SPARQL 
query to return the triples that have the specified URI as the subject.
Display the triples using D3.js in three columns:
    1. Show the predicate as a link to the predicate definition
	1. Show a second column which contains a "V" if the object is a resource
	and can be viewed in VIVO. The V is a link to display the object in VIVO.
	If the object is a literal, the second column is blank.
	1. Show a third column containing the object.  Show the literal value or
	show a link to an inspector-request for the the object.
	
# Styles

These pages use the wilma.css style file from VIVO.

Additional styles are used by inspector-results.html and can be found in 
the html file.

# D3

inspector-results.html uses D3.js to display results.  D3 is a powerful 
Javascript library for data driven documents.  See d3js.org

# License

    author       = "Michael Conlon"
    copyright    = "Copyright 2013, University of Florida"
    license      = "BSD 3-Clause license"
    version      = "01.0"