Symantec markup and how it's used by people and computers. 

Structural markup helps no one. 

Semantic helps 
People 
future you
Other programmers

Computer
Seo
Screen readers

How does it help?



Semantic class names or presentational? When to use what. 

Full presentational is the declaration name. How to define abstraction rules?

Combine the declaration names?

Is it possible to create rules for abstraction depth?

Meanings change. Today this vertical page might be adaptive tomorrow. This circle might become a square for the square shaped people of squaredom. They hate blue circles. 

How can our names change to reflect meaning? We change them. How do we avoid that?

Should selector names be semantic?

How abstract should our naming conventions be?

How do we map depth in terms of ideas?

META



CORE PROBLEM:
Presentational markup is not user friendly

A Potential Problem With Front-End Frameworks
Understanding WTF You Did Last Year

SOLUTION:
Teach the reader to think semantically by giving them a better understanding of what that means.

/// TITLE BRAINSTORMING AREA, CAUTION LIGHTING HAS BEEN KNOWN TO STRIKE

## why the words you use in your class names matter. 

## Semantic Vs Presentational Markup
## What Exactly is Semantic Markup?
## Future Proof Your Markup
## You Probably Don't Know What Semantic Markup Really Is /// hooray for linkbait headlines!
## You Say Potato, I Say a Starchy Tuberous Crop

/META

BEGIN

Separate semantics from presentation.



It's easier to maintain

What is easier to maintain?
<div class="box21 bg80 column corners3 corner-br-8">
.box21 {
  display:flex;
  flex:21;
...
...
...
...



or this

<div class="screen">
.screen {@include display;
         flex:11;
         background-color:hsl(100,20,40);
         flex-direction:column;
         border-radius:2rem;
         border-bottom-right-radius:6rem;
}


Refactor your code. You'll thank yourself for it.

Let's pretend you are doing work for nintendo. They contact you and ask you to update a marketing page they created for a new game. The screen on their current website is a dark grey when it actually needs to be a dark green. You have 10 minutes until the President of the company makes an announcemnt regarding this new game. Which one of these examples looks like it would be easier to update



## Twiddling

"I would however, support an assertion in the architecture document that important information SHOULD be stored and (optionally) delivered with markup that is as semantically rich as achievable, and that separation of semantic and presentational markup, to the extent possible, is architecturally sound."

Separation of semantic and presentational markup, **to the extent possible**, is architecturally sound /// Interesting that it isnt assumed fully possible.

It may not always be fully possible to abstract every class into one that has more meaning. Sometimes a structural container is just a container.

front end frameworks need to work for multiple people. then need to be generic.
therefore classnames may be generic.

here is an example of a custom presentational framework (it is a grid, an hsl coloring system)

Let's use an idea. I want to build a layout that looks like a gameboy to place an illustration inside. The illustration is the loading screen from the fictitious video game studio I work at called "Handsome Game Developers", and I want the website to resemble the platform we are launching our new game on. The gameboy.


A potential problem with existing front-end frameworks lies at the heart of the idea. The idea that an existing framework is more efficient because we don't have to spend time initially creating all of our desired patterns. This idea is sound. If I'm familiar with a frameworks style guides I can prototype an idea very quickly. It only becomes a problem when these frameworks are deployed  is that they need to understandable by more than one person. This means that selector names need to be less abstract. Our human minds abstract ideas to better understand them. The 5 small flaps of dead cow carcass sitting in in my lap might sound odd to you based on that description, but completely normal if I were to abstract the parts of it into the form, icon, or symbol we have named 'wallet'.

How Should I be Naming my Classes?
Semantically of course!

What does that mean?

http://www.w3.org/2001/tag/doc/contentPresentation-26.html

Border4px

What if I want one box to be border 5px? I'm going to need to change the html markup and not just the css. 

Semantically as possible when possible. Easier to maintain and understand by humans. Dont get too crazy.


-----


how should i name m classes?

semantically, different levels of abstraction?

example chair

lets take an example and move it through different levels of abstraction

Should there be rules for levels of abstractions? maintianing the same level?

rectangle

box

container

page

page background


dont get too specific, it needs to be flexable like a component, so you can use it across multiple projects.


examples

blue page background

maintain the same level of abstraction across your project.



-----



Do You Know How You Should Be Naming Your Classes?

"Semantics in HTML is always a hot topic. Some people strive for it at all times. Some people critisize a dogmatic adherence to it. Some people don't know what the heck it is." - [Chris Coyier](http://css-tricks.com/semantic-class-names/)

The first step is admittance. I don't know "what the heck" semantics in HTML really is.

Many people think it is about [solving problems](http://www.w3.org/2001/tag/doc/contentPresentation-26.html). That's great! We want to be good designers and developers by solving problems instead of creating them.

It took me several readings of the semantic and presentational markup definitions before I thought I knew what they meant. It then took another few years before I really knew what they meant. Then another few weeks where [I didn't know what anything meant](http://en.wikipedia.org/wiki/Existential_crisis).

Presentational markup can make it difficult to communicate ideas and meaning to humans, which makes it difficult to read and less efficient to maintain. This is why [everyone agrees](http://en.wikipedia.org/wiki/Semantic_Web), semantic markup is the [cats pajamas](http://bit.ly/catsPajamas).

If you are even a little bit unsure on how best to include semantic markup in your HTML then this is the article you've been waiting for! It's time to think semantically.

### Markup

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

Now that you have a clearer understanding of what LaTeX... err, **markup** is. Let's explore the differences between *presentation semantics* and *semantic markup*.

### Presentational Markup

Formal Definition:

"In computer science, particularly in human-computer interaction, [presentation semantics](http://en.wikipedia.org/wiki/Presentation_semantics) specify how a particular piece of a formal language is represented in a distinguished manner accessible to human senses, usually human vision."

In plainer terms, it describes how a piece of the document that is being presented to you, looks to you.

Let's try a fun experiment!

If you have a piece of paper and pen nearby I want you to draw the image that I'm thinking of. It is of three 2D rectangles. Two of the rectangles are taller than they are wide.

What does your drawing look like? Send a picture of it to me on [twitter](https://twitter.com/ryanallen_com) or post it in the comments!

Here are several ways you may have interpreted my presentational description:

![Illustration of Rectangles #1](imgurl)
![Illustration of Rectangles #2](imgurl)
![Illustration of Rectangles #3](imgurl)
![Illustration of Rectangles #4](imgurl)

None of those drawings resemble each other in a way we can quickly distinguish. We are not able to group those images into a single clear, defined and meaningful category. The only way we can quickly categorize these images is at their most general form, *rectangles*. If we study the images long enough other patterns may begin to emerge, but how deep into our psyche are we willing to go?

So, why is this a problem?

You and anyone else who will be editing this code in the future are the users in this case. Months and years from now, do you want to spend hours, days, or weeks trying to figure out what you were thinking? Of course you don't. That's crazy talk.

Presentational markup can make it difficult to communicate ideas and meaning to other people and to future you, which makes it difficult to read and less efficient to maintain. This is why [everyone agrees](http://en.wikipedia.org/wiki/Semantic_Web), semantic markup is the [cats pajamas](http://bit.ly/catsPajamas).


### Semantic Markup

Formal Definition:

"[Semantic Markup](http://en.wikipedia.org/wiki/Semantic_HTML) is the use of HTML markup to reinforce the semantics, or *meaning*, of the information in web pages rather than merely to define its presentation or look."

Even the formal definition is easier to understand. So how do we express *meaning* in our markup?

Let's try the rectangle experiment again, however, this time we will communicate the [meaning of the forms](http://en.wikipedia.org/wiki/Theory_of_Forms) instead of their presentation. 

Draw this next image that I'll describe to you semantically.

Draw a chair and post it in the comments.

Did you draw it with three rectangles, two of them taller than they are wide and the third wider than it is tall [like I did](imgurl)?

It's the same image I described in the first example. While your chair might not have looked exactly the same as mine, it will probably look like a chair. What does your first drawing look like? 

Why is this important? 

If you drew one new image of rectangles every day for a year, how quickly would you be able to go through that pile of paper and find the one you drew on the 144th day? What if the stack of papers got shuffled? What if your mom wanted to find that drawing to hang on the fridge, how would you explain to her how to find it?

When you are writing semantic class names in your CSS, try to embed as much meaning as you can with the names. Don't name that class .box {...} when you can name it .logo {...}. Or better yet, [header__logo](http://webdesign.tutsplus.com/articles/an-introduction-to-the-bem-methodology--cms-19403).

Presentational markup has its uses, building rapid prototypes is one of them, but long term it is difficult to maintain and difficult for other designers and developers to work with. If you want to work with teams of people take the time to think clearly about the work you are doing and take the time to refactor your class names. It will not only make you a better person to work with, but a more focused, thoughtful, and precise individual.

As a final example here is some [presentational markup](http://codepen.io/ryanallen/pen/emEjpV) from an upcoming article. Can you figure out what I'm building based on my markup?

### Semantic or Presentational?

Pop quiz time! Which version is semantic?

[note - if no better option is found hack all this stuff into a codepen for an answer reveal](codepenurl)

<div class="box">
or
<div class="tv-screen">

<i>italic<i>
or
<em>emphasis<em>

"two eggs, potatoes, cheese, peppers, salsa, and a tortilla"
or
"breakfast burrito"

[/note]
