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

#How to Use Semantic Markup to Improve Discoverability
By building meaning into your content with open graph, twitter cards, and microdata, your content will be more attractive, more relavant, and more discoverable to potential users.

---

Google, Facebook, Twitter, and many other platforms you and I use to share and discover content can not read our minds... at least [not yet](http://www.wired.com/2012/11/mike-vernal-facebook/). The [machines powering the cloud](http://en.wikipedia.org/wiki/Skynet_(Terminator))rely on you and I, designers and developers, to teach them about the meaning contained in our content and how it relates to our target audience. By teaching these platforms about abstraction and meaning we allow them to display more relevant, provocative, and discoverable content.  

##What is Discoverability?

Discoverability is the ease at which a machine or person can find a bit of relevant information online. 

Which one of these facebook posts gets more of your attention?
[fb](imgurl)

Which one of these tweets is more provocative?
[tweet](imgurl)

Which one of these Google search results is more interesting?
[Google](imgurl)

The differences above are very obvious. If you are not implementing Facebook's Open Graph Protocol, Twitter's Card system, and Microdata for search engines, your content is being ignored in favor of your competitors' more interestingly displayed content. In this article I will show you the importance of understanding your target audience while implementing these systems into your semantic markup. 

##Markup

First, what exactly is *markup*?

Formal Definition:
"A [document markup language](http://en.wikipedia.org/wiki/Markup_language) is a modern system for annotating a document in a way that is [syntactically](http://en.wikipedia.org/wiki/Syntax) distinguishable from the text."

In simpler terms, it's a way to mark, annotate, or style a document with pens, pencils or computers in a way that looks symbolically different than the text you are *marking up*. The term comes from proofreaders who would *markup* manuscripts for edits. 

![Illustration of Proofreaders' Marks on Manuscript](imgurl)

Proofreaders' marks are a form of markup. Remember these from middle school English class... or were you too busy with your Pokemon and your fancy Walkman to pay attention?!

Here are 3 ways you can markup a document to indicate a heading in a digital document:

[HTML](http://webdesign.tutsplus.com/courses/30-days-to-learn-html-css):

    <h1>I Am the Best Heading</h1>

[Markdown](http://daringfireball.net/projects/markdown/syntax):

    ## No I Am the Best Heading

[LaTeX](http://latex-project.org/guides/usrguide.tex)

    \section{I'm LaTeX}

Now that you have a clearer understanding of what LaTeX... err, **markup** is, we will create a basic HTML5 document with a single piece of content to illustrate the different ways to build meaning into that content which will lead to an increase it the ability for it to be discovered.

##HTML

First, we will create the initial HTML document in the [text editor](http://computers.tutsplus.com/tutorials/vim-for-beginners--cms-21118) of your choice.

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

###Content
Now let's add our single piece of content, an image of a very unhappy cat, into a section inside our document body.

<body>
  <section>
    <img
      src="http://ryanallen.com/img/forlorn-feline.gif"
    >
  </section>
</body>

###Title
Now that we know what content we are working with we can add the first bit of context to our page. Our tried and true <title> tag inside our document's head.

<head>
  <title>Forlorn Feline</title>
</head>

Easy! Let's move on to something a bit more challenging (though still simple) with Facebook's Open Graph Protocol!

##Facebook

The [Open Graph](http://ogp.me) protocol enables any web page to become a rich object in Facebook's social graph. It allows any web page to have the same functionality as an object on Facebook. It was [launched in 2010](https://developers.facebook.com/blog/post/377/) at [f8](https://fbf8.com), Facebook's developer conference.

Facebook's open graph (as well as Twitter's card system which we will look at next) works with meta data that you add inside your web pages' <head></head>. The same place we just put our <title>. In the case of Facebook's open graph protocol there are *four* properties that are required.

### Required Open Graph Markup

[facebook screenshot with areas called out](imgurl)

The four required open graph properties Facebook requires are:  

* title
* type
* image
* url

####Title
The first property Facebook requires is the Title tag, which is the title of your object as it should appear on Facebook.

[callout title](imgurl)

Here is how my example will be titled when the HTML document is shared on Facebook.

<meta 
  property="og:title" 
  content="Forlorn Feline"
>

If you create a title that is different than the original title Facebook will give you an error when debugging your page. Facebook allows the difference but it won't validate 100%. I do not know why Facebook frowns on this, if you know why let me know!

####Type
The second property Facebook requires is the [type of object](http://ogp.me/#types) it will be showing users on its platform.

[callout website](imgurl)

This image doesn't represent [music](http://ogp.me/#type_music) or [video](http://ogp.me/#type_video). It isn't an [article](http://ogp.me/#type_article), [book](http://ogp.me/#type_book), or [profile](http://ogp.me/#type_profile) either. All we are left with is the fact that our content lives inside an HTML document, which when uploaded to a web server, becomes a [website](http://graph.facebook.com/schema/og/website).

<meta 
  property="og:type" 
  content="website"
>

####Image
The third property Facebook requires is an image that represents our object. This one is pretty simple!

[callout image](imgurl)

<meta 
  property="og:image" 
  content="http://ryanallen.com/img/forlorn-feline.gif"
>

####URL
The fourth and final property Facebook requires is the URL users will experience when interacting with the object.

[callout url](imgurl)

Just like the image property this one is pretty simple.

<meta 
  property="og:url" 
  content="http://ryanallen.com/forlon-feline.html"
> 

That does it for everything that is required. It's time to get more abstract with the meaning we are injecting into our content, and for that we need to identify our target audience.

####Target Audience

The point of this article isn't to teach you how to identify your target audience. I do however, want to impress upon you the importance of knowing who that is. When you are building context into your content you need to know who you want discovering your content, and what they should learn about that content.

For the content in this article, the image of the unhappy looking cat, the target audience is a web designer looking to learn more about discoverability (you). Let's see what that looks like next in the optional markup facebook understands.

####Optional Abstract Markup
We can add some [additional markup](http://ogp.me/ns/ogp.me.ttl) like a [description](http://ogp.me/ns/ogp.me.ttl), which while not required, makes it much more interesting for anyone who happens upon our content.

So what should our description be? It should be relative to the target audicence.

[callout description](imgurl)

<meta 
  property="og:description" 
  content="Vincenzo the cat is sad that no one is discovering the onine content he worked so hard to create. Such hurt. Very Sadness."
>

Great!

Remember how I told you that Twitter works in a similar way to Facebook's Open Graph Protocol? Let's take a look at it next!

##Twitter
[final twitter card example](imgurl)

Twitter requires five properties compared to Facebook's four.

* card type
* attribution
* title
* description
* image

Most of these properties don't actually require us to do any additional work. Why is that?

"When the Twitter card processor looks for tags on your page, it first checks for the Twitter property, and if not present, falls back to the supported Open Graph property. This allows for both to be defined on the page independently, and minimizes the amount of duplicate markup required to describe your content and experience." [source](https://dev.twitter.com/cards/getting-started#opengraph)

###Minimizing Duplicate Markup
That's great! The tags we don't need to duplicate (though you could if you had a reason to) are: 

* og:title
* og:description
* og:image

Three down, two to go!

###Card Type
[callout card type](imgurl)

First we will tell Twitter the [type of content](https://dev.twitter.com/cards/types) we are sharing.

Let's set this card to the default *Summary Card* when the HTML document is shared on Twitter.

<meta 
  name="twitter:card" 
  content="summary"
>

Great! That was simple.

###Attribution
[callout attribution](imgurl)

Twitter requires an account to be attributed with a twitter account belonging to the content creator and/or content owner. If the content is owned by a company page, or a company department, (or exists on the company site but isn't owned by the company) you can use a site style attribution.

Here is how this will look if hosted on my [personal site](http://ryanallen.com):

<meta 
  name="twitter:creator" 
  content="@ryanallen_com"
>

Here is how it would look if webdesign.tutsplus hosted the HTML:

<meta 
  name="twitter:creator" 
  content="@ryanallen_com"
>
<meta 
  name="twitter:site" 
  content="@wdtuts"
>

Twitter will need to authenticate and white-list the domain for each type of Twitter Card. It is simple and automated. I don't know what is involved if you get blacklisted. If anyone has experience with this I would enjoy learning more.

That's it for Twitter! Good thing we did Open Graph first, Twitter allows us to save a lot of time by working with other platforms to the best of its ability. Thanks Twitter!

Time to revisit the search engines for some new, contextual, and exciting ways to optimize your SEO!

##Microdata and Search Engine Optimization

"On June 2nd [2011] we [Microsoft] announced a collaboration between Bing, Google and Yahoo to create and support a standard set of schemas for structured data markup on web pages. Although our companies compete in many ways, it was evident to us that collaboration in this space would be good for each search engine individually and for the industry as a whole." - [Michael O'Connor](http://blog.schema.org/2011/07/on-june-2-nd-we-announced-collaboration.html)

[Microdata](http://schema.org/docs/gs.html) is different from the other markup we have already structured in that it does not live in the document head.

We will use microdata to infuse context into our content in our HTML document's body. [Search engines will use our data to improve the discoverability of our content](https://support.google.com/webmasters/answer/99170) for their users.

The machines believe what we tell them. For now at least...

Before we add Microdata to the content inside our HTML document's <body>, let's take a look at everything we have done so far.

###Required Microdata Markup 

The following tags are required for every item you wish to build meaning into. 

* Item Scope
* Item Type

First we [need to identify](https://schema.org/docs/full.html) the *thing* we are describing.

Let's have some fun with semantics and build some context or meaning into our content aimed at our target audience.

Remember we have only one singular piece of content. What is one obvious bit of meaning contained within our image?
[img](url)

Well, it sure looks like a cat. That's great since designers love cats! What *thing* best represents a cat in the [schemas markup available](https://schema.org/docs/full.html) to us to use?

The meaning contained in this image is probably not an [action](https://schema.org/Action), [broadcast service](https://schema.org/BroadcastService), [event](https://schema.org/Event) [medical entity](https://schema.org/MedicalEntity), [place](https://schema.org/Place). It is definitely a [creative work](https://schema.org/CreativeWork), or more specifically, [visual artwork](https://schema.org/VisualArtwork). 

Great! Let's set the type of item contained in this section as Visual Artwork.

<section
  itemscope
  itemtype="https://schema.org/VisualArtwork"
>
  <img 
    src="http://ryanallen.com/img/forlorn-feline.gif"
  >
</section>

That is all that is required, the problem though is our content is still mostly meaningless. Google, Bing, Yahoo and Yandex are now 100% certain that our content is a visual artwork, but nothing else. Let's add some more meaningful context aimed at our target market, web designers.

####Optional Microdata Properties

It isn't necessary for me to [list all of the properties](https://schema.org/VisualArtwork) you can use with the Visual Artwork item type, here instead are some relative to web designers, who we identified as our target audience.

Let's start by declaring all the things about this content that aren't abstract but are instead concrete, firm, and unchanging in their meaning. 

#####Image

First, this is an [image](https://schema.org/image) with a source location (src) on the web. That will remain true.

<img 
  itemprop="image"
    src="http://ryanallen.com/img/forlorn-feline.gif"
  >

#####Height

Our image has a physical [height](https://schema.org/height) of 300 pixels.

<img...>
  <meta
    itemprop="height"
      content="300px"
  >

#####Width

Our image has a physical [width](https://schema.org/width) of 600 pixels.

<img...>
  <meta
    itemprop="width"
      content="600px"
  >

#####Artform

Our image is an Illustration [artform](https://schema.org/artform).

<meta
  itemprop="artform"
    content="Illustration"
>

#####Material

The [material](https://schema.org/material) our image was created with was digital.

<meta
  itemprop="material"
    content="Digital"
>

#####Author

[I](https://twitter.com/ryanallen_com) am the [author](https://schema.org/author), or creator, of the digital illustration.

<meta
  itemprop="author"
    content="Ryan Allen"
>

#####Audience

Lookin' good! Let's now add our target [audience](https://schema.org/audience). 

<meta
  itemprop="audience"
    content="web designers"
>

#####Educational Use

Next let's set the type of [educational use](https://schema.org/educationalUse) we intend for this image, which is an example in this case.

<meta
  itemprop="educationalUse"
    content="example"
>

#####Family Friendly

There is nothing about this that is NSFW, so let's make sure that is clear.

<meta
  itemprop="isFamilyFriendly"
    content="true"
>

#####Character

What did we name our cat [character](https://schema.org/character)?

<meta
  itemprop="character"
    content="Vincenzo"
>

Oh yeah. That's a pretty awesome name, though it is moving into a more abstract realm. Things are [about](https://schema.org/about) to get all abstract now. 

#####About

Let's add some more context [about](https://schema.org/about) the situation in our [image](https://schema.org/image) related to our [target audience](https://schema.org/audience). 

<meta
itemprop="about"
  content="Vincenzo the cat is sad that no one is discovering the onine content he worked so hard to create. What should he do!?"
>

Nice. Let's finish this off with a list of comma delimited, targeted, and relative [keywords](https://schema.org/keywords) to bump our content's discoverability factor over 9000.

<meta
itemprop="keywords"
  content="designer, design, web design, seo, discoverability, open graph, twitter cards, microdata, google, bing, microsoft, yahoo, yandex, content, context, semantics, meaning, sad, cat, animation, gif, cute, illustration, tutsplus"
> 

##Validate
Validate your code with [Google](http://www.google.com/webmasters/tools/richsnippets), then [Facebook](https://developers.facebook.com/tools/debug/), and finally with
[Twitter](https://cards-dev.twitter.com/validator). Fix any errors you come across like the professional that you are.


##Summary
So what does everything look like together?
[all the code](codepen url embed if possible)

By building meaning into our singular piece of content with open graph, twitter cards, and microdata, we have improved the chance that our target audience will discover it, share it, and create t-shirts with it printed on the front.



---
Validation Proof for Ian:

Twitter: 
https://www.dropbox.com/s/y6aks0946fuiw0m/Screenshot%202015-02-19%2014.28.21.png?dl=0

Facebook:
https://www.dropbox.com/s/fe9q0kzb4wwvzj6/Screenshot%202015-02-19%2014.31.47.png?dl=0

https://www.dropbox.com/s/5uvcvbkhhpnvxjp/Screenshot%202015-02-19%2014.32.04.png?dl=0

https://www.dropbox.com/s/7iw6r5rhl46uddn/Screenshot%202015-02-19%2014.32.34.png?dl=0

Google:
https://www.dropbox.com/s/omxvshu92evwyb6/Screenshot%202015-02-19%2014.34.05.png?dl=0

