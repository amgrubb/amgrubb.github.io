---
title: 'Enabling Continuous Integration of Forked MMINT Repository'
date: 2020-12-12
excerpt: Ella Chang and Sophie Crane
collection: projects
permalink: /posts/2020-12-12-ci-for-mmint
layout: archive
---

**Enabling Continuous Integration of Forked MMINT Repository**  
**_2020 Fall Special Studies Project by Ella Chang and Sophie Crane_**

Continuous Integration (CI) is used by programmers to decrease the number of bugs that arise when multiple people are working on the same code. CI involves frequently sending code to a shared repository where any changes are combined and tested. This helps the coders to find any new bugs and to avoid writing over each other’s code. The coders will pull the new code frequently to make sure they are working on the newest version.
	
We worked on adding CI to INTeractive Model Management, also known as MMINT, which is developed by programmers at the University of Toronto. We forked the code and worked on the .travis.yml file. When this is committed to GitHub it will notify Travis and then build a virtual machine to test that the code runs. For our project we also worked on learning how to build metamodels for Tropos. <!-- and uploaded what we found to grubb-lab-private.-->

See our [GitHub repository](https://github.com/amgrubb/MMINT) for more.

<img src="/images/sscrane-ci-mmint.png"
    alt="Travis continuous integration showing unit tests passes"/>