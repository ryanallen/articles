1. How to Use Semantic Markup to Improve Discoverability
  2.1 What is Discoverability?
  2.2 Markup
    3.2.1 Definition
    3.2.2 Reword
    3.2.3 Non Technical Example
    3.2.4 Technical Example
  2.3 HTML
    3.3.1 Content
    3.3.2 Title
  2.4 Facebook's Open Graph Protocol
    3.4.1 Required Open Graph Markup
      4.4.1.1 Title
      4.4.1.2 Type
      4.4.1.3 Image
      4.4.1.4 URL
      4.4.1.5 Target Audience
    3.4.2 Optional Markup
  2.5 Twitter Cards
    3.5.1 Required Twitter Markup
      4.5.1.1 Minimizing Duplicate Markup
      4.5.1.2 Card Type
      4.5.1.3 Attribution
  2.6 Microdata and Search Engine Optimization
    3.6.1 Required Microdata Markup
      4.6.1.1 Item Scope
      4.6.1.2 Item Type
    3.6.2 Optional Microdata
      4.6.2.1 Image
      4.6.2.2 Height
      4.6.2.3 Width
      4.6.2.4 Artform
      4.6.2.5 Material
      4.6.2.6 Author
      4.6.2.7 Audience
      4.6.2.8 Educational Use
      4.6.2.9 Family Friendly
      4.6.2.10 Character
      4.6.2.11 About
      4.6.2.12 Keywords
  2.7 Validate
  2.8 Summary

---
@324
####Target Audience

The point of this article isn't to teach you how to identify your target audience. I do however, want to impress upon you the importance of knowing who that is.

---




## Semantics

---

