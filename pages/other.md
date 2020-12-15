---
layout: layouts/page.njk
title: Other content and considerations
date: 2020-11-24
permalink: /other/index.html
eleventyNavigation:
  key: Other content
  order: 2
---
The following sections outline additional content and functionality identified by NDSU, with notes as to how each element will be incorporated into the larger framework described in the [project overview](/). For the most part, our understanding is that all of this content will fit into one of the three key areas of the overall site. 

### 1. Non-Ag Content (Gravity Switch) 

As noted by NDSU:

> The Non-ag Content part of the project focuses on the auditing, re-organizing, and migration of non-ag (community, family, food, health, horticulture, and money) NDSU Extension content.

This is largely the same content described in the Extension section of the project overview. For the purposes of this project EC assumes all of the content will live in the Extension section of the website, under the appropriate program or department.

**Questions:**

* Gravity Switch is developing a new content architecture for this that will presumably differ from the structure outlined in the project overview -- when will this work be complete? 
* We are assuming it will not introduce new content types or functionality beyond what is described above?
* Need clarity on 4-H -- we assume if it is included it will function the same as the rest of the new site?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLScKG1p-3Ziupjn8VlFMwVDa0vOwy6qk5_wPFh_ZWV1Rdya-6w/viewform?usp=sf_link" target="_blank">Answer Non-ag Content questions 🤔</a>

::: callout
**NDSU responses:**
* Timeline: In 1 -2 weeks.
* Scope: It will not introduce new content types or functionality beyond what is described in the Project Overview document.
* 4-H: That is correct. If 4-H decides to join the project their pages  will function like the rest of the pages within the site.
:::

### 2. Central Services

Central Services are external services provided by NDSU that will be used to pull in content throughout the new website. These include:

* **Directory**
* **News**
* **Newsletters**

**Questions:**

* Aside from newsletters, how will we be accessing this data? 
* Is there a documented API for each, or a feed of some sort?
* What type of data will we get in response? (JSON, XML, ?) 
* Are we able to query the data? (e.g. query news by department, or topic -- query directory by department)
* NDSU notes the directory will need to be expanded to include AES/CAFSNR -- when will this work be completed?
* What documenation is available for accessing these services? 
* Does every department/group etc. have a newsletter? How many are there? 

We need to determine best way to integrate these as needed, in a flexible and thorough manner 

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSfoqtUzwHiDlp-j4JgXDrwHuCdChRIyw56xspRLm_mQOTcIfg/viewform?usp=sf_link" target="_blank">Answer Central services questions  🤔</a>

::: callout
**NDSU responses:**
* **Accessing data:** 
* Directory - Currently the directory application serves “blocks” of HTML that are inserted into a CMS page by a bit of Javascript. With the new CMS project it would probably make sense to provide just the data via an API.
* News - News is a separate Plone instance, my initial thought is that we would use our Apache server to “mount” it somewhere in the URL space of the new site, e.g. /agriculture/news or /agriculture/aghub/news. 
* RSS and Atom feeds are also available for all articles as well as some subsets of articles. (More subsets are possible as needed)
* **API/Data sources:**
* Directory - An API could be added
* News - RSS and Atom feeds, needs to be documented
* Directory - does EC have a preference? We could provide either JSON or XML.
* Documentation still needs to be developed
* **Data queries:** 
* Directory - There is no mechanism providing a general query capability but there are quite a number of pre-defined groups (departments, etc.) that can be requested. A more general query capability could be added if needed.
* News - No, it might be possible to add (e.g. query by the tags used for each article)
* **Schedule for directory expansion:** Not scheduled yet
* **Number of newsletters:** We are working on defining which newsletters we need. All county offices and each REC will have one or two. Along with existing newsletters that would put us around 125.
:::

### 3. Event registrations

As noted by NDSU:

> This service is critical to the Engagement Strategy and will be developed by Electric Citizen within Drupal.

**Questions:**

* Tagged events will show up as links in other areas of the site as needed 
* Currently you use an external service/site for registrations -- can we assume that will continue to be the case? 
* We did not budget for or include in scope a full registration system

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSfovYxL0rhJ8JZML5t626YwTK4wySg87h5dgUvco2KH7I2TnQ/viewform?usp=sf_link" target="_blank">Answer Event registrations questions 🤔</a>

::: callout
**NDSU responses:**
* Scope/budget -- Understood. We would like to discuss options that would work best for a registration system and explore how we can achieve them either through third-party services or an expansion of scope. Only online payment runs through NDSU’s Marketplace payment system. We would like a central registration system for collecting registrations, separate from taking payments in Marketplace. Marketplace is not a convenient platform for taking registrations, so many of our staff are using Qualtrics or Google Forms, then sending registrants to Marketplace if online payments are required. We are required to use Marketplace for online payments. Our hope is to have the ability to build simple registration forms for events within our Drupal system. However, we are not that familiar with Drupal. I have seen simple registration/event systems implemented through Wordpress add-ons, but they may not have all the features we need. We are hoping Electric Citizen can help us think through the Drupal options for registration, if any.
:::


### 4. Research Extension Centers

As noted by NDSU:

