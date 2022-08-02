---
title: 'Implementing Intention Filtering and EVO in Next State'
date: 2022-08-02
excerpt: Yesugen Baatartogtokh, Irene Foster, Venus Nguyen, Thu Tran
permalink: /posts/2022-08-02-intention-filtering
layout: archive
---

**Implementing Intention Filtering and EVO in Next State**  
**_Yesugen Baatartogtokh, Irene Foster, Venus Nguyen, Thu Tran_**

Explore States returns a state space of all possible solutions at a given time point, so the number of possible solutions can be quite large. Thus, it can be difficult for the user to locate a specific solution as they would have to manually click through the state space. To mitigate this problem, we added another set of filters to Explore States. Previously, there was only one set of filters that were criteria that were applicable to the whole model, such as “most resource satisfied”. The new filter, Intention Filter, allows the user to select an individual intention from the model and filter solutions based on satisfaction values. This allows users to find possible solutions more quickly if they know the parameters of the solution they want. Intention Filter works in unison with the previously existing whole model filter, which allows for a less laborious search process.

In addition to adding IF-Next filters, we also extended Evaluation Visualization Overlay (EVO) into Explore states. EVO was originally implemented as a feature on the main Modeling and Analysis window of BloomingLeaf and portrays the satisfaction values of the goal model as different colors, which helps users understand and visualize the goal model faster. Finally, we updated the appearance of Explore States to better match the aesthetics of the main window and cleaned up the CSS files associated with Explore States.

<img src="/images/intention-filtering.png"
     alt="Collaborations Poster for Next State Project"
     />

