# Graph generator from scientific papers
The script scrapes a given pdf trying to recostruct a graph containing the references between the pages of the paper. This can be particularly useful for long mathematical papers to understand the relationships between many results (theorems, lemmas, definitions...) and the structure of the underlying theory.

## How does it work?
The code reconstructs a dictionary with the extracted info by each link. then plots a graph of the corresponding adjancy matrix. 


Reverse engineering the pdf is quite complex, in particular we can only know the origin page of the link and not from which proof it comes from. On the other hand it's possible to extract the name of the destination object. This allows us to build a table of the most referenced results.

(Note that the links have to be clickable)
