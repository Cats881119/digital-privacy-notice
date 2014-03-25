digital-privacy-notice
======================

Entry for the Digital Privacy Notice Challenge


Notes from webinar
==================

- http://www.youtube.com/watch?v=Ywcc7N042oc
- ONC i2, improve health outcomes
- Linda Sanchez. Notice of Privacy Practices (NPP) clear, user-friendly
- integrated within websites for better patient communication
- model notices, specific statements, patients know about their rights with providers
- NPP 'document' Chief Privacy Officer, Office of Civil Rights
- model notice is paper based for providers and health plans
- can be difficult to understand and digest
- customizable. final product english and spanish. fillable PDFs three different designs + text only version
- foundation for current challenge
- background research, barriers to comprehension of notices from consumers, what was working and not
- Barbara Kingsley - findings from research. participants surprised how many entities can get their health data
- patients most interested in their rights
- trust stops after doctor
- consider a layered notice: patients won't read everything
- list rights before disclosures
- break out rights / choices / disclosures
- use hooks to gain consumer attention, highlight important information, check language for lowest reading level
- compelling, readable, understandable, easily integrated with HIPAA covered entities
- JS for interaction, html/css presentation layer
- Use content and design elements 
- Customizable by the entity [see paper-based model] enter in name, address, special notes about practices e.g. do not create/contain psychotherapy notes. describing any state laws etc
- reading vs consuming paper vs online
- MUST: no deviation from DPN model notice language. additional framing language. visual appeal. entity link to other relevant content. results from public voting.
- submissions end april 7
- Josh jshapiro at capconcorp
- customizing opportunities to connect with other information on an entity's website. clinical trials - list and link. operations purposes, link to quality assessment improvement page.
- browser requirements
- used by either plan or provider
- multilingual

Initial thoughts
================
- Needs to be integrated within provider's site, but pasting in a bunch of markup will not end well with conflicts
- iframe might be the best solution, like twitter embed - or a popup to another page or third party link
- iframe to either html content or hosted content
- html content could be generated and exported, or hosted content would get a unique link
- hosted content could be versioned
- easy drag and drop links
- jquery version could be open-source under apache license, but builder could be commercial
- layered priority
- embedder has a print option, save option, email me option
- Share / export
- Download .pdf
- customize sections
- drag and drop
- generate email
- generate docx
- new window or embedded view
- interactive 4-sq menu
- ask questions of privacy officer live
- "what does this mean?"
- crowdsourced policies e.g. see policies that other privacy officials frequently added (like NPP recipies)
- 508, color blind, print css

User Flow
=========
- Let's get started creating your 
1. Are you a health care provider or a health plan?
2. What is the covered entity's name, address, website, other
3. What is the covered entity's privacy official's information -> name, phone, email, other
4. Special notes entity's practices
5. Privacy Rule greater limits on disclosures
6. Blue Button
7. What will the effective date of the notice be? [datepicker]
8. OCHA

Markup Organization
===================
- npp-header
- npp-content
  - section-layered
    - section-layered-intro
	- section-layered-rights
	- section-layered-choices
	- section-layered-uses
  - section-rights
    - segment-opener
	- segment-bulletblock
	- segment-annotation
	- segment-break
  - section-choices
  - section-uses
  - section-responsibilities
  - section-closing
- npp-footer

License
=======
Copyright (c) 2014 Tony Webster. All rights reserved.