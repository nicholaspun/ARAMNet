# ARAMNet

_Disclaimer: I'm not affiliated with Riot Games. Pls don't sue me Riot. League is great. ARAM is fun. I just wanted to do some math and ARAM presented such a nice opportunity to me :")_

Side note: I don't know what it is with me and finding math problems in League, but I just realized that I also did [TFT math](https://gist.github.com/nicholaspun/83bd9d886decbdf1b4121b272b4a8018) 5 months back.
That stuff was more combinatorial though, which in a sense will be complete opposite of what I'm about to present.

If you know what ARAM is, I'll leave this to keep you busy for a sec: How do you make champion selection fair when everyone comes in with varying pool sizes?
In particular, try to cook up situations where champ select is definitely skewed.
(Jeez, I feel like a math textbook telling the reader that something is an exercise)

Now for those who don't know what ARAM is, imagine a swimming pool with 152 unique balls.
10 people come in to select balls, _but_ some people paid more to get in.
So the overseer decides to do something like this: Those who didn't pay as much can't select from some fraction of the pool (the fraction scaling by the amount).
Those who paid an ample amount can select from the entire pool.
Who has the advantage here?
Say I paid less and I pick a ball before anyone else does.
Well, no matter what I pick, since the rich guys have access to the entire pool, I'm going to pick a ball that they have a chance of picking as well.
On the contrary, if the rich guy picks first, there's a chance that they pick a ball from the fraction of the pool that I _don't_ have access to.
In this case, their selection doesn't affect me.

So, in one ordering, the person going after _is_ affected and in the other, the person going after _might_ be affected.
And, this is just 2 people, what happens when there are 10?
No matter how we order people, there's probably no way to make it _completely_ fair, but could we make it _as close to_ fair as possible?

That's the motivation of this project.
I really try to solve it completely, but end up failing and falling back to finding empirical evidence.
Nevertheless, it was fun for a while.
I prove some easy propositions, write some code, train some neural networks ... all because I can't stop doing math while playing League.

Anyways, I hope you have as much fun as me.
Check out the code (the `.ipynb` file) and please read the writeup.
If this problem is much more obvious to you than it was to me, please tell me!
I don't mind being dumb if I still get to learn math. 