> There are 7 Research Extension Centers (REC) across the state. Along with the Main Station and Agronomy Seed farm, each of them will need web content associated with their location, staff, and work.

Example: https://www.ag.ndsu.edu/research/research-extension-centers

These currently live under the hub of Extension, and we assume they will remain so. 

* Possible Group module candidate
* The Group module allows a small group of editors to self control their part (and only their part) of the website

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSc9cKxB8fcVxshhRzdKHOdUxv6g8ORuxcjqi4M_btwNEh_8Ng/viewform?usp=sf_link" target="_blank">Answer REC questions 🤔</a>

::: callout
**NDSU responses:**
* Microsites: The vision is to simplify these sites, reducing the amount of content on the sites by moving it to the relevant topics within the Ag Hub, and focusing on the REC sites on engaging with ag producers and other stakeholders.
* Menus: No. The Ag Hub menu would be the top-level menu on these pages.
* REC content/homepage: We are still working with RECs to define what the priorities for REC pages will be.
* Site managers: The site management varies at each REC. Some sites have multiple content creators, some have only one. Going forward each REC will have one section manager.
* Global News/profile content types: yes
::: 

### 5. NDSU Extension County Offices

As noted by NDSU:

> There are 53 County Extension Offices across the state. Each of them will need web content associated with their location, staff, and work.

As with Research Centers, this content will continue to live under the main Extension website.

**Questions**
* Could you clarify your vision for these “microsites” moving forward
* If these are continuing on in a similar version to what is currently presented, what content should be featured on the homepage of each county office?
* How is each center’s “site” currently managed? Who creates and updates pages? Will that same process be used moving forward?
* We are assuming these will be managed by people at the offices, and need flexibility in terms of how many pages or what content to add. Is this correct?
* What is the “Ask an Expert” widget on these pages, and is it continuing?
* Currently, these are part of Extension services and listed in a sidebar menu? Is that the plan moving forward?
* What is the mini slideshow on the landing page of each? What is its purpose? To show which coursework is available? Do we need to recreate?
* The “latest info” block, is that simply a list of News items tagged with “Extension”? Anything specific to each Extension office?
* It appears that each office has a blog. How are these currently managed?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSe_U_STM14R6Pe9Imcwkh_NfKnb_C9fW5E3BgpsTR_WT3Hr8Q/viewform?usp=sf_link" target="_blank">Answer Extension Office questions 🤔</a>

::: callout
**NDSU responses:**
* Microsites: The vision is to simplify these sites, reducing the amount of content on the sites and focusing on the content strategy for County Extension sites. The content strategy for County Extension Offices is Building trust in NDSU Extension, Building relationships with the people of their county, Being a local resource, and Showing impact/value. This means that educational content that may currently reside on county Extension sites will be migrated to the appropriate topic. The Ag Comm team will work with county Extension staff to migrate content that fits the content strategy into new pages organized under the NDSU Extension subsection of the NDSU Agriculture site.
* Featured content: The County Extension pages will be changed significantly. We have not yet finalized our priorities for County Extension pages, but based on our engagement strategy and the content strategy mentioned in the previous answer, events, directory information and newsletter signup will likely be high priorities.
* Site managers: Currently 1-3 people in each county office manage their sites with primary responsibility usually falling to the county administrative assistant. We anticipate that process will change with the addition of "editors" to review and publish content.
* Site managers 2: Yes, although we will be introducing an "editor" level to review and publish additions.
* Ask an Expert: Ask an Expert is a national tool managed by eXtension.org. It is currently undergoing an overhaul of its own. We anticipate continuing to use the tool, although it may become a link rather than a widget
* Sidebar menu placement: I'm not sure what you are referring to. Can you clarify?
* Slideshows: I think you are referring to an item type that some county offices have on the landing page. The purpose varies, but usually they are not very helpful. We do not need to recreate it.
* Latest info block: That is an RSS feed from www.ag.ndsu.edu/news with generic Ag & Extension news, which will not be a part of the new County extension pages. Each extension microsite can create "news" items specific to their site, but we don't anticipate needing that feature in the new site.
* Blogs: They are managed by the County Extension Offices. Our plan is to remove the blogs from county Extension site because they too often duplicate educational content that will reside within the Ag Hub or Extension topic areas. we will be encouraging County Extension offices to use social media and their newsletter for sharing that kind of timely information.
:::

### 6. Multidisciplinary Issues & Research Projects

> Some topics and issues do not fit neatly within a particular topic or even a section of the site. In some cases (e.g. Farm/Ranch Succession Planning), the intended audience will dictate the section of the site the content belongs in (e.g. Farm/Ranch Succession Planning belongs on the Ag Hub). In cases of new issues or projects in which the content is not clearly organized into a topic or section, it can be created as Multidisciplinary Issues within Extension or Ag Hub, or Research Projects with AES.

**Questions**

* Are you intending a new content type for this, or simply normal "pages" that will get added where they best fit?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSfi9MCNFUCum2tutnlrHn1L0N6nHSW45ehrGccPckXN1FZ1_g/viewform?usp=sf_link" target="_blank">Answer Multidisciplinary Issues questions 🤔</a>

::: callout
**NDSU responses:**
* New content type? - Normal pages added where they fit best.
:::