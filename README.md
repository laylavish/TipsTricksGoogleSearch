# Tips & Tricks to Get Search Engines to Return Authentic Results

Tips and tricks you can do to make Google Search (and other search engines that have similar operators) remove a lot of AI generated imagery and/or results (eg. llm garbage)

### Preliminary
This is meant to be used in conjunction with my [huge AI blocklist for uBlock Origin and uBlacklist](https://github.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist), as using this guide supplements where the blocklist fails (and the blocklist supplements where this guide fails), leading to near-perfect image authenticity. 

You can of course use this guide alone, but the results won't be nearly as comprehensive as using this in conjunction with my blocklist. Thank you for understanding.

## Minus Operator

The `-` operator excludes webpages that have a specified search term(s).

You can subtract multiple search terms (compound words) by adding quotation marks around them (eg. -"Apple iPhone").

For the purposes of removing AI content from search results, you can subtract search terms like `-ai,` `-"stable diffusion"`, `-"ai art"`, `-lora`, etc to remove results that have these search terms in plain text. This should clean up search results pretty well. 

If you want to remove the obvious theft and pawning of art through platforms like etsy, redbubble, displate, etc, you can be a bit \*creative* and subtract the search term `-"add to cart"` which will remove any site from Search that has shopping cart functionality.

> TIP: The minus operator can be used in conjunction with any other operator.


## Site Operator

The `site:` operator includes or excludes a specified website or domain. 

You can use the minus operator to subtract what sites you want to remove from Search. An example would be: `-site:midjourney.com`.

You can also limit to only have results with the domain of your choice, or remove specific top level domains. An example of removing a specific top level domain would be: `-site:.com`

To remove a lot of a lot of AI sites from Search, limit the domain to only `.com` with `site:.com`. Many AI sites use .ai, .art, .co, etc domains because they are substantially cheaper and often times coincide with the thing they do (eg. ai-concept.art), so limiting results only to `.com` will most certainly clean much of your results.


## Quotation Mark Operator

The `""` operator searches for webpages that include the EXACT term or terms you specify.

Can also be used in conjunction with the `-` operator to exclude multiple words or phrases from appearing in your searches (eg. -"midjourney art").

> TIP: Quotation marks can also be used for other operators as well, such as: `intext`; `intitle`; `allintext`; `allintitle`; basically all operators that allow you to exclude or include a word or phrase.


## Before and After Operators

The `before:` operator includes or excludes results **before** a specified date (eg. before:2022). All search results will be **before** 2022, no exceptions.

The `after:` operator includes or excludes results **after** a specified date (eg. after:2022). All search results will be **after** 2022, no exceptions.

You can combine both operators together for a precise search. An example would be: `digital art before:2022 after:2019`. This would search for results of digital art before 2022, but after 2019. No results from 2018, 2017, etc. Only results from 2020 and 2021.

To pretty much remove all AI from searches entirely, use `before:2022`. This will limit all results from before 2022, aka the year where AI really came into the fray. This will clean your searches pretty much perfectly, although information will be outdated, since it is not up-to-date.

## Intext Operator 

The `intext:` operator searches for webpages that include the term(s) you specify that exist in their content.

`intext:` is similar to the Quotation Marks, in that it searches for terms that you specify, but is dissimilar in the way it checks for said terms.

`intext:` searches for terms by searching through a page's content entirely. It checks headers, footers, paragraphs, comments, pretty much anything on the site that is in plain text.

You can inverse `intext:`'s function by subtracting it (eg. `-intext:midjourney`). Doing so will operate very similar to subtracting terms with Quotation Marks.

To remove AI garbage, you can add things like `-intext:"ai art"`, `-intext:lora`, `-intext:"stable diffusion"`, etc to clean up your results.


## Remove Borru Tagged Results

There are some stubborn sites that are in limbo in my [huge AI blocklist](https://github.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist). Take, for example, Pinterest.

Pinterest is a legitimate site for viewing authentic artwork, reference, and sharing of ideas; unfortunately Pinterest is overrun by AI garbage, so instead of outright blocking Pinterest, we can block a lot of the AI trash that exists when you use your handy-dandy Search operators.

Here's the thing: AI "artists" are not artists, therefore they are incapable of describing artwork. 

They are only capable of describing their "artwork" via [borru tagging](https://danbooru.donmai.us/wiki_pages/howto:tag), which describes artwork in the most rudimentary way. That's why you'll see AI bros describe artwork with "high detail", "intricate details", "breath-taking", "captivating", "enchanting", "high quality", "beautiful", etc. Take a look at Etsy (and Pinterest) if you don't believe me.

So what we'll do is use their booru tagging against them. 

We can input their most used tags, such as "high detail", to filter out the AI garbage you see on Pinterest. 

Use `-intext:"high detail"` or another booru tag to filter out more AI trash.


## Limit Results to a Specific Region

You can limit Search to give you results from a specific region, which can clean image searches dramatically.

Changing the region in which results are retrieved to United States reduces AI appearances, since there are many Chinese AI sites and discussion boards.

Here are ways to limit the results to a specific region in the most popular search engines:


### In Google Search

In the bottom right or top right of Google, there should be a settings icon or settings title. Click on it, then click on advanced search.

There, you can narrow your results by a region that you select.


### In DuckDuckGo Search

Underneath your search bar, there should be an **All regions** drop down menu.

Click it, then type the region you want to limit search results to.


### In Brave Search

If you are using Local Results, turn it off by hitting the **Revert to global** blue text.

Underneath your search bar, there should be a settings button. Hit it, and a new sub menu should appear.

Now hit your locale (it should be the first bubble, mine says "United States"), and type in a region to narrow the results by.


## Limit Results by File Type

If you really wanna get down and dirty, you can use the `filetype:`operator (also available in advanced search) to limit the results by file type.

Why would you want to do this? Well, many AI sites use the file format webp, which is a file type that has an efficient compression algorithm. Its whole purpose is to save server data.

AI sites use webp because they produce so much data (AI spews out so much data very quickly), so we can limit the file type to `png` to remove AI sites that use webp by typing `filetype:png`. Although this helps, limiting the file type to `jpg` actually reduces AI queries even more, at the cost of potentially lower quality reference images.


## Query Limit

Yup, there is a query limit. 

The limit is 32 words, which is not that much. So, don't go willy-nilly and try to spam tons of filter terms in Search to try to clean it.

> As much as I want that to work, it unfortunately doesn't; so ya gotta be diligent with your query count.


## After That, Now What? 

So, now you're up to speed on Search and can achieve authentic results like how the internet used to be before AI.

So what now? This is just for search engines, what about social media sites like YouTube? 

Well, there is this extension called [BlockTube](https://addons.mozilla.org/en-US/firefox/addon/blocktube/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search) which allows you to block YouTubers from appearing on your feed; meaning, you can go on an AI YouTuber block-spree and remove them forever. 

Instagram and Twitter respectively have block features, so you can also go on a block-spree as well. Anything else that doesn't support blocking, use uBlock Origin.

# Special thanks

Thanks are given to [Google Guide](https://www.googleguide.com/category/overview/index.html) for the awesome overview of Google Search operators.
