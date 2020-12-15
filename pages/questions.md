---
title: Open questions (high level)
date: 2020-11-20
permalink: /questions/index.html
eleventyNavigation:
  key: Open questions
  order: 3
---
These are a variety of high-level topics for open discussion that will inform some significant architectural decisions. There is some duplication between these question areas and some of the content type questions. Answer both as appropriate. 

## Navigation questions

Navigation on a large Drupal site with many editors and several distinct sections can get quite complex, and we hope to find a simple efficient way to handle menus. 

* In an ideal world, how will top level and sub navigation be handled? 
 * e.g. If I go into the CAFSNR or Extention areas of the site, should there be a second-level of horizontal navigation at the top? Or in a sidebar? A megamenu?
* Presumably the top-level will also include some links to global "news", "events", "contact" etc.  
* Within a subsection of the main site, should this global nav always appear? 
* Will there be one person/office responsible managing the main navigation? 
* Who else needs the ability to add their OWN pages/items to the navigation? (e.g. Research centers, extension groups)

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSek60Fsqi2DSxYL_giop0AcX8nGC2oAl_52Ow1dA_yi1t4YDA/viewform?usp=sf_link" target="_blank">Answer Navigation questions 🤔</a>

::: callout
**NDSU responses**
* **Top-level nav:**
* There will be a second level of horizontal navigation at the top.
* NDSU Ag Level - Top level is NDSU navigation (About, Academics, Admission, Athletics). Second level is NDSU Ag navigation (Academics, Ag Hub, Extension)
* CAFSNR, Ag Hub, Extension level - Top level is NDSU Ag navigation. Second level is relevant navigation for that level.
* Levels below subsection (e.g. NDSU Extension - Food) Top level is relevant CAFSNR, Ag Hub, or Extension navigation (e.g. Extension nav.). Second level is navigation for that level (e.g Food nav.).
* Other levels below - same as above with additional sub-navigation displayed on the left.
* **Secondary nav:** -  Yes, there will be “navigation” items displayed outside the navigation hierarchy.
* **Subsection navigation:** No, not always. It would depend on the subsection.
* **Menu management** -- Yes, NDSU Ag Comm web team manage the navigation for NDSU Agriculture and the Academics, Ag Hub, and Extension subsections. County Extension section managers, REC section managers, academic department section managers, topic area section managers need the ability to add pages and add them to the second and third level navigation.
:::

## Content sharing throughout site

> Educational content produced at the county level should be integrated into the appropriate topic area on the Ag Hub or Extension sites.

This is one of several examples where NDSU mentions content flowing into the Ag Hub, or from one area of the site to another. (e.g. Publications)

* In Drupal, content has a single home or "source of truth"
* We can pull in content via relationships/tags, but it will always "live" in a single place
* For example, a Publication will always be a node that lives in the Publications area of the site
* But based on tags, we could then show that publication on the relevant page of the site

**Questions**
* What your are your goals and expectations about sharing content throughout the site?
* We are assuming a heavy use of taxonomy and "related content" throughtout (e.g. show Publications that match this tag) and a mix of curated relationships (e.g. editors adding "related links/pages" as needed throughout the site. Does this sound right?
* We have identified numerous obvious taxonomies for specific content types, but wonder if you have thought of any additional taxonomies that might be used as a global organizing mechanism? (e.g. one or more taxonomies such as "topics" that are shared among multipe content types.) Have you given any thought to this?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSdlJgP-C06W3n_du0FI6gbwZJeAfMA-LJLzoEaSU8ivt6UVTw/viewform?usp=sf_link" target="_blank">Answer Content sharing questions 🤔</a>

::: callout 
**NDSU responses** 
* Overall vision: no response
* Taxonomy and related content: Yes, that sounds right. We have a list of tags we use for news releases and more recently publications. That list could be used and built upon for this project.
* Global Taxonomy planning: Other than the list of tags in the previous question, we have not.
:::

## Events

We will likely have more questions surrounding events as we go but here are some to begin planning.

* We need more clarity on event "series", events with "multiple locations"
* As noted we did not plan for or budget a full-scale event registration system -- can we assume that we can rely on external links to the NDSU payment system in place now?
* We also need more clarity on how "programs" (within Extension) will relate to events? Do "programs" need to show up in the main event calendar?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSepFTSyadDrvInL2J8mjj6DFypsInpGCWZQKHyeiNhbj5Mngg/viewform?usp=sf_link" target="_blank">Answer Events questions 🤔</a>

::: callout
**NDSU responses:**
* Event series: Here’s an example: a series of webinars that take place at the same time over a series of 10 weeks (e.g. Wednesdays at 2 p.m.). Registrants can choose which of the webinars they want to attend, one, some, or all. Each of the webinars is represented on the correct day and time on the events calendar, but there is also a way to connect these 10 webinars into a series, so someone could view the complete schedule.We are trying to make a distinction between the above “series” and a program which may include webinars, workshops or other learning events, but they are all interdependent. The intention is not to pick and choose which interest you, but to engage in all of them over time.\
* Event registrations: This was covered in the question about event registrations in the “Home” section of this document. We are not using a common, central service for registrations, but need to make that part of our overall plan.
* Programs/events relationship: Programs will not show up in the main event calendar. The individual sessions in a program only need to be communicated to those registered for the complete program, so programs should not relate to events.
* Event categories/filters: Our current calendar includes the ability to sort by county and region, so people can view events near them or we can display the relevant events on a county page. We would need to do the same for academic department events and REC events (those are not currently part of our calendar). We will also need to define events by the same list of tags we use to define other content, so relevant events can be displayed on topic pages. Finally, I think we would want to add delivery method (in-person, online, both).
* Older events: We would like events to stop displaying/be unpublished after the end date, and be deleted after 6 months. As I’m typing this, I’m thinking we may need to change 6-months to 12, so users have the opportunity to duplicate and update an annual event. Maybe?
:::


## News

We are unclear about the specific content types needed for "news releases" and "columns" and/or "new alerts" content type, or whether all of the news will be coming directly from Central Services (Plone).

Examples from current site(s): 
* https://www.ag.ndsu.edu/news/newsreleases/2020/aug-3-2020/inventory-forage-supplies-early/view
* https://www.ag.ndsu.edu/news/columns/spotlight-on-economics/spotlight-on-economics-selfish-behavior-has-economic-costs
* https://www.ag.ndsu.edu/academics/student-profile-billie-lentz

**Questions**

* Is all of the news coming directly from Plone? (Columns, new releases) Will you be creating additional news NOT coming from Plone?
* Do we need a content type for each type of news, or just one type?
* What about content moderation/approval process? Which parts of the site does it apply to? All areas or just some?
* When does a news item get “moved” to the Archive? After a certain number of days? Should they still show up in site search? Why is there a need for an official "archive"?
* What types of taxonomies (categories) do you anticipate being able to use for tagging/sorting and display different lists of new?
* 

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLScwyp1cxdB565XEpI5zBn-oTNYdCIpS0akCEsWjYOH5dzlsog/viewform?usp=sf_link" target="_blank">Answer News questions 🤔</a>

::: callout
**NDSU responses:**
* Plone news -- Global news (releases and columns) would come from Plone. Subsection/microsite news would become “newsletter articles” published within a subsection (so they can be linked to from social media), but not included in search, which could be packaged into a newsletter.
* Content types -- If we don’t consider displaying global news as a content type, then just one content type, “newsletter article.”
* Moderation/approval -- It applies to all areas. Section managers will moderate/approve all content
* Archives -- Global news will be in Plone and have separate expiration/archive rules. Newsletter articles should never show in search. Since they will not show in search, there is no need for a news archive. Newsletter articles should have an expiration date of 12 months from creation, but can be set manually and causes the item to be unpublished.
* Taxonomies -- Those taxonomies will come from Plone for global news which will use the list of tags/keywords mentioned in previous answers. Newsletter articles will not need tagging sorting, since they won’t be displayed, only used to link to from social media and included in email newsletters.
:::

## Publications

Our assumption is that Publications will remain its own, stand-alone area of the website with a single content type, but Publications can also be displayed elsewhere within the site (e.g. if a college or program has a "Publication" a description and link can be displayed on their pages via a tag View). Publications may also be displayed on the Ag Hub (we think?), again via a tagged search or View. 

**Questions**

* In your major changes doc you say: "Publications become the primary content type for Ag and Extension information" Can you expand on this?
* Where would these be found on the new site? Currently they are only in Extension? Show as list on a single page with search as they are now? Given the above question, how else will these be used/integrated in the site?
* “Expire after 5 years” -- is this the same for all Publication content? Does this mean to delete the node entirely or just unpublish?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLScnIhljl8_cvcfeqJrm5ZdBXzlZu1Ja2jTr4QrdTNjlW7BRXA/viewform?usp=sf_link" target="_blank">Answer Publications questions 🤔</a>

::: callout 
**NDSU responses:**
* Primary content type -- Publications, at their best, are the gold standard of Ag and Extension information. For all but new and emerging topic areas, publications should be the foundation of the content because they are peer-reviewed and intended to have a relatively long shelf life.
* Content home -- We are now planning to have a publication type that can be used throughout the Ag Hub and NDSU Extension subsections, so publications reside within the topic area they relate to. Some publications cross multiple topic areas, so there will be a need to display them in one or more areas based on tags/keywords.
* Expiration -- This is the same for all Publications. The node should be unpublished. Authors will have a chance to review, revise and and re-publish the publication
:::



## Group module, Workbench Access, Content moderationx

We need to develop more detailed requirements surrounding each of these areas to determine appropriate user roles, workflows, and methods. These decisions will have a significant effect on overall site archicture. 

* **Group** -- this module may be a candidate for letting research centers and county sites manage their own content and menus 
* **Workbench Access** -- this is a third-party module that helps us control who can edit what content and provides a fairly reasonable way to manage access across a wide range of content. We are considering this as the main candidate to manage content within CAFSNR, Extension, and Ag Hub 
* **Menu access** -- one big issue in Drupal is Menu permissions; if you give a user permissions to "manage menus", they typically then have access to manage ALL Menus. This usually undesirable so we will need more details surrounding expectations for Menu management
* **Number of Menus** -- we'll need to determine whether we create separate menu structures for each key area of the site, or rely largely on one Primary Menu

**Questions**
* How many user and  distinct groups of users will there be managing the site? (e.g. central admin, REC editors, county site editors, extension editors, etc.)? 
* Which users will be able to manage main navigation menus, and add new pages? Which users will be restricted to only their own areas/pages?
* Can we limit adding of new pages and menus to certain areas (e.g. research/county centers), and have a central admin team manage the main navigation? (Other users could edit and maintain their assigned pages, just not add new ones or alter the main menu.)
* What about content moderation/approval process? Which parts of the site does it apply to? All areas or just some?
* How about content scheduling? Which areas/types of content need scheduling, if any?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSdZE3bzAOGK8-gykPvoPLQVJIooEyN3qrBl8_IkuWbUP13Kug/viewform?usp=sf_link" target="_blank">Answer workflow questions 🤔</a>

::: callout 
**NDSU responses**
* Distinct users and groups -- Administrators (NDSU Ag Comm Web Team) (6-8 users) Section managers (80-100)
* Menu managers -- Administrators manage the navigation for NDSU Agriculture and the Academics, Ag Hub, and Extension subsections. Section managers need the ability to add pages and add them to the second and third level navigation. Section managers will be restricted to their own areas.
* Limitations on menu management -- yes
* Moderation/approval process -- applies to all content
* Scheduling -- applies to all content
:::

## Content syndication

As noted in the overview, content from Central Services will be pulled into this website and we noted a number of concerns and questions. We will call them out here again as they are of special concern:

* How will we be accessing this data? 
* Is there a documented API for each, or a feed of some sort?
* What type of data will we get in response? (JSON, XML, ?) 
* Are we able to query the data? (e.g. query news by department, or topic -- query directory by department)
* NDSU notes the directory will need to be expanded to include AES/CAFSNR -- when will this work be completed?
* What documenation is available for accessing these services? 
* Does every department/group etc. have a newsletter? How many are there? 
* We need to determine best way to integrate these in a flexible way throughout as needed

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSeIxUIoHBoV7iO84mIyoc3sMdtCuGuct_A9gZ2sgRQp_4VoFw/viewform?usp=sf_link" target="_blank">Answer Content syndication questions 🤔</a>

::: callout
**NDSU responses**
* no response -- see related questions in Other content
:::

## Tools

In previous discovery we identified two main JS tools (e.g. Wheat nitrogen calculator), and list of Excel spreadsheets used as tools. Our current plan is to re-theme and hopefully use the exact JS in the current tools, and link to each spreadsheet as appropriate. 
 
 See: [List of tools](https://docs.google.com/spreadsheets/d/13ONJKXYxq10thkYPBgB92lCRoIgG1FVTbxRyoc6xThk/edit#gid=996020785)

**Questions**
* Where is the new home for the two primary JS tools we have identified? 
* For all of the Excel sheets, we assume you will just link to them as needed throughout the site?
* Are there any other comments or expectations surrounding tools?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSdFcPaHGKOCyf6MQwipdKwzr2BOj5AZaZV_9rm30nlgADZNSA/viewform?usp=sf_link" target="_blank">Answer Tools questions 🤔</a> 

::: callout
**NDSU responses**
* Location: These tools can be moved to NDSU Agriculture web space.
* Location 2: These tools can be moved to NDSU Agriculture web space.
:::

## Newsletters

To design an effective way to organize newsletter subscribe buttons throughout the site, we need a bit more information. 

* Does every department/group etc. have a newsletter? How many are there? 
* If we build a widget that allows you to drop a "subscribe to newsletter" button, with some descriptive text onto any area of the site is this sufficient? Are the newsletters coded such that the content editor would know what code to use for their particular newsletter?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSeYlo2fNS5qyZ4WfGyobo6xEQvzjWUIDYyHMBHgeeslKYghhg/viewform?usp=sf_link" target="_blank">Answer  Newsletter questions 🤔</a>

::: callout 
**NDSU responses** 
* Numbers -- We are working on defining which newsletters we need. All county offices and each REC will have one or two. Along with existing newsletters that would put us around 125.
* Widget -- We’d like those subscriptions to be contextual, so newsletters related to that area, department, or topic are displayed .
* Coding -- 
Section managers will post newsletter articles within areas meant for their newsletter, e.g. Cass County posts newsletter articles in a folder for “Cass County Newsletter.” Newsletter articles will not be displayed on pages or in search.
:::

## Calls to Action

We have not discussed how, or if, to handle calls to action. Many of our higher ed clients use a standard set of "Schedule a visit!" or "Apply now" or "Contact us" calls to action that can be placed in key places on the site. 

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSfsBsbcUjZ9FCerfYRr-EZFBPSq2MNgWguWLEFJg2VY3bAhYw/viewform?usp=sf_link" target="_blank">Answer CTA questions 🤔</a>

::: callout
**NDSU responses:**
* CTAs -- There are no common calls to action persistent across NDSU Agriculture. There are some that could be displayed across subsections, e.g. CAFSNR (Apply, Visit), Ag Hub (Subscribe, Contact Us), Extension (Contact Us).
:::

## Search

We have not discussed search; unless NDSU provisions a Solr server we will be limited to core Drupal search and Search API. This is powerful, but will limit the ability to do certain things like searchable PDFs.

* How will search be handled? 
* Global search plus Ag Hub search? 
* Any other key search requirements? 

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSesFsA0odCb8gteIaoatXbjaInn_J2Yhl7HeSHV7-Z-9znLrQ/viewform?usp=sf_link" target="_blank">Answer Search questions 🤔</a>

::: callout
**NDSU responses:**
* General -- We currently use Google Custom Search. We have found we get better results than we did when we had Solr search. We need faceted search options especially within Ag Hub and Extension. We are open to discussing which available options would work best for our needs. Global search and Ag hub specific search are needed. We need specific search or facets for recipes. We also need the option for users to search only a section of the site.
:::

## Design work

We will be duplicating the existing NDSU theme, and are presuming a single theme will be used across the site and all microsites. 

**Questions:**
* Is our assumption of a single theme across all pages correct?
* Will you be providing any additional wireframes or guideance for page layouts and content placement?
* Do you need a style guide? Is there one?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLScwgJTlkRwVeAN_r0VLtQkzZcuvxRqI4OjJ2DGLO3NlyBMMKQ/viewform?usp=sf_link" target="_blank">Answer Design work questions 🤔</a>

::: callout 
**NDSU responses:**
* Yes, we are thinking of one theme across the site.
* Yes our graphic designer is working on page layouts starting with mobile first.
* Yes. We need a style guide. There is not one now.
:::
