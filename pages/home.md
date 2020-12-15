---
title: Project overview 
date: 2020-11-25
permalink: /
eleventyNavigation:
  key: Home
  order: 0
---
The following sections outline our understanding of current project scope, informed by all of the documentation and information generated to date. These documents include the original RFP, questions and responses, Electric Citizen's original proposal, meeting notes, and all files provided by NDSU.

There are still numerous unknowns and questions to be answered and this project overview can be used to both inform those answers and to develop a final technical architecture. The purpose of this living website is to clarify key technical requirements, and to ultimately create an official build plan.

All the pages in this site are interspersed with "answer" buttons that will open up a Google Form allowing you to provide answers to our specific questions. Please be as expansive in your responses as possible; we can set up a Zoom to discuss finer points as needed. _Note: you should be able to go back and edit or add to your responses as needed_.

## Primary goals and requirements

Electric Citizen will develop a single Drupal 9 website that will bring the content from numerous areas throughout *NDSU Ag/Ext* under a single umbrella. The homepage of the website will consist of a yet-to-be-determined set of content, and from the top level navigation of this website, a user will be able to navigate to one of these main areas and its subpages: 

![Diagram](/static/img/ndsu.png)

* All sections of the main site will share a common theme
* All sections will share a common set of content types and functionality (with limitations and restrictions as needed) 

### 1. NDSU Ag and Ext homepage

We have not discussed the homepage in any detail so we should start this discussion soon.  

**Questions:**

* Is the above diagram accurate, as a high-level overview of how content will be organized on the new site?
* Have you given any thought as to how the homepage will be organized?
* What content or types of content should it contain? What calls to action? 
* Will the homepage need any special features or controls different than a standard landing page?
* Is VP of Agricultural Affairs simply a link out to another part of NDSU site?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/1N26zqAp2S3jSr1kweZHWXhEeTUDFh0PeP0M6GUjO2Fo/edit?usp=sharing" target="_blank">Answer NDSU Ag homepage questions 🤔</a>  

☝️ This will open a response form in a new tab. You can edit/change your responses if needed.

::: callout 
**NDSU responses:** 
* Yes, the diagram is accurate.
* Some. We anticipate it will be primarily focused on directing people to CAFSNR, Ag Hub, and NDSU Extension.
* As stated above, it should be primarily a landing page to direct people to main content areas of the site. The main calls to actions will be to navigate to one of those areas and to subscribe to the “For the Land and Its People” newsletter.
* The homepage will not need special features or layouts different from a landing page
* The VP page should reside within the NDSU Agriculture top level. Selected content from www.ndsu.edu/vpag could move under an “About” section of www.ndsu.edu/agriculture.
:::


### 2. College of Agriculture, Food Systems, and Natural Resources (CAFSNR)

All of the content for CAFSNR (including general info, all academic programs/units, schools, colleges, etc) will be moved into the new site. This content is quite broad and deep:

https://www.ag.ndsu.edu/academics

All of the departments and schools are currently on two disparate systems, with different navigation and content. 

* https://www.ndsu.edu/agecon/ (e.g. Typo 3)
* https://www.ag.ndsu.edu/plantpath/ (e.g. Ag CMS)

Moving forward, all of these sites will be moved under the CAFSNR umbrella of the new Ag/Ext site, with consistent navigation and content types for all units/schools (About, Future Students, Current Students, Faculty & Staff, Alumni, Research, News/newsletters, Alerts).

All content and design decisions in this section should be geared toward student recruitment.

#### Questions:

* Does each school/dept have their own content team? 
* Plus a main content team for CAFSNR?
* You mention consistent menus for each school -- does this mean no custom pages/menu items for each school? Or should they be able to add additional pages as needed?
* How should we handle long names (e.g. College of Agriculture, Food Systems, and Natural Resources) in the top-level menu?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSctQWd81uo58r3nXdCm9zk2USnY5Uw0__v587qQlJNt2pUS2w/viewform?usp=sf_link" target="_blank">Answer CAFSNR questions 🤔</a> 

