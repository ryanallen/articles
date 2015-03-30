With over 20 million downloads on iOS, Android, Windows Phone and Windows 8, Bryan Mitchell is a force in the gaming industry. He has been developing games for over half a decade and has been programming for more years than some people have been alive. I'm honored to have the chance to interview Bryan about what it's like to develop an immersive horror experience that looks incredibly terrifying!

---
[video](https://www.youtube.com/watch?v=ZQsyr4QX-GU&t=0s)
***That video gives me goosebumps! You mention in the video that "they said this couldn't be done". What's an example of a difficult problem and how do you begin to solve it?***

[Inertial navigation](http://en.wikipedia.org/wiki/Inertial_navigation_system) on mobile devices, and [single camera depth estimation](http://papers.nips.cc/paper/2921-learning-depth-from-single-monocular-images.pdf). I had a subscription to [deepdyve](https://twitter.com/deepdyve), and read through many unsuccessful attempts at making them work on the iPhone. Computer vision, on the whole, is full of unsolved problems people have been working on for 20 years. Even the human eye and brain aren't perfect, we are fooled by camouflage and many kinds of optical illusions.

***That's interesting, I hadn't thought about the human eye not being perfect before. What are some other interesting things this project has made you think about?***

I enjoy reading about things like [AI-complete](http://en.wikipedia.org/wiki/AI-complete), and [Computer vision](http://en.wikipedia.org/wiki/Computer_vision).

Imagine someone [blind from birth](http://en.wikipedia.org/wiki/Molyneux's_problem), all of a sudden being able to see. They would essentially be like a baby seeing for the first time, and would have to learn what this new input meant.  They would have to build all of the associations we built, like if a baseball is getting bigger its about to hit them.

Most humans can quickly and efficiently tell which pixels in an image are people and which are not, but we have to use green/blue/black screens to help computers tell background from foreground. We understand the context from the content from many sources. How do you think you understand what a person is with all the differences that are between people? Two people standing next to each other may be different heights, genders, body types, one wearing a suit while the other is nude, etc. Yet you as a human understand that there exist two people on the screen. We have to tell the computer all the little things that could exist for an object to be called 'human'.


Solving these issues required some out of the box thinking, and an understanding of film/lighting was invaluable. Almost all of computer vision is based on advanced mathematics and signal processing. I tried to approach it in an experimental way, in a less mathematical way. 

***Why was knowing about film and lighting useful in solving problems, and what is an example of one of the problems that knowledge solved?***

Knowing that light falls off at an inverse squared rate was useful, as was having an intuition about how light is reflected, which motivated exploring more *visual sensory* approaches than *signal* ones. The early days of computer vision were a lot like that.

***What the initial spark of motivation was for [Night Terrors](https://www.kickstarter.com/projects/1988291115/night-terrors-augmented-reality-survival-horror)?***

Bryce, my producer, pitched me "[Paranormal Activity](https://twitter.com/oren_peli) as an augmented reality game" and it immediately interested me. The movie is amazing, it's someone walking around with a camera, and I thought if we could turn players into that character and do everything in real time it would be incredible!

***The found footage movies are incredibly immersive, which was a big reason why they are scary for me. How terrifying is your game?***

It's creepy as hell just walking around in the dark, with only the LED as light, wearing headphones that route the microphone feed, with NOTHING being added! I've scared myself so many times. Even a couple times today in fact.

***Will there be micro transactions where I can pay to gain my real-life sanity back?***

Haha. No. Once it is gone, the game keeps it.

***Excellent! Thank you again for your time Bryan and best of luck [on your kickstarter for Night Terrors!](https://www.kickstarter.com/projects/1988291115/night-terrors-augmented-reality-survival-horror)!***