---
title: Leah is more fun than programming
tags: tech, leah
layout: post
---
I know I have been really bad about about keeping up with my blog.  In the past I would make long senseless posts about wushu between the fun adventure posts.  Well, since I haven’t been doing much of that (and when I do I mostly just work basics and get sore), I don’t have that stuff to post about.  Now, there are more adventures, nearly all inspired or caused my the little miss, but work has been nuts so I am falling behind on them.



I could replace the wushu posts with programming posts, but I am not sure that is what my audience (read: Kelly) wants to read about. Not that they wanted to read about wushu, but it was an easy topic that was constantly on my mind. So now that programming is my idée fixe I figured maybe I should write about that. So here goes:

I just spend the last few days trying to figure out some weird C Runtime Library (CRT) issues with our new installer.  We had always built things as multithreaded, not multithreaded dll, so it was never a problem. We would much rather have larger exe’s than to redistribute the msvc dlls.  Well, turns out that you can’t build  C++/CLI mixed mode code as multithreaded, so you have to dynamically link to the CRT if you want to build with /cli.  Drat. I just want to statically link and be done with it.  This was annoying because I didn’t notice until after I deployed on a machine with out the Visual Studio installed, and it would crash hard and give me this fancy FileNotFound error.  I read all about manifests and how to embed them, but Visual Studio’s linker automatically does that for me – eventually I figured out that we were trying to use the redist dll’s from VS2005, but built out lib with VS2005sp1!  Egads!  Now that I have the correct version of the dlls, I think we are in business. 



And that’s why they call them business socks.



Hmm, maybe, I shouldn’t write about that stuff – and if I want to I will need to make the articles useful, and that takes lot of time.  Plus my audience really just wants to hear A) Stories about Leah B) Funny stories or C) Funny stories about Leah.  



They would prolly love to hear about how Leah got my wallet, emptied it’s contents, stuck the post-it’s on her belly and handed me the empty shell with a big grin on her face. I think she hid one of my credit cards. Hopefully this is not foreshadowing.
