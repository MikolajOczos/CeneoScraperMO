# CeneoScraperMO
1. Choose the product from the site (source). Send a request through a browser for access.
2. If response is ok, parse the html page contect into DOM structure.
3. Extract from the DOM structure opinions and their components.
4. Save opinions with their components at complex data structure.
5. If there are more pages with opinions, repeat steps 1-5
6. Save data strucutres with opinions into data base.
7.  
### Structure of single opinion on ceneo.pl
|Component | Variable | Selector
|opinion ID | opinion|
|opinion’s author | author |
|author’s recommendation | recommend | 
|score expressed in number of stars | stars |
|opinion’s content | content
|list of product advantages | pros
|list of product disadvantages | cons
|how many users think that opinion was helpful |upvotes
|how many users think that opinion was unhelpful | downvotes
|publishing date | published |
|purchase date | purchased |
|