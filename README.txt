**************************************************************************************************
Assumptions:

1) 	artifacts and recomendations are 'attached' only at the Application Level

2) 	the hiearchy will always follow the same strict structure. ie: an application must have a 
	category, domain, and portfolio above it without skipping any steps.


**************************************************************************************************
Questions:

1) 	What exactly are recomendations and artifacts? Should they link to another page? contain more
	information beyond a name?

2)	How are we looking at generating our json objects and have we decided on a structure there?


**************************************************************************************************
Known Flaws:

1)	Nodes depend on nested for loops to decend the chain and access lower recomendations. This
	causes the higher nodes to crash the page

2)	Currently leans heavily on a specific format in the json to help modify html elements. Probably
	Not the best structure in the world

3)	Most of the styling for elements is added with d3 scripting as they are created on the page.
	Seperating the css into a style sheet would be cleaner

4)	Very static. As a resutlt current page layout not suitable for the size of trees we would 
	likely be creating 


**************************************************************************************************
Wish list:

1)	fixed size rec and artifact divs with a scrole bar rather than dynamically sized

2)	access the recs/artifacts from higher nodes without crashing the page

3)	collapsible nodes

4)	tie collapsible tree to collapsible dropdown menu

5)	zoom, pan

6)	color scale to indicate health if at all possible
