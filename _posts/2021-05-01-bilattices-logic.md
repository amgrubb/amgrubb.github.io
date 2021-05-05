---
title: 'Thesis: Bilattices and the Logic of Goal Modeling'
date: 2021-05-01
excerpt: Isabel Montesanto
collection: projects
permalink: /posts/2021-05-01-bilattices-logic
layout: archive
---

**Bilattices and the Logic of Goal Modeling**  
**_Senior Honors Thesis by Isabel Montesant_**

<!-- Lucy completed her seniors honors thesis with Prof. Grubb and received highest honors!-->


>_Thesis Abstract:_
Goal modeling is an area of software engineering that allows stakeholders, in domains from software to public planning, to break down their intentions visually and make trade-off decisions. Currently, Grubb et al. are building a web application, BloomingLeaf, that would allow stakeholders to build and to automatically analyze goal models within the Tropos framework. Practical concerns suggest that the best way to allow users to make models large enough to represent most real-world projects is to have them to create smaller submodels that the application automatically merges into a big-picture view. However, the existing merge algorithm is unable to merge information about goal fulfillment in most cases where it differs between submodels.

This project uses the bilattice, a flexible logical formalism introduced by Ginsberg (1986), to propose solutions to the remaining gaps in the model merging algorithm. Bilattices are sets of values with two related orderings, the first ordered by truth vs. falsity (or other dichotomous qualities), and the second by amount of information. The formal syntax BloomingLeaf uses to record the fulfillment of goals is modeled using a nine-element bilattice of &lt;evidence for satisfaction, evidence for denial&gt; pairs. The bilattice structure suggests two uniform approaches to reconcile information from sources that disagree: gullibility (accept everything) and consensus (accept what the sources agree on). The applications portion of this project outlines the results of applying the consensus approach to fulfillment values that differ across models. This strategy produces obvious solutions for most merge cases, and a few promising solutions for the remaining cases. 

Isabel's thesis was submitted to the Logic Program and was co-advised by Jay Garfield.