---
title: 'Frontend Refactor of BloomingLeaf to Backbone.js'
date: 2021-08-13
excerpt: Manar Alnazer, Yesugen Baatartogtokh, Angela Chu, Irene Foster, Catherine Kung 
collection: projects
permalink: /posts/2021-08-13-backbone-refactor
layout: archive
---

**Frontend Refactor of BloomingLeaf to Backbone.js**  
**_2021 SURF Abstract by Manar Alnazer, Yesugen Baatartogtokh, Angela Chu, Irene Foster, and Catherine Kung_**

BloomingLeaf is an analysis and modeling tool that allows users to model goals that evolve over time. These models consist of intentions, actors, and links. By evaluating the changes in intentions over time, users are better able to understand future project evolutions. BloomingLeaf has been developed incrementally over several years as new features were required to explore research questions. As such, the code contained multiple global variables and was highly coupled. For example, if a developer wanted to update one of the elements, they would have to look through the code for all of the places it was mentioned and update it in every spot. Recently, while exploring new model management features, we discovered that the code base could be significantly improved by taking full advantage of Backbone.js.

Backbone.js is a JavaScript library that implements a Model-View-Controller framework. It uses both "Models" to represent data and "Views" to create the user-interface. The Models are passed into their respective Views, and when they are updated they trigger a change event that then reflects that change across every View associated with the Model. This eliminates the need to manually search for and update every aspect of the user interface associated with data when there is a change.

We migrated the BloomingLeaf codebase into Backbone centric Models, using the original class objects as a foundation. Although previously there were Backbone Views for some features, the Backbone data structures were not being used to tie data to Views, essentially rendering them into static HTML chunks. Additionally, we updated the Views and created templates for them, to use the associated Model data and parse it into the appropriate HTML locations. This created reusable modular views for each of the major parts of the BloomingLeaf user interface. 

Turning the codebase into Backbone makes the data structures more compatible, and updates our Views to take in that data in order to make a more dynamic and structured web application.  Although there is more overhead to learning the Backbone terminology and features, once learned it provides a consistent and straightforward way to ensure a singular coding style for the frontend of the codebase. After implementing Backbone.js, all Views and Models are connected directly and many components of the application only have to be updated in one spot. We hope that this will help future students learn the codebase faster.

<img src="/images/backbone-frontend-model-chart.png"
     alt="Object Model for BloomLeaf Front-end."
     />

