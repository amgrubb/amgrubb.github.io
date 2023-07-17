---
title: "Slide to Hide: Allowing Users to Specify Elements' Presence Intervals"
date: 2023-07-07
excerpt: Xinran Bi, Emily Kung, Karenna Kung, Caroline Zouloumian
permalink: /posts/2023-07-07-presence-interface
layout: archive
---

**Slide to Hide: Allowing Users to Specify Elements' Presence Intervals**  
**_Xinran Bi, Emily Kung, Karenna Kung, Caroline Zouloumian_**

BloomingLeaf is a tool used to create and analyze Tropos goal models. The elements of a model are actors, intentions, and links. Actors’ desires are expressed as intentions, and intentions can be linked together with different types of relationships. We can simulate possible paths of how satisfaction values change over time for each intention, while taking into consideration the constraints on an intention’s satisfaction values and its relationships to other intentions.

Sometimes, an element of the model is not present during the entire timeline. For example, let’s imagine Molly is driving Emma home. They want to choose music that fits both of their tastes. Molly loves Taylor Swift, while Emma wants to listen to The 1975. Once Emma is dropped off, Molly doesn’t have to consider Emma’s wish for The 1975 anymore and can take it off the playlist. The actor representing Emma is not present during the whole car ride, so their music tastes only need to be considered for part of the car ride. This scenario demonstrates the need for presence conditions. We aimed to create a front-facing interface so that a user could specify that an actor or intention appears part way through the time period, disappears part way through the time period, or disappears and later reappears during the time period.

To this end, we updated the tool such that, upon clicking on an actor or intention, the inspector window includes a slider with two sliding values representative of time points between the minimum and maximum times of the model. The user can use the sliding points to specify the start and end values of a time interval, and can click a checkbox to indicate whether they are specifying an inclusion or exclusion interval. Additionally, both slider limits and the stored intervals change according to the maximum range available to the actor or intention. Intentions belonging to an actor cannot be present while their actor is not, and neither actors nor intentions can exist outside of time point 0 and the maximum time point. The list of exclusion intervals for all intentions is also viewable in the Assignments Table tab of the tool. From this view, the user can also add or delete excluded intervals.

After setting the intervals using the sliders, when the user simulates a path, actors, intentions, and their links do not appear at time points that are within their exclusion intervals, enabling the user to envision only the relations in the model that are relevant at the given time point.

Future work may include considering presence conditions in the Next State feature. This feature allows the user to choose specific satisfaction values for each intention at a certain time point, so incorporating presence conditions would mean that the user can only select satisfaction values for intentions that are present at the given time point.

<img src="/images/pc-view.png"
     alt="Screenshot of Actor view with presence conditions."
     />

