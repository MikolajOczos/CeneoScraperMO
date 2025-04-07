# CeneoScraperMO
1. Choose the product from the site (source). Send a request through a browser for access.
2. If response is ok, parse the html page contect into DOM structure.
3. Extract from the DOM structure opinions and their components.
4. Save opinions with their components at complex data structure.
5. If there are more pages with opinions, repeat steps 1-5
6. Save data strucutres with opinions into data base.
7.  
|Component | Variable | Selector
opinion | opinion | ds_product-review:not(.user-post--highlight)|
|opinion ID | opinion_id|["data-entry-id"]
|opinion’s author | author |span.user-post_author-name|
|author’s recommendation | recommend | span.user-post_author-name__author-recomendation > em|
|score expressed in number of stars | stars |span.user-post__score-count|
|opinion’s content | content | div.user-post__text |
|list of product advantages | pros | div.review-feature__item--positive|
|list of product disadvantages | cons | div.review-feature__item--negative | 
|how many users think that opinion was helpful |upvotes| button.vote-yes["data-total-vote"]|
|how many users think that opinion was unhelpful | downvotes | button.vote-no["data-total-vote"]|
|publishing date | published | span.user-post__published > time:nth-child(1)["datetime"] |
|purchase date | purchased | span.user-post__published > time:nth-child(2)["datetime] |















