# Commerce
CS50w Project 2: Django E-Commerce Website

The app let's users browse, bet and comment on e-bay like auctions, as well as create their own listings. The app supports auction watchlist. 

### Specification:
<https://cs50.harvard.edu/web/2020/projects/2/commerce/>

### Video Demo:
<https://www.youtube.com/watch?v=bNbtJ6nHQy8>

### auctions/models.py
Contains Django models that define structure for the stored data:
* Listing - contains information about every listing.
* Bid - stores all user auction bids.
* Comment - stores all user comments.
* Watchlist - stores all items added to the user's watchlist.
* Winner - stores winners for every listing.
* Category - stores every listing's category.

### auctions/views.py
Contains views associated with each of the routes. 

### auctions/urls.py
Contains URL configuration for the app:
* / - main page, shows all active listings.
* /login - login interface.
* /logout - logout interface.
* /register - register interface.
* /categories - sorts all listings in categories.
* /category/<category_name> - shows all active listings in a given category.
* /listing/<listing_id> - show the listing.
* /create - let's user create a listing.
* /close/<listing_id> - let's user closer a listing if he/she is the creator.
* /bid/<listing_id> - let's user bid on the listing.
* /comment/<listing_id> - let's user comment on the listing.
* /watchlist - shows user's watchlist. 
* /watchlist_add/<listing_id> - let's user add listing to their watchlist.

### auctions/templates/auctions
Contains HTML templates, in particular: 
* index.html shows all active listings. 
* listing_show.html displays information about a given listing.
* listing_create.html let's the user create their own listing. 
