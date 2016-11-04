---
layout:     post
title:      "NP completeness reduction"
date:       2016-04-02 23:01:00
author:     "Avi Srivastava"
header-img: "img/post-bg-01.jpg"
---

<p>GSAD is a short form of Genome-Scale Algorithm Design[1] (a book used for reference) and an abbreviation for blog name to identify the content.</p>

<p>As a computer scientist, we hear terms like P, NP, NP-complete and NP-hard a lot in our quest. These tractability related terms are quite intuitive
	 to understand and really useful when you are designing and proving the complexity of your algorithm. One thing which always confuses me is the 
	 process of reduction and it's direction. As we know to prove a problem X as NP-hard we have to reduce some known NP-hard problem to X and then 
	 we say X is as hard as any NP-hard problem. But why not the other way around? How do you remember this counter-intuitive reduction process?</p>

<p>The trick to this lies on the fact that normally if we know a problem A is solvable then we just reduce the required problem B to A and then say 
	since A is solvable then B is solvable too. But in the case of NP-hardness, the question is just the opposite i.e. problem A is not-solvable 
	(actually we don't know even B is solvable or not) and hence the opposite direction of reduction.</p>

<p>A more intuitive way which helps me remember it as follows*:
Assume:
problems as a circle.
problem A is P: if a single query point Z is known to be inside a circle A.
problem B is NP: if a single query point Z is known to be outside of circle B.
reduction from A to B as moving circle B inside A.</p>


<p>First, let's take the problem A which is P (i.e. a query point Z is known to be inside circle A) and a query problem X which we want to know is 
	P-solvable or not. Now, let's reduce A to X. By our definition of reduction if we reduce problem A to X we move circle X inside A. 
	Then question arises are we sure that known point Z(which was inside A) will also be inside X?? No, it's not always true since a point can always 
	be inside A and outside X which doesn't prove anything. Now if we reduce X to A then we are actually moving circle A inside X and any point Z 
	inside A will always be inside X and hence, X is P-solvable.</p>

<p> Now let's go to our original motivation. Take problem B which is NP i.e. we know a point Z exist which is outside circle B and there is problem 
	X which we need to prove as NP. Now let's reduce X to B i.e. move circle B inside X. So are we sure if a point Z which is outside B will be 
	outside X?? No, not always, Hence proves nothing. Now let's try the other way around let's reduce B to X i.e. move circle X inside B, what will 
	happen now? As we know point Z is always outside B then we can say it'll definitely be outside X and hence we can say X is NP if the reduction 
	is done from B to X.</p>

Reference:
[1] http://www.cambridge.org/us/academic/subjects/life-sciences/genomics-bioinformatics-and-systems-biology/genome-scale-algorithm-design-biological-sequence-analysis-era-high-throughput-sequencing
* I am no way saying this is the right way. This just helps remember the process in an intuitive way.