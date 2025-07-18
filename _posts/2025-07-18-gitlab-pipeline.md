---
title: "Validation Station on the Pipeline of Specification Integration"
date: 2025-07-18
excerpt: Kika Kovaleski, Vivian Myers, Jessica Klurfeld, Karenna Kung
permalink: /posts/2025-07-18-gitlab-pipeline
layout: archive
---

**Validation Station on the Pipeline of Specification Integration**  
**_Kika Kovaleski, Vivian Myers, Jessica Klurfeld, Karenna Kung_**

During software development, engineers often fail to account for the original goals and stakeholder requirements of a project. Requirements engineering is the process of defining, documenting, and validating these goals. Using the GitLab Development Kit and GitLab’s Ruby on Rails codebase, we are integrating requirements as “specifications” into GitLab to help developers track overarching goals and connect them to issues and merge requests (issuables). 

This summer, we expanded on previous work by integrating automatic code validation and implementing new features. We focused on testing our codebase using GitLab’s CI/CD pipeline to ensure it meets their quality standards for future integration. We installed and configured GitLab Runner, an application which works with GitLab CI/CD to run pipeline jobs, on a remote server. Using Docker Engine, an open source containerization technology, we were able to automatically execute these jobs in isolated, reproducible environments. Running and passing these tests allowed us to resolve critical errors and merge branches with different features, including edit, delete, and counter badges, to enable further development. This process also highlighted inconsistencies in our database, which we worked to fix by reconfiguring our initial Rails migrations and regularly testing changes using the pipeline.
	
Additionally, we added several new features to our user interface. We implemented a “content” feature, allowing specifications to have a more detailed description. We also implemented a dropdown for specifications on the “merge request” and “issues” pages to permit users to link these objects. Specifications selected in the dropdown are displayed in the sidebar. When clicked, each selected specification routes to its individual page. We implemented resource events to track who linked or unlinked specifications from issuables and when they did so. We also drafted mockups of the next feature we plan on developing: the ability to approve or deny suggested specification links.

Our ongoing work involves parallelizing our pipeline on a high-performance computing cluster, to allow for more efficient progress. GitLab’s CI/CD pipeline is computationally resource-intensive, making it difficult to run efficiently on our small servers. Future feature development includes an “archive” feature, permitting users to approve or deny LLM-suggested links between issuables and specifications, and deployment.


<!--
<img src="/images/pc-view.png"
     alt="Screenshot of Actor view with presence conditions."
     />
-->
