# Tips & Tricks for Google Search to return authentic results

Tips and tricks you can do to make Google Search return authentic seach results, ya know, what you're **actually** looking for; eliminate AI results in your queries once and for all1

## Quintessential Google Search Operators

--

The minus ```-``` operator: Excludes webpages that have a term or terms you specify. 

You can add multiple terms by adding quotation marks around the terms (eg. -"apple iphone").

For the purposes of removing AI content from queries, you can add these at the end of your query; -ai -ia -"stable diffusion" -"ai art" -lora. This should clean up the results well, but if you want to remove the obvious theft and pawning of art through platforms like etsy, redbubble, displate, etc, you can add this at the end of your query: -"add * cart" (or just -$ -€). 
> The star ```*``` symbol is known as a wildcard, which matches a word with any phrase. The phrase we set is "add to cart", but we replace "to" with the star operator ```*``` just to make sure everything is caught, plus, wildcards don't take up query count (which i'll get to later).

The minus operator can be used in conjunction with any other operator.

--

The ```site:``` operator: Includes or excludes a website or domain you specify (eg. site:youtube.com -- will limit all results to the domain YouTube.com).

You can add the minus ```-``` operator in front of the site (site:) operator to exclude sites you DON'T want to see (eg. -site:reddit.com). 
> This goes far beyond just naming sites, since you can also limit queries to have a domain extension of your choosing (eg. site:.com).

Now, let's apply this to remove much of this AI filth.

Limiting the query to only have .com will remove a lot of the AI garbage, since a lot of AI sites use domains that end in .ai, .art, .co, .xyz, etc. 

In your query, add ```site:.com``` at the very end of your query to remove AI sites that use .ai, .art, .co, etc top level domains.

--

The quotation marks ```""``` operator: Searches for webpages that include the EXACT term or terms you specify; will not perform automatic stemming of phrases (eg. "run" will not search for "running", "ran", etc).

> Using quotation marks is very useful if you are looking for an exact term or phrase within a webpage (eg. "anime" digital art).

Can also be used in conjunction with the minus ```-``` operator to exclude multiple words or phrases from appearing in your queries (eg. -"midjourney art").

Quotation marks can also be used for other operators as well, such as: ```intext```; ```intitle```; ```allintext```; ```allintitle```; etc.

-- 

The ```before:``` and ```after:``` operator: Includes or excludes results before or after user specified dates (eg. before:2022, or after:2022).

Can be useful if you are looking for authentic artwork before this AI ordeal. 

Append ```before:2022``` to the end of your query to achieve authentic results.

-- 

The ```intext:``` operator: Searches for webpages that include the term(s) you specify that exist in their content (eg. intext:animation); similar to the quotation marks operator.

Useful for finding terms that exist within a page's content, such as inside paragraphs, header and footers, comments, etc.

For removing AI garbage, I like to add ```-intext:lora``` towards the end of my query.

--

Those are what I believe to be the most essential Google Search operators, and they are extremely useful. Now time for some tips and tricks.

There are some stubborn sites that are in limbo in my [huge AI blocklist](https://github.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist). Take, for example, Pinterest.

Pinterest is a legitimate site for viewing authentic artwork, reference, and sharing of ideas; unfortunately Pinterest is overrun by AI garbage, so instead of outright blocking Pinterest (if you want, Pinterest does exist in the nuclear section), we can block a lot of the AI garbage that exists when you do a Google Search with our handy dandy operators.

Here's the thing: AI "artists" are not artists, therefore they are incapable of describing artwork. They are only capable of describing their "artwork" via borru tagging, which describes artwork in the most rudimentary way. That's why you'll see AI bros describe artwork with "high detail", "intricate details", "breath-taking", "captivating", "enchanting", "high quality", "beautiful", "cute (insert subject here)", etc. Take a look at Etsy (and Pinterest) if you don't believe me.

So what we'll do is use their booru tagging against them. We can input their most used tags, such as "high detail", to filter out the AI garbage you see on Pinterest. I often append (-intext:"high detail") or another booru tag at the end to filter out more AI trash.

Now, the query limit. Yes, there is a query limit. The limit is 32 words, which is not that much. So, don't go willy-nilly and try to spam tons of filter terms in Google Search to try to clean Google Search. As much as I want that to work, it unfortunately doesn't; so ya gotta be diligent with your query count. One way to bypass query count (kinda) is to use wildcards.

Wildcards don't use up the query count, whereas common words, known as stop words (eg. where, do, I for, a) do take up query count. So you can substitute wildcards for stopwords (since google discards stopwords unless quoated) and save query count.

Now, for more obscure tips. You can limit the query to give you results from a specific region, which is only available by using advanced search.

In the bottom right or top right of Google, there should be a settings icon or settings title. Click on it, then click on advanced search. Now you can narrow you results by a region that you select. I often limit the region to United States, since it removes a lot of Chinese AI "art" and AI discussion boards.

If you really wanna get down and dirty, you can use the filetype (filetype:) operator (also in advanced search) to limit the results by file type.

Why would you want to do this? Well, many AI sites use the file format Webp, which is a file type that has an efficient compression algorithm. Its whole purpose is to save server data.

AI sites use webp because of the amount of data being produced, so we can limit the file type to png to remove AI sites that use webp by typing (filetype:png). Although this helps, limiting the file type to jpg actually reduces AI queries even more, at the cost of lossy images (although that's not really a problem).

So, now you're up to speed on Google Search and can achieve authentic results like how the internet used to be before AI.

So what now? This is just for Google Search, what about social media sites like YouTube? Well, there is this extension called BlockTube which allows you to block YouTubers from appearing on your feed; meaning, you can go on an AI YouTuber block-spree and remove them forever. Instagram and Twitter respectively have block features, so you can also go on a block-spree as well. Anything else that doesn't support blocking, use uBlock Origin.
