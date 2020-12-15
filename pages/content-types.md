---
layout: layouts/page.njk
title: Content types 
date: 2020-11-24
permalink: /content-types/index.html
eleventyNavigation:
  key: Content types
  order: 4
---
NDSU Ag & Ext has compiled a list of known content types, along with desired functionality, and outstanding questions. This list does not appear to be exhaustive based on the review of other components of this project (such as the Ag Hub, county extension offices, etc.).  Further discovery is needed to determine how these types interact across the entire Ag & Ext site.

**We have started an initial build plan draft below that will be expanded and revised as we continue to gather more information. See draft plan here:**

* See [Build plan draft](https://docs.google.com/document/d/1ubikpzz9qfGd5bDxCGCpTcKc-JsCyMPvYySkUo4nIKQ/edit?usp=sharing) -- if you have initial feedback on anything in this plan please add comments directly to the draft document.

## Pages 

Basic pages are an essential content type in Drupal and they control all basic informational pages on a site. Examples from NDSU Ag’s current site include: https://www.ag.ndsu.edu/research/history and https://www.ag.ndsu.edu/pesticide/fumigation-resources-1.

* Landing pages
* Basic pages
* Destination pages* 

Typically we build a basic page content type for all standard content, and then a landing page content type for more advance/highly designed pages (including the homepage).  

**Questions:**

* In reading your notes it sounds like there is a difference in intended purpose for destination pages and landing pages, but from a functional perspective do these pages have fields or layouts that are different or unique enough to warrant two different content types?
* If yes, what do you think the different fields would be on each type?
* It’s also mentioned that pages should be “taggable” -- in what way? 

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSeemz2gd88iKLSU92MZck-kRtH_YqLEIinGXAIM8vHpwgNu7w/viewform?usp=sf_link" target="_blank">Answer Pages questions 🤔</a>

::: callout
**NDSU responses:**
* Destination vs Landing -- I don’t think so. We are OK with basic pages and landing pages as content types as described above.
* Programs -- No, programs can be part of the Ag Hub or Extension
* Additional -- Pages could be tagged to help generate lists of related content. We have a set of standard tags/keywords that will be consistent across the site.
:::

## Events

NDSU Ag & Ext will need an Events content type with the ability to add date-and-time-based events, and present in a list or calendar format. They will also need the ability to offer online registration for an event. Examples from current site(s): https://www.ag.ndsu.edu/info/cal.

* See related events questions in [Open questions](/questions)

## News/News columns

Our understanding is that all news will come from central services and that we may need one or more content types to accomodate news imports. 

* See the related news questions in [Open questions](/questions)

## Profiles

NDSU Ag & Ext will need a Profiles content type. This currently exists on a 3rd party “people” application and needs to be integrated with the new Drupal site. 

**Questions**
* Do you intend to continue to use the current People application and import that data into Drupal or do you plan to have Drupal replace that application?
* If the former, will the data in the external site match 1 to 1 with the new Drupal site? Or will you add additional data after it is imported?
* Is there an existing set of taxonomies used to group and filter profiles?
* Some pages throughout the sites have "staff listings" that appear hard-coded, and not part of a directory? Is this correct? 
* Do site “search” and “search directory” need to be combined, as they are now?


<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSe4H18_hvVzSWaDJqumoCKRRTtbzbfnr6Uc9PXmhgYW2zqUsQ/viewform?usp=sf_link" target="_blank">Answer Profiles questions 🤔</a>

::: callout
**NDSU responses:**
* People applications -- We intend to keep using our current directory
* Additional data/fields -- no, 1 to 1 match
* Existing taxonomies -- There is no mechanism providing a general query capability but there are quite a number of pre-defined groups (departments, etc.) that can be requested. A more general query capability could be added if needed. Profiles can have tags that are being used to generate directories for topic area teams and could be used for other purposes.
* Hard coded listings -- Yes, but we will be replacing those with lists generated from the directory
* Search -- Global search should search the directory as well. We would be interested in the ability to search the directory only as well.
:::

## Programs

This is a content type for Extension programs and includes event information, registration information, and description text.  Examples from current site(s):

Field to Fork (event)
Pesticide Training (course)
Master Gardener (course)
Spring Fever (event)

See: [Content type desc](https://docs.google.com/document/d/1hibGF9EzPqhJCrmshdzR_hkgxfOv7AMqAowXX1L6AFk/edit)

**Questions**
* What distinguishes a “Program” from an “Event”?  Do these content types need unique fields or could they be combined by tagged to appear in different areas of the site?
* Is there an existing set of taxonomies used to group and filter programs?Should there be?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSeg1Y19aDgB_EziPfvRqDl1K61CCF9PIwSsyQz1djogod1eyA/viewform?usp=sf_link" target="_blank">Answer Programs questions 🤔</a>

::: callout
**NDSU responses:**
* **Program vs event**
* Here are some examples of programs: https://www.ag.ndsu.edu/mastergardener, https://www.ag.ndsu.edu/preventnd. 
* They are educational programs that take place over time and include deeper learning. 
*We are trying, internally, to delineate these programs from single events or series of events which may include presentations and workshops that are not interconnected. 
*These are event series, not programs, because you could attend one presentation or workshop without losing much. 
* If you only attend one session of a program you will not complete the program or achieve the desired deep learning.
* **Taxonomies** -- Programs can be organized under relevant topic areas. We haven't thought about grouping or filtering them, but it might be helpful.
:::

## Publications

NDSU Ag & Ext will need a Publications content type long-form articles with a table of contents. 

See: [Publications](https://www.ag.ndsu.edu/publications)

See related publications question in [Open questions](/questions) 

## Alerts

These are banners that appear when needed for emergencies or other important and timely events. Site admins can create these and then choose to publish them. They could appear sitewide at a designated location (typically near the top of the page), or they could be specific to certain sections of the site (e.g. Soybean page has an aphid alert).

**Questions**
* Does our understanding align with your expectations? If no, please clarify.
* Do these need to have publish or expiration dates or can they be manually triggered?
* You mention that these would possibly be scribable by email and text. Could you talk a bit more about your vision here. That will help us to gauge what may be possible in Drupal.
* You mention these alerts would be Topic-based, could you provide some examples of how that relates to where alerts get shown and when?
* Your documentation states: “Reviewed at least every 7 days. Deleted, not archived” -- what does reviewed mean? Reviewed by who? Could these simply be unpublished instead of deleted?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSfWNyurv8IEveBenAa5e0XcxL5YEAjm12YsEJ6HIxU__0uNpQ/viewform?usp=sf_link" target="_blank">Answer Alerts questions 🤔</a>

::: callout
**NDSU responses:**
* Sound right overall? -- yes
* Scheduling -- We need the option to publish at a future date and to have them expire based on date
* Subscribable -- (sorry if that typo was ours) - Users would be able to enter an email address to mobile phone number and carrier to receive alerts on specific topics when they are posted on the website.
* Topic-based -- An alert updating COVID restrictions might be displayed throughout the site or on NDSU Agriculture, CAFSNR, Ag Hub, and Extension. An alert about a new weed issue affecting crops may display on the Ag Hub, on the Crops page, and on the page of the affected crop. An alert for an e coli outbreak in food miay display on the Food and Food Safety pages under Extension.
** Review process -- Yes, they could be unpublished after 7 days unless the creator has set an expiration date sooner than that, forcing authors to review the alerts and re-publish them, if needed, or delete them. They will not be archived. they should be reviewed by the administrator who created them.
:::

## Recipes

Currently recipes are simply content in the body field of a basic page, but it is recommended that a new content type be created for specifically for these.

Examples from current site(s): 
https://www.ag.ndsu.edu/food/recipes/beans/black-bean-chocolate-cake

**Questions**
* Does our understanding align with your expectations? If no, please clarify.
* Where will recipes live on the site? In a single, searchable list?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLScv0mh0b1_EHADokGvZ09Csuxf5250Cm654MD-4moPjKsJmyg/viewform?usp=sf_link" target="_blank">Answer Recipes questions 🤔</a>

::: callout
**NDSU responses:**
* Is our understanding correct? -- yes
* Location -- They will live in a Recipes section under the Extension Food section, in a single, searchable list.
:::

## Podcasts

The document mentions podcasts with the ability for people to manage subscriptions. This likely means a dedicated content type with views.

**Questions**
* Could you give us a bit more background on this requirement. Does this capability already exist on your site and if so where? If not, do you have an example of what you envision this looking like? 
* Will you have more than one podcast? Do they need to be treated separately with homepages for each podcast?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSfAdWnBf3XWSDvuyWEf4WQnKfzgVs5lPAw7QByKj-iaQIok4g/viewform?usp=sf_link" target="_blank">Answer Podcasts questions 🤔</a>

::: callout
**NDSU responses:**
* We are using separate microsites to host some podcasts. Others are hosted on 3rd party platforms and show notes and transcripts are posted on microsites. 
* We would like to have the ability to host podcasts on our Drupal site. 
* Here’s an example in Wordpress which includes podcast series pages with pages for each episode, the audio files, description and artwork are hosted on the Wordpress site, and the addin generates a podcast-friendly feed that can be used in Apple Podcasts, Spotify, etc. http://militaryfamilieslearningnetwork.org/podcasts
* Yes, more than one podcast with homepages for each
:::

## Plants

This is a content type for a plants database. It currently exists as a Plant Selector. We plan to duplicate this functionality as is.

Examples from current site(s): 
https://www.ag.ndsu.edu/tree-selector

**Questions**
* Does our understanding align with your expectations? If no, please clarify.
* There are 104 entries and we assume you will be manually migrating these into the new system, correct?
* Where would these be found on the site? Currently they are only in Extension? Show as list on a single page?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSfTY8HycwfuKwoW7JB73UY5ssDCGwUhtUHzhtTdjexondF2LQ/viewform?usp=sf_link" target="_blank">Answer Plants questions 🤔</a>

::: callout
**NDSU responses:**
* Overall understanding correct? -- No. Tree Selector is a standalone tool that will continue to be available. We are interested in adding a plant database that has similar functions but for learning how to grow and care for plants, not select the right tree.
* Migration? -- No. All the entries would be new, corresponding to flowers, fruits, vegetables, and houseplants, not just trees.
* Location -- They would reside under the Extension - Horticulture section of the site in a single, searchable list.
:::

## Research Reports 

We are unclear on the requirements for this content type. 

> REC content that has not been Extensionized, is not clearly actionable

**Questions**
*  Could you share a bit more about what these and how you see them being integrated into the new site?
* Is this a content type, and if so, how complex and what kinds of fields?

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSeoTQIFLKKgjpVo-F2TEquRSBXfwSl9OIyUV7wgvZQOCchnoQ/viewform?usp=sf_link" target="_blank">Answer Research Reports questions 🤔</a>

::: callout
**NDSU responses:**
* We may not need a content type for research reports. This was an internal designation we were trying to work through. There are research articles like those gathered in this annual report, https://www.ag.ndsu.edu/carringtonrec/documents/annual-reports/2019-annual-report-web.pdf, that should be available within the relevant topic area on the Ag Hub. In the Ag Hub wireframe, there is a “Latest Research” box and “See all research” link which should lead to all the research on a given topic. So there needs to be a way to delineate “research” from other content.
* No. We think we can designate research through tags/keywords.
:::

## Extension County Offices

There are 53 of these currently that appear to function as “microsites” and appear under Extension in the site’s navigation. Content includes basic information, resources, staff information, and news. It is unclear at this point if the same approach is expected on the new site.

Examples from current site(s): 
https://www.ag.ndsu.edu/extension/county-extension-offices
https://www.ag.ndsu.edu/casscountyextension


* See questions and responses in [Other content](/other)

## Research Extension Centers

Currently there are 10 Research Extension Centers and each is treated like a microsite with its own navigation. Content includes pages detailing various research, news, reports, and staff directories. The homepage highlights content found in various sections of the site. Content overall is very file-heavy (lots of links to PDFs). In the new site, these center sites live navigationally under the Ag Hub. It is unclear at this point if the same approach is expected on the new site.
Examples from current site(s): 

https://www.ag.ndsu.edu/research/research-extension-centers
https://www.ag.ndsu.edu/CentralGrasslandsREC

* See questions and responses in [Other content](/other)


## Other

* Videos (Drupal media)
* Images (Drupal media)
* Social media (how to handle, just icon links? share links?)
* Newsletters -- managed externally, subscribe links added to Drupal on relevant pages. Also, an overall landing page listing them? This may need to be a content type, if so. 

* See question regarding newsletters in [open questions](/questions)

**Questions**
* Video: It is recommended that all videos be hosted by a 3rd party, such as YouTube or Vimeo and embedded as a media type in Drupal. Will that be the case on your site or do you anticipate loading videos directly to Drupal?
* Video: You mention that the video must be captioned. It is our understanding that this happens in YouTube and not on the site. Is that your understanding, as well?
* Social media: Can you expand on your needs surrounding social? Just icon links? share links?


<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLSd_3hJuAcYjixdydyPQ168RZIVJ7oC9uOrw58gfmsOp7h0ygQ/viewform?usp=sf_link" target="_blank">Other questions 🤔</a>

::: callout 
**NDSU responses:**
* Videos will be hosted off-site and embedded
* Captioning in youtube? -- yes
* Social media -- Just icons and share links.
:::

## Careers

This is a content type for job postings.
Examples from current site(s): 
https://www.ag.ndsu.edu/careers/current-job-openings

**Questions*
* Are these specific to Ag and Extension, or does the same job posting appear everywhere? 

<a class="button bg-green-500 hover:bg-blue-500 rounded" href="https://docs.google.com/forms/d/e/1FAIpQLScgMay_bLDvyMyPI7-b4lNry_J4cVPLV3p_tvI1nctJyqS8SQ/viewform?usp=sf_link" target="_blank">Careers questions 🤔</a>

::: callout
**NDSU responses**
* Our only need for careers/job postings would be pages where openings can be listed with links to the official job listing on https://www.ndsu.edu/employment/joblist
:::

### Out of scope for now?

These are all items that were unknown prior to our initial discovery and our initial proposal. We are willing to discuss as needed but given overall project scope, budget, and timeline, these may be best left for a phase two.

* Worksheets/checklists
* Quizzes
* Data vis/interactive tables

See: [Primary Content Types](https://docs.google.com/document/d/1wYS2346FsuRB856vs30HUkO2SYo0NFyIxlIHHQHSlx4/edit#heading=h.a8xanigqye1j)








