---
title: "Operation Specification: Extending GitLab to Incorporate Specifications"
date: 2024-07-19
excerpt: Kika Kovaleski, Aline Marra, Sydney Weisberg
permalink: /posts/2024-07-19-gitlab-start
layout: archive
---

**Operation Specification: Extending GitLab to Incorporate Specifications**  
**_Kika Kovaleski, Aline Marra, and Sydney Weisberg_**

Requirements engineering (RE) is the process of defining, documenting, and validating users’ goals. Requirements are crucial as they guide developers towards creating products based around user needs, but they often fall through the cracks as developers fail to consider these needs throughout their development activities. GitRE will help center user requirements in software development projects by integrating requirements engineering into the development process.

In traditional software development, developers use version control features such as “issues” and “milestones” to track their progress towards project goals. These work well for short-term achievements but fail to account for the larger-scale goals of a project  – especially goals related to user needs. GitLab, a popular version control system built on the Git versioning system, uses these features. GitLab is an open-source platform that allows users to develop on its codebase via the GitLab Development Kit (GDK), a tool that allows users to run a local instance of GitLab. We used GDK, working in GitLab’s Ruby on Rails codebase, to add requirements specifications as first-class entities in every repository.

Specifically, we created an interface that integrates requirements engineering into the GitLab development process. We updated GitLab to include tabs where developers can create, delete, edit, and view specifications (i.e., requirements). These specifications can be viewed on account, project, issue, or merge request pages, and developers can search for specifications by name on account and project pages. They can be created individually, or developers can import specifications in bulk with a CSV file. Specifications can be linked to issues and merge requests so users can keep track of their progress towards fulfilling each specification. When creating or editing merge requests and issues, users can manually add these links via a dropdown.

Specifications are distinct from issues and milestones in that they cannot be “closed” as development progresses; they are standing goals that serve as a reminder of what the project should be able to do for users.

Our ongoing work involves adding options to unlink specifications from issues and merge requests, allowing users to select multiple specifications on dropdown tabs, and replacing the specification “delete” option with an “archive” option. Incorporating these features will help developers maintain a focus on users’ needs by making development with specifications more flexible and intuitive.

<!--
<img src="/images/pc-view.png"
     alt="Screenshot of Actor view with presence conditions."
     />
-->