We will do this by remaining patient, focused, and truthful in our considerations for the true meaning our content conveys relative to our [target audience](http://www.forbes.com/sites/jaysondemers/2013/08/27/6-steps-to-decoding-your-target-audience/).

You and I will then use our time in an effort to really listen to, empathize with, and understand the ideas, values, and core motivators for that target audience. 

Finally we will teach the machines, through the use of thoroughly considered and validated semantics in our markup, the true meaning of the thoughts, ideas, and words in our markup.

"With all this in hand, we shall grow healthily as human beings, able to influence others with meaning. So we shall arrive at a sustained level of mutual and truthful communication." - Dominick A. Barbara: [*The Art of Listening*](https://books.google.com/books?id=2dsWLwEACAAJ&dq=the+art+of+listening+barbara&hl=en&sa=X&ei=qb3bVMy1GYKrgwTo14D4Bg&ved=0CB8Q6AEwAA) Springfield, C. C. Thomas, 1958, p. 13. 

I know what you're thinking. 

"That sounds too complicated for a simple tutorial. For various reasons. None of which are any of your business!"

I agree. Let's simplify things. 

For this tutorial the target audience is a singular person. The best person. You.

---

## Markup
First, create the initial HTML document in the [text editor](http://computers.tutsplus.com/tutorials/vim-for-beginners--cms-21118) of your choice.

Declare the document type you intend to use as html:

<!DOCTYPE html>

Great! Now open an html tag.

<html>

Create an open head tag and a close head tag.

<head></head>

Create an open body tag and a close body tag.

<body></body>

Finally, close out your html.

</html>

Put it all together and what do you have?

<!DOCTYPE html>
<html>
<head></head>
<body></body>
</html>

That is so much simpler than the [ways it used to be](http://www.w3.org/TR/html4/sgml/dtd.html). Now let's add some content!

### Content
---


Create a top, level 1 heading that tells your target audience (you)
what they can expect from the paragraph of content it highlights.

In my example:

<h1>The Meaning Contained Within the Name Ryan</h1>

Create a paragraph that explains the meaning behind your name.

In my example:

<p>
  According to today's most reputable, 
  widely used, and socially accepted sources, 
  Ryan is a kingly name that represents the smartest, 
  best looking, and nicest guy ever.

  Ryan has the deepest respect for all beings regardless 
  of their differences, and is on an eternal quest
  to balance himself and find harmony with those around him.

  He's the best.
  Seriously.
  Just ask anyone.
</p>

Great! Now all that is left to do is add an image that represents your meaning.

###Adding Meaning

"Quote about meaning"

I don't know anything about you, however, I'm going to assume that you haven't been power-leveling your [precognition skill](http://starwars.wikia.com/wiki/Precognition) like I have been. Let's use a method that has been working for one [successful](http://www.buzzfeed.com/awesomer/what-would-the-buzzfeed-post-about-you-be-called#.ghw9oDp2xb) discovery platform.

You will need to start with a [data-researched, effective, and thought-provoking headline](http://minimaxir.com/2015/01/linkbait/).

First add a title no longer than 70 characters. It should summarize the *main idea* of your name in a way that is most likely to get the attention of your target audience, which is a singular individual, you.

What is the *main idea*, or the *meaning* contained within the word, symbol, or logo, that is your name?

---

####What Does Your Name Mean?

Time to research the *meaning* behind your name. Let's go to Google, our information overlord, for the top 3 search results!

#####A Meaningful Description by You

Research the meaning contained within your name the best way you know how. Here is how I went about it for my name, Ryan.

I decided to rely entirely on Google to answer this question.
[*meaning of name Ryan*](screenshot on desktop)

According to [one first-page source](http://www.behindthename.com/name/ryan):
"From an Irish surname which was derived from Ó Riain meaning 'descendent of Rían'. The given name Rían *probably* means "little king" (from Irish rí "king" combined with a [small] suffix)."

So it *might* be part of an Irish word with a different spelling with some extra letters added on the end for aesthetic reasons.

Another [first-page source](http://www.sheknows.com/baby-names/name/ryan) says:
"American Meaning: The name Ryan is an American baby name. In American the meaning of the name Ryan is: Little king."

Wait I thought it was Irish?

The best [first-page source](http://www.urbandictionary.com/define.php?term=ryan) says:
"the cutest guy ever, and has the greatest respect for girls, is funny, and very very LOVING!
Ryan wants to go to Virginia Beach to vistit (sp) one girl he met there on vacation1"

The reason I *think* this last result is *the best* is due to its top ranking on two, not just one, top platforms, [Google](https://www.google.com/search?client=safari&rls=en&q=meaning+of+the+name+ryan&ie=UTF-8&oe=UTF-8) and [Urban Dictionary](http://www.urbandictionary.com/define.php?term=ryan). Also because clearly, it's the best.

What was the best meaning you found contained in your name? Tell me the best description of your name in the comments or on [Twitter](https://twitter.com/ryanallen_com)!

For the [good of posterity](https://answers.yahoo.com/question/index?qid=20081103122314AANaZCr), I'll remove spelling and punctuation errors and reformat it into a clearer, more precise, and truer description.

<meta
  name="description" 
  content="Ryan has the deepest respect for all living 
  and nonliving beings regardless of their gender, nationality, 
  or plane of existence. There is one person, place, and time, 
  he is eternally seeking to form a reconnection with. The Yin 
  to his Yang. 

  Ryan is the cutest guy ever. 
  I'm super serious, everyone thinks so!"
> 

That is pretty text heavy description. I will [abstract](http://web.engr.oregonstate.edu/~budd/Books/oopintro3e/info/chap02.pdf) some ideas away to compress the text (with an unknown algorithm my brain created long ago) and find the core message.

[map zoom abstraction animation](imgurl)

<meta
  name="description" 
  content="Ryan is the best."
>

I think that was [the meat of it](http://www.bestlibrary.org/ssmedia/2009/10/identify-main-points-in-an-article-or-illustration-.html). It relates to the meaning expressed in the other examples as well. [Some kings were the best](http://listverse.com/2010/08/11/top-10-greatest-monarchs/) person a community had to represent and lead them.

I can now extract an interesting headline from my description that will hopefully get my attention in the future.

<title>
  You Probably Don&#8217;t Know 
  What Name Represents 
  the Best Person
</title>

Incredible. We should let everyone know who masterfully crafted this typographical work of art!

<meta name="author" content="Ryan Allen">

This might not be as important as we used to think, at least not [according to Google](https://webdesign.tutsplus.com/articles/why-you-should-add-authorship-information-to-your-website--webdesign-8957).

What does it all look like together?

<!DOCTYPE html>
  <html>
    <head>
      <title>
        The Meaning 
        Behind the Name: 
        Ryan
      </title>
      <meta 
        name="author" 
        content="Ryan Allen"
      >
      <meta
        name="description" 
        content="Ryan is the best."
      >
    </head>
    <body></body>
  </html>

---



####Show and Tell

Humans like images. You are human. Let's show future you an image that conveys *the meaning contained in your name* in the best, visually pleasing way.

<img src="URL TO YOUR IMAGE">

[handsome photo of me](imgurl)

That is a really, really, good looking image. Seriously. 

### Everyone on Facebook Needs to See This

The [Open Graph](http://ogp.me) protocol enables any web page to become a rich object in Facebook's social graph. It allows any web page to have the same functionality as an object on Facebook. It was [launched in 2010](https://developers.facebook.com/blog/post/377/) at [f8](https://fbf8.com), Facebook's developer conference.

Let's teach Facebook about the meaning of your name.

Facebook's open graph (as well as Twitter's card system we will look at next) works with meta data that you add inside your web pages' <head></head>. In the case of Facebook's open graph protocol there are *four* properties that are required.

#### Required Open Graph Markup

[facebook screenshot sharing ryan](imgurl)

The four required open graph properties Facebook requires are:  

* title
* type
* image
* url

#####Title
The first property Facebook requires is the Title tag, which is the title of your object as it should appear on Facebook.

[callout title](imgurl)

Here is how my example will be titled when the HTML document is shared on facebook.

<meta 
  property="og:title" 
  content="
  You Probably Don't Know 
  What Name Represents 
  the Best Person"
>

####Type
The second property Facebook requires is the [type of object](http://ogp.me/#types) it will be showing users on its platform.

[callout website](imgurl)

We are making this statement in an HTML document, which when uploaded to a web server, becomes a [website](http://graph.facebook.com/schema/og/website).

<meta 
  property="og:type" 
  content="website"
>

#####Image
The third property Facebook requires is an image that represents your object.

What image will you use to convey an abstract idea about your name?

Here is what it looks like for my example:

<meta 
  property="og:image" 
  content="http://ryanallen.com/img/ryan-is-the-best.png"
>

#####URL
The final property Facebook requires is the URL users will experience when interacting with the object.

Where are you going to upload this HTML document you are making?

Here is where mine lives:

<meta 
  property="og:url" 
  content="http://ryanallen.com/semantics/"
>

####Optional Markup
We can add some [additional markup](http://ogp.me/ns/ogp.me.ttl) like a [description](http://ogp.me/ns/ogp.me.ttl), which while not required, makes it easier for Facebook to learn as much as we are willing to teach.

<meta 
  property="og:description" 
  content="According to today's most reputable, 
  widely used, and socially accepted sources, 
  Ryan is the smartest, best looking, and nicest 
  guy ever. His fragrance is derived from a 
  sensual mix of exotic oils known only to 
  a select few Mystics and Shaman. 

  He's the best.
  Seriously."
>

There sure are a lot of ways to convey meaning behind a word. Semantics is crazy. Let's take a look at the different semantics another popular social network and discoverability platform uses!

---

1. How to Use Semantic Markup to Improve Discoverability
  1.1 Markup
    1.1.1 Definition
    1.1.2 Reword
    1.1.3 Non Technical Example
    1.1.4 Technical Example
  1.2 HTML
    1.2.1 Content
    1.2.2 Title
  1.3 Facebook
    1.3.1 Required Open Graph Markup
      1.3.1.1 Title
      1.3.1.2 Type
      1.3.1.3 Image
      1.3.1.4 URL
    1.3.2 Optional Markup

---

### Twitter Cards

[Twitter Card Example](imgurl)

Twitter Cards are based on the [same conventions](https://dev.twitter.com/cards/getting-started#opengraph) as the Open Graph protocol, which makes it easier to generate a Twitter card without duplicating our markups' meta tags. Hooray!

Speaking of markup, what does our markup look like at this point?

<!DOCTYPE html>
  <html>
    <head>
      <title>
        The Meaning 
        Behind the Name: 
        Ryan
      </title>
      <meta 
        name="author" 
        content="Ryan Allen"
      >
      <meta
        name="description" 
        content="Ryan is the best."
      >
      <!-- FACEBOOK OPEN GRAPH -->
      <meta 
        property="og:title" 
        content="
        You Probably Don't Know 
        What Name Represents 
        the Best Person"
      >
      <meta 
        property="og:type" 
        content="website"
      >
      <meta 
        property="og:image" 
        content="http://ryanallen.com/img/ryan-is-the-best.png"
      >
      <meta 
        property="og:url" 
        content="http://ryanallen.com/semantics/"
      >
      <meta 
        property="og:description" 
        content="According to today's most reputable, 
        widely used, and socially accepted sources, 
        Ryan is the smartest, best looking, and nicest 
        guy ever. His fragrance is derived from a 
        sensual mix of exotic oils known only to 
        a select few Mystics and Shaman. 

        He's the best.
        Seriously."
      >
    </head>
    <body>
      <h1>
        You Probably Don't Know 
        What Name Represents 
        the Best Person
      </h1>
      <h2>
        It's Ryan.
      </h2>
      <img 
        src="http://ryanallen.com/img/ryan-is-the-best.png"
      >
    </body>
  </html>

Perfect!

#### Required Twitter Card Markup

The five required properties properties Twitter cards require are:  

* card
* content owner's twitter account
* title
* description
* image

"When the Twitter card processor looks for tags on your page, it first checks for the Twitter property, and if not present, falls back to the supported Open Graph property. This allows for both to be defined on the page independently, and minimizes the amount of duplicate markup required to describe your content and experience." [source](https://dev.twitter.com/cards/getting-started#opengraph)

That's great! The tags we don't need to duplicate are:  

* og:title
* og:description
* og:image

Three down, two to go!

#####Content Type

First tell Twitter the [type of content](https://dev.twitter.com/cards/types) you are sharing.

[callout type](imgurl)

Here is how I am setting my content to be displayed as the default *Summary Card* when the HTML document is shared on Twitter.

<meta 
  name="twitter:card" 
  content="summary"
>

Great! That was simple.

Twitter requires an account to be associated with the website holding the content. You can use your twitter account:

<meta 
  name="twitter:creator" 
  content="@yourTwitterUsername"
>

If this is being done within an abstract container, such as a company page, or a company department, you can use a site style attribution:

<meta name="twitter:site" content="@CompanyTwitterUsername">

Twitter will need to authenticate and white-list your domain for each type of Twitter Card. It is simple and automated. I don't know what is involved if you get blacklisted. If anyone has experience with this I would enjoy learning more.

So what does our markup look like now with Twitter Cards added?

<!DOCTYPE html>
  <html>
    <head>
      <title>
        The Meaning 
        Behind the Name: 
        Ryan
      </title>
      <meta 
        name="author" 
        content="Ryan Allen"
      >
      <meta
        name="description" 
        content="Ryan is the best."
      >
      <!-- FACEBOOK OPEN GRAPH -->
      <meta 
        property="og:title" 
        content="
        You Probably Don't Know 
        What Name Represents 
        the Best Person"
      >
      <meta 
        property="og:type" 
        content="website"
      >
      <meta 
        property="og:image" 
        content="http://ryanallen.com/img/ryan-is-the-best.png"
      >
      <meta 
        property="og:url" 
        content="http://ryanallen.com/semantics/"
      >
      <meta 
        property="og:description" 
        content="According to today's most reputable, 
        widely used, and socially accepted sources, 
        Ryan is the smartest, best looking, and nicest 
        guy ever. His fragrance is derived from a 
        sensual mix of exotic oils known only to 
        a select few Mystics and Shaman. 

        He's the best.
        Seriously."
      >
      <!-- TWITTER CARD -->
      <meta 
        name="twitter:card" 
        content="summary"
      >
      <meta 
        name="twitter:creator" 
        content="@ryanallen_com"
      >
    </head>
    <body>
      <h1>
        You Probably Don't Know 
        What Name Represents 
        the Best Person
      </h1>
      <h2>
        It's Ryan.
      </h2>
      <img 
        src="http://ryanallen.com/img/ryan-is-the-best.png"
      >
    </body>
  </html>

Good thing we did Open Graph first, Twitter allows us to save a lot of time by working with other platforms to the best of its ability. Thanks Twitter.

Time to revisit the search engines for some new, contextual, and exciting ways to optimize your SEO!

### Microdata and Search Engine Optimization

"On June 2nd [2011] we [Microsoft] announced a collaboration between Bing, Google and Yahoo to create and support a standard set of schemas for structured data markup on web pages. Although our companies compete in many ways, it was evident to us that collaboration in this space would be good for each search engine individually and for the industry as a whole." - [Michael O'Connor](http://blog.schema.org/2011/07/on-june-2-nd-we-announced-collaboration.html)

[Microdata](http://schema.org/docs/gs.html) is different from the other markup we have already structured in that it does not live in the document head.

We will use microdata to infuse context into our content in our HTML document's body. [Search engines will use our data to improve the discoverability of our content](https://support.google.com/webmasters/answer/99170) for their users.

The machines believe what we tell them. For now at least...

####Required Microdata Markup 
The following tags are required for every item you wish to build meaning into. 

* Item Scope
* Item Type

First we [need to identify](https://schema.org/docs/full.html) the *thing* we are describing. 

What are we describing again? It's something intangable...

<h1
  itemscope 
  itemtype="https://schema.org/Intangible"
>
  You Probably Don't Know What Name Represents the Best Person
</h1>

That was simple. I isn't very useful by itself, it needs more context to relate to. Let's add some.

####Optional Microdata Markup

By adding [data that describes](https://schema.org/docs/full.html) the item's properties as well as embedded meta data you can ensure the humans using Google, Bing, Yahoo! and other discoverability platforms, receive as much useful meaning as you can provide.

Where were we again?

...You Probably Don't Know What 

Oh right. We were talking about a name...

<meta 
  itemprop="name"
  content="Ryan"
>

...and the meaning behind that name. 

The name, in my example, Ryan... 

Represents 
<span 
  itemprop="description"
>
  the Best Person
</span>


Now remember we are talking about a name and the letters, symbols, or logos used to convey the context and meaning contained within the idea, or branding, of the name.

<h2  
  itemscope 
  itemtype="http://schema.org/Brand"
  itemprop="brand"
  itemprop="name"
>

What was my name again?

It's Ryan.

Don't forgot the image being used to brand visual meaning. My example looks like this:

<img
  itemprop="logo" 
  src="http://ryanallen.com/img/ryan-is-the-best.png"
>

That should wrap things up. Let's take a look at everything together!

###Final Markup
<!DOCTYPE html>
  <html>
    <head>
      <title>
        You Probably Don&#8217;t Know 
        What Name Represents 
        the Best Person
      </title>
      <meta 
        name="author" 
        content="Ryan Allen"
      >
      <meta
        name="description" 
        content="Ryan is the best."
      >
      <!-- FACEBOOK OPEN GRAPH -->
      <meta 
        property="og:title" 
        content="
        You Probably Don&#8217;t Know 
        What Name Represents 
        the Best Person"
      >
      <meta 
        property="og:type" 
        content="website"
      >
      <meta 
        property="og:image" 
        content="http://ryanallen.com/img/ryan-is-the-best.png"
      >
      <meta 
        property="og:url" 
        content="http://ryanallen.com/semantics/"
      >
      <meta 
        property="og:description" 
        content="According to today's most reputable, 
        widely used, and socially accepted sources, 
        Ryan is the smartest, best looking, and nicest 
        guy ever. His fragrance is derived from a 
        sensual mix of exotic oils known only to 
        a select few Mystics and Shaman. 

        He's the best.
        Seriously."
      >
      <!-- TWITTER CARD -->
      <meta 
        name="twitter:card" 
        content="summary"
      >
      <meta 
        name="twitter:creator" 
        content="@ryanallen_com"
      >
    </head>
    <body>
      <h1
        itemscope 
        itemtype="https://schema.org/Intangible"
      >
        You Probably Don&#8217;t Know What 

        <meta 
          itemprop="name"
          content="Ryan"
        >
          Name 
        </span>
        Represents 
        <span 
          itemprop="description"
        >
          the Best Person
        </span>
      </h1>
      <h2  
        itemscope 
        itemtype="http://schema.org/Brand"
        itemprop="brand"
        itemprop="name"
      >
        It&#8217;s Ryan.
      </h2>
      <img
        itemprop="logo" 
        src="http://ryanallen.com/img/ryan-is-the-best.png"
      >
    </body>
  </html>

####Upload and Validate

Upload your HyperText Markup Language documents to the publicly available [world wide web](http://reason.com/archives/2014/01/03/is-skynet-inevitable).

Here is where my example can be found:

[http://ryanallen.com/semantics/](http://ryanallen.com/semantics/)

Validate your code with [Google](http://www.google.com/webmasters/tools/richsnippets), then [Facebook](https://developers.facebook.com/tools/debug/), and finally with
[Twitter](https://cards-dev.twitter.com/validator). Fix any errors you come across like the professional that you are.

I hope you enjoyed learning about a few of the most popular methods used to describe meaning to the most popular discoverablitly platforms to allow their users to find you which in turn bumps your content up in the rankings of these platforms which means more people will find and share and learn from your content which will drive it further up the rankings on these platforms until you are the best number one
