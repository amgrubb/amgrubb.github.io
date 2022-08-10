---
title: 'Presence Conditions Within BloomingLeaf Tool'
date: 2022-08-03
excerpt: Venus Nguyen, Xinran Bi
permalink: /posts/2022-08-02-presence-conditions
layout: archive
---

**Presence Conditions Within BloomingLeaf Tool**  
**_2022 SURF Abstract by Venus Nguyen and Xinran Bi_**

We introduced presence conditions in BloomingLeaf to visualize changes within the goal model’s evolution. BloomingLeaf is an analysis and modeling tool that allows users to model goals that evolve over time. These models consist of intentions, actors, and links. By evaluating the changes in intentions over time, users are better able to understand future project evolutions and make decisions from them. A presence condition states whether a model element (i.e., intention or actor) exists at a particular time point in the project’s evolution.

We first determined how to make an intention invisible. The “element ID” in each intention allowed us to change the visibility of each intention, so we successfully made intentions disappear in the CSS code. We then identified intentions with their IDs and have them stored automatically from the given goal models.

Next, we started looking through the front-end code and testing out possibilities of getting intentions within our model to disappear on a time-based condition. Once a user simulates a goal model within the analysis window, BloomingLeaf creates a path of timepoints that shows the progress of a goal model through a set span of time. At each timepoint the Satisfaction value of each intention changes. Users are able to step through each time point and examine the current state of the model with the use of a slider. We tested the disappearance of intentions based on satisfaction values to allow the visibility of elements more reliant on the prebuilt attributes. Satisfaction values are values assigned to intentions indicating whether the intentions are satisfied or denied within the evolutions of the model. Ultimately, we validated we could make intentions appear or disappear with the given satisfaction values.

We then grouped actors and all the intentions within it to change the visibility of elements on the actor-level instead of a single intention. We found a list of actors containing their embedded elements (intentions and links) to make a specific actor disappear with all its embedded elements. In future work, we hope to implement presence conditions with Actors.


<img src="/images/presence-conditions.png"
     alt="Presence Conditions Demonstration"
     />