::: callout
**NDSU responses**
* Content teams: Yes, although some departments have more developed teams than others. NDSU Ag Communication staff will need to work closely with departments throughout the migration process.
* *Consistent menus: Yes, that team includes the director of college advancement and Ag Communication staff.*
* *Menu control: We are hoping to have consistent core navigation on school/department pages, but schools/departments will be able to add pages/menu items*
* Long name: I think, in menus, College of Agriculture, Food Systems, and Natural Resources can be shortened to “Academics,” but we need to discuss with our web team and CAFSNR content team.
:::

### 3. Ag Hub

As noted by NDSU: 

> The goal of the Ag Hub is to provide a one-stop source for information about various Ag topics (e.g. wheat production, federal ag programs, variety trials, farm/ranch stress) rather than content stored based on organizational structure (departmental, REC).

> The Ag Hub is a new top-level section of the website that will be used to organize content that is currently spread across numerous different websites including Extension, AES, and CAFSNR. Paulsen is currently developing the list of content and an architecture for this content, and have produced an initial wireframe. 

* [Content architecture](https://docs.google.com/spreadsheets/d/13ONJKXYxq10thkYPBgB92lCRoIgG1FVTbxRyoc6xThk/edit?usp=sharing)
* [Wireframe](https://www.figma.com/proto/HmJmEmT8DQyGhk6Do370rn/NDSU-Wireframe?node-id=9%3A51&viewport=176%2C-201%2C1&scaling=min-zoom)

**Questions:** 

::: callout 
*This is one of the most unclear portions of the project for our team.* Our understanding is that it will contain a mixture of new content, along with content pulled from both Extension and perhaps CAFSNR. Defining the Ag Hub needs to happen soon and will inform large parts of the architecture.
:::

* From our conversations and the wireframe presented, it appears this was originally intended to be a stand-alone site, but is now being folded into this umbrella site. Is this correct? 
* From a technical level, this appears to mostly be a topic-based directory that includes search in order to present a variety of content (and content types) in a one-stop section of the website. Is that correct?
* Given that this is no longer a stand-alone site (assuming our assumption is correct), **we believe there may be a better approach to the Ag Hub that is structured more like a searchable directory of resources (perhaps with faceted search), instead of a "minisite" within a site**. Are you open to discussing this approach?
* In the architecture linked above, there is a lot of content listed for Ag Hub that is actually part of Extension, or another area of this site. 
* We need to best determine how Ag Hub will function to pull in that content, vs creating it two places.
* In your site outline, you have both County Centers and Research Centers under Ag Hub, but we are envisioning them under Extension, with CONTENT from those centers pulled into the Ag Hub as appropriate.
* Your sitemap also indicates other content, such as all of the topics shown in the wireframe (REC/AES). Is your current thinking around Ag Hub much simpler than we are envisioning?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLScR2wn1BZPV3PXiqwxceIJJDfAenxCDQuCbfV93gyWr6LzBhA/viewform?usp=sf_link" target="_blank">Answer Ag Hub questions 🤔</a> 

::: callout
**NDSU responses**
* Wireframe/stand-alone site: The wireframe was prepared by Paulsen and is focused only on the architecture within the Ag Hub. So it wasn’t that the Ag Hub was designed as stand-alone, it is more that we were still working through the top-level architecture and Paulsen addressed only the part of the site that was in their scope in the wireframe.
* AgHub: No. The content referenced in the Ag Hub will reside within the Ag Hub. It will be a main content hub, not a directory linking out to content that resides in other parts of the site. Faceted search will be a major feature of the Ag Hub, allowing users to search within types of content. Content currently hosted on Extension and Ag research sites will be re-organized within and migrated to the Ag Hub. The point of the site is to provide a home for all actionable information that can help ag producers improve their operations.
* Searchable directory approach: We are willing to discuss it along with Paulsen. Filtered, faceted search is part of the plan for the Ag Hub.
* County centers/research centers: County offices will be under Extension, but RECs will be under the Ag Hub, because they exclusively serve Ag audiences.. Ag content from those sites will be re-organized and migrated to the appropriate topic under the Ag Hub. This will reduce the amount of content that is a part of the County and REC sites, allowing both entities to focus on encouraging deeper engagement with the people of their county or region.
* General aghub: The Ag Hub will bring together content that is currently located under Extension, one of the Research Extension Centers (which fall under the Ag Experiment Station organizationally), and CAFSNR. This content will not be pulled into the Ag Hub. It will be re-organized and migrated into the Ag Hub. This will provide a central site for crop and livestock producers to find content that can help them improve their operations. It is simpler in terms of the content will reside within the Ag Hub, rather than be pulled in from various sources.
:::

## 4. NDSU Extension

All of the content from NDSU Extension will be moved over to the new site, and made available via top level navigation. The content for extension is also quite broad and deep:

https://www.ag.ndsu.edu/extension

There are subsites for each primary area of extension (e.g. Crops, Farm Economics) that contain:

* **Topics** -- these seem to be variety of pages and sub-pages within each area that contain everything from publications and PDFs to subpages and external links. They appear to be organically organized and created (and many are out of date).
* **Programs** -- multiple programs per landing page, each with its own subpages. Links to external registration. 
* **Publications** -- a list of linked publications that are pulled from the global publication content type. Clicking a publication takes you directly to the publication section of the site.
* **Connect** -- a page with bio info, headshots, and basic contact info for each area.


Each topic currently has a slider with large images linking out to various places, including YouTube, links to pubs, etc. There are also links to “apps”, quick links, resources, latest tagged news.


**Questions:**

* NDSU indicates that this content is being re-organized with a new architecture. When will this work be complete?
* Are the "topics" pages all self-managed by each group? They are set up differently, and many are out of date.
Is there a better way to handle "topics"? 
* For program registrations, these appear to be handled by an external link to an NDSU payment system -- can we assume this to be case moving forward also?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSePCUUinA-TxTU_6w7K0pINmIOvFxN9p7udggKaPb9i3XGwEQ/viewform?usp=sf_link" target="_blank">Answer Extension questions 🤔</a> 

::: callout
**NDSU responses:** 
* Architecture timeline: Gravity Switch is nearing completion of the new architecture. We need to confirm with their team, but it should be done in the next week or two.
* Topics pages: The content of “topics” pages currently on the NDSU Extension homepage is managed by the content team for each area, but the updates need to be made by Ag Communication staff. The “new” topic pages will not be so reliant on timely information that needs to be manually updated, like the slideshows on the current pages. We have been working on assembling content teams for the topics (they’ve been communicating with Gravity Switch and Paulsen to inform their work) who will work with editors to organize, update, add and delete content on their pages.
* Registrations: Only online payment runs through NDSU’s Marketplace payment system. We would like a central registration system for collecting registrations, separate from taking payments in Marketplace. Marketplace is not a convenient platform for taking registrations, so many of our staff are using Qualtrics or Google Forms, then sending registrants to Marketplace if online payments are required. We are required to use Marketplace for online payments. Our hope is to have the ability to build simple registration forms for events within our Drupal system. However, we are not that familiar with Drupal. I have seen simple registration/event systems implemented through Wordpress add-ons, but they may not have all the features we need. We are hoping Electric Citizen can help us think through the Drupal options for registration, if any.\
* Editors/content teams: Each area within Extension has a content team. We are hoping to give at least some of the members of that team the ability to manage menus and add new pages within their area, however we would like to have a permission level for managers who would be able to publish those changes. So a permission level for those who can add pages and manage the menu in an area of the site and a higher permission level for those who will review those additions before publishing them.
:::

## Assumptions and Agreements

* EC will build a single site Drupal architecture, including all of the content types, views, taxonomies, and all other related Drupal configuration in order to build out the site as described above and elsewhere on this project site
* NDSU and/or its partners will be responsible for all content migration into this new platform

