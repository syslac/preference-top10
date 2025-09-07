# preference-top10

Ever tried to rank a large enough collection that you always risk forgetting something?

This simple web app tries to "solve" that problem by constructing a ranking by progressively pitching couple of items 1v1.

This is not the most optimized algorithm to sort the collection, probably, but gives the user the opportunity to actually work through the whole list and see some maybe unlikely pairings.
The page will keep promping the user with new comparisons until all items are fixed wrt the item just above. Usually it's not enough to run it to completion to get a reasonable top-N, because at some point you will be working to fix lower-ranking choices mostly, but you could be unlucky enough with the random selection that it's necessary to run it for a long-ish time to actually see all options.

Tech-wise, this is a single html file including enough javascript for it to work, with basically no styling, enough for it to work, and with sizes big enough for it to be readable on mobile browsers (you can share this via chat and open it on a mobile browser and it will work, stand-alone, no dependencies required).

There is no way to save partial completion; state gets cleaned at every page reload.

There is no way to accept user input for the input list, it's hardcoded in Javascript (and not included in this repo: bring your own list!).

Some comments in the code will probably refer to bands, as this was the initial concept for the app, but I've seen a similar design online used to find your favorite Pokémon, so I decided to reimplement it myself.
