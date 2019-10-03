---
  title: Degrees of Freedom
  date: "2019-10-01"
  Author: "Giacomo Bignardi"
  menu: main
  tags:
- Art
- Creative Computing
- Genetic
description: A generative Art about freedom, constrictions and probailistic propensities and how they emerge from the relationship between coded information and complicated environments.

---
A blog post on a generative Artwork I did in the past. It's about freedom, constrictions and probailistic propensities and how they emerge from the relationship between coded information and complicated environments.

<!--more-->

## Introduction

We are in the (post)genomic era. But what does it mean? And how can we interpret the results that are emerging from the genetic sciences? E.g., what does it mean to say that 30 to 60% of the variation in one's [differences in political ideologies can be accounted for by genetic factors](https://link.springer.com/article/10.1007%2Fs10519-014-9648-8); that [polygenic risk scores might predict up to 11 percent of differences in educational attainment] (https://doi.org/10.1038/s41588-018-0147-3); [or that music ability show substantially heritable components](https://link.springer.com/article/10.1007%2Fs10519-009-9260-5)? 

## Deterministic?

A common thought which is usually associated with the word genetic is *determinism*: it's pre-written, it's fixed, it's a [blue print](https://www.amazon.ca/Blueprint-How-DNA-Makes-Who/dp/0262039168). However, as nicely pointed out by Fisher ( [which knows what the subject is about](https://www.mpi.nl/people/fisher-simon-e) ) there is nothing more misleading than that:

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">Your genome is not a blueprint. A thread about misleading metaphors in science communication... 1/11</p>&mdash; Simon E. Fisher (@ProfSimonFisher) <a href="https://twitter.com/ProfSimonFisher/status/1018486635409891328?ref_src=twsrc%5Etfw">July 15, 2018</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>


Here I used a generative art piece to dive deep into the topic. A generative art, put simply, it's just a media that has been written in some sort of programming language (for this piece I used C++, and, to be more precise, I used an open source library, called OpenFramework, which made my life way easier). Once the code was written, the art piece unfolded by following the rules set by the underlying code. That is, it was generative. The conceptual comaprison between the code and the genetic code should be obvious now. Both are setting rules. The question is: what are those rules for? 

> "Genetics is not a puppeteer pulling our strings. Genetic influences are probabilistic propensities...Genes are not destiny. You can change... Heritability describes what is but does not predict what could be"

When someone is saying that music ability shows substantially heritable components, it says that a given percentage of the variation in music ability in a given population can be accounted for by genetic factors. How do we know that? Have you ever met some identical twins? that is indiviudals that are roughly genetically identical. Maybe you have met two twins that were both skilfull singers, talented painters, creative designers, or maybe good mathematician (i.e. when I am saying skilfull, talented, creative or good I am always making a relative judgment, that is when one is compared to the population). Just this anetocdal knowledge might make you think "It's genetic". However, observation of identical twins alone isn't enough for you to conclude anything. Indeed, it might be that the enivrionment that they shared could actually be the reason behind their ability. Those skillful twins, for example, grew up in a family of musician. Maybe was just the environmental exposure, or a aimed parenting, that shaped their musical ability.Yet you don't know. Here comes the twin method.

```
THE TWIN METHOD

Besides several tools that can be used to estimate and disentagle such genetic influences from environmental ones, 
the twin method ingenioulsy use and compare the observations of identical twins with the one of fraternal twins. 
The only difference on the source of influences between the two pairs is the genetic one (fraternal twin are only 50% genetically identical on average). 
Thus, by comparing how much identical twins are simlar between each other to how much fraternal ones are, 
we can grasp how much of, for example, musical ability is due to genetic factors and how much is due to environmental ones.

```

If we are lucky enough and we have data on the music ability of two identical twins and two fraternal twins, then we can say something about why people vary, for example, in their music ability. This is what they did in the paper [I mentioned before](https://www.ncbi.nlm.nih.gov/pubmed/19288254), and they found xx percent of the variance in musical talent (to be honest, variance in the self report talent) to be accounted for by genetic factors!

So, are people's musical abilities written in their genes? Is it determined whether you are, for example, a [good singer]() or not?


![degrees of freedom](/posts/creating-a-new-theme_files/GIf_deterministic.gif)

The gif above is from a couple of frames out of the 4500 generated ones.
Conceptually the two rectangles are a pair of identical twins (To make stuff easier I just took out the fraternal twins). Their location is their genetic potential. The potential was equal for both of the twins, since the frame was divided in a lower and an upper part with corresponsing equal potentials (remeber that all this stuff are made up). The vertical distances between any of the two rectangles (twins) represented their similarity, which was simultaneously translated in the radius of the circle on the side of the frame. To keep stuff easy, only one source of environmental difference was included: pixel brigthness. For example, the frame above shows a situation where no evnvironmental differences at pixel location were present. Finally, the set of rules were set: every twins was allowed to move (develop) from left to right, following the brightest dot on the screen. In the frame above, since the enviroment was homogeneus, that is there was no differnece in brightness at any point, developmental trajectory did not changed. 

Going back to our example, the circles would represent the similarity in musical ability between pairs. Any deviation from the standard circle would signify a different developmental trajectory in musical abilities of one of the two twins. Since the environment was homogeneus, the genetic potential determined entirley the extent to which twins resembled each other. There was variation in the population of twins, but it was entirely determined by the genetic potential.
How does this fictious visual example should thus help us in understanding *if  people do have a gene for signing ability,  if  their  musical abilities are written in their genes, and thus if it is determined whether or not you are a good singer?*

## Generative Art

Now take 3 minutes of your time to watch how the generative art unfolds over time:

<iframe src="https://player.vimeo.com/video/316463576" width="640" height="360" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe>


## So? probabilistic!

What happend? as you can see from min 2 the developmental trajectories changed, and the respective circles stared to diverge from the fixed one. Why? because of the environment. The brightness of the environemnt changed from pixel to pixel. That is the enviroment became heterogeneous. If you want to know more about the environment (terrain), you can read the original post from which this post was born (here), read the slides of a talk where I explained the process (here), or contact the artist who actually crafted the terrain (here). Nevertheless, the only thing you need to know for now, is that the brightness changed from pixel to pixel, and so did the developmental trajectories.That is, when the code was allowed to interact with the environmnet, the rules started to play their role: they started to inform the developmental trajectory, and differences among twins started to emerge.

Think about music ability. Genetic predispositions set the rules trhough which the relevant mechanism apt to make individuals differ in their musicality should develop. But that development is never indipendent from the environment. That is, there is no development without environment, there are no changes  without interactions**.
So. going back to the question about determinsitic views: are people musical abilities written in their genes? No! But, on average, there are genetic probablistic propensity that might influence the likehood of develooping musical abilities in a certain group. Is it determined whether you are a good singer or not? No! please, no. It's about average propensites. It's not about you, or me. ** The difference are of degrees, not of kind** (can you  guess why  degrees of freedom now?)


## Conclusion

To summarise, this generative art told me something. It told me a story about developmental trajectories, and how they are the results of an *&* between the genome/code/nature and environemnt/terrain/nurture. It told me how genetic propensity are propensity, not blue prints. 
It also taught me something: the rules are global, but the results of the application of such rules are local. A different terrain would have changed developmental trajectories, and the overlying probabilistic propensities. By such perspective, freedom it's a relative concept, anchored to many degrees, resulting in a "shape of the environment." 


![](/posts/creating-a-new-theme_files/ThumbnailSharedf.png)

*note(it's a little bit more complicated than this thou, indeed since also in  the heterogeneous environemnt there were region of pixel with equal  brightness surrounding one twin, I add another rule: developmental noise. That is, sometimes development trajectory were random)
** this is not completly true. Living organims genetically identical exposed to the same environemtn can differ. This is probrably due to intrinsic developmental noise, which my rules did not tak into consideration when the environment was homogeneous.