# The Design Playbook

## Table of contents

- [Purpose of the playbook](#purpose-of-the-playbook)
- [Initial questions](#initial-questions)
- [Forms](#forms)
- [Accessibility](#accessibility)
- [Psychology](#psychology)

## Purpose of the playbook

Much of what we do is about uncovering unknowns and gaps in our knowledge, applying the right approach to a given problem, and making sure appropriate best practices are used.

The playbook is our evolving first-attempt at surfacing the design expertise held individually in our heads. By investing in this asset and promoting the sharing of knowledge, we create not only a more refined design process, but more rounded individuals.

## Initial questions

- [What is the client looking to achieve?](#what-is-the-client-looking-to-achieve)
- [How will the end-user consume it?](#How-will-the-end-user-consume-it)
- [Who are our users?](#who-are-our-users)
- [How will the user be consuming our work?](#how-will-the-user-be-consuming-our-work)
- [Does the client themselves have content guidelines?](#does-the-client-themselves-have-content-guidelines)
- [Does the client themselves have design guidelines?](#does-the-client-themselves-have-design-guidelines)
- [How does our work fit into the bigger picture?](#wow-does-our-work-fit-into-the-bigger-picture)

### What is the client looking to achieve?

What is their fundamental reason for investing in this work? Projects aren't undertaken on a whim, but rather to solve a problem. To determine our own approach, we first need to understand the why we're doing it.

### How will the end-user consume it?

We don't create isolated features, but rather joined-up experienced. Where will the user come from before they see our new work? Whether it was direct from a marketing email, an internal page on the company website, or a third-party ad, we need to know exactly what was promised to them.

### Who are our users?

What demographics need to be catered for in our product? Is there a very specific type of user (e.g. a hen party booking system), or a very broad set of user groups (e.g. a county council recycling widget). Our use of colour, text size, target size, language, and design patterns are all influenced by who will be using the product.

### How will the user be consuming our work?

The expected screen size, device type, and level of distraction are just a few factors that influence our design choices. Going further, is the work more likely to be used in a well lit office, in the comfort of their home, or during a rush-hour commute? Will it be consumed in the day or in the evening? If it's the former, should we expect it to be used outside in direct sunlight?

There's no one-size-fits-all approach to interface design, and the choices we need should account for the environment that our product is likely to be consumed in.

### Does the client themselves have content guidelines?

Content guidelines help align individuals on how to write for the business or product. Documents of this ilk usually involve humanised characterisations of the company, dos and don'ts, and general suggestions on the tone of voice to use to ensure the language is both on-brand and relatable to their audiences.

Failing the presence of a formal guideline, determine who is in charge of the company content strategy to ensure our own approach is in keeping with the client's own expectations.

### Does the client themselves have design guidelines?

Is there an existing style guide or pattern library to guide our design decisions? In the absence of either, are there existing company products or brand materials that can help guide the visual presentation of our work?

There may be times where existing assets do exist, but are out dated, poorly constructed, or simply not fit for purpose. However, this should be always be a conscious decision, and an audit of current design materials should always be undertaken.

### How does our work fit into the bigger picture?

If we're building a new feature, page, step, or even product, it's essential we intimately understand where our work sits in the customers journey.

Design decisions made in isolation lack the context needed to truly understand the needs or concerns of the user they're designing an interface for. Uncover the possible routes a user has taken to get here, consider their motivation and the messaging they've seen (or not seen) already, and use it to execute a truly joined-up experience.

## Forms

- [Present forms in a single column](#present-forms-in-a-single-column)
- [Create visual relationships through proximity and white-space](#create-visual-relationships-through-proximity-and-white-space)
- [Place form labels above the field](#place-form-labels-above-the-field)
- [You probably don't want to use a dropdown](#you-probably-dont-want-to-use-a-dropdown)
- [Make the process as simple as possible](#make-the-process-as-simple-as-possible)
- [Don’t hide important supplementary helper text](#dont-hide-important-supplementary-helper-text)
- [Write implied, actionable error messages](#write-implied-actionable-error-messages)
- [Present error messages inline](#present-error-messages-inline)
- [Use field length as an affordance](#use-field-length-as-an-affordance)
- [Use address capture to infer relevance](#use-address-capture-to-infer-relevance)

### Present forms in a single column

Forms laid out across multi-columns result in a higher frequency of user error and a slower and lower completion rate. With multi-column layouts, users are more prone to both entering information in the wrong field, or even missing the field entirely.

- https://cxl.com/research-study/form-field-usability/
- https://baymard.com/blog/avoid-multi-column-forms

### Create visual relationships through proximity and white-space

Create visual associations between related labels and inputs by placing the elements close to one another, and ensuring that unrelated elements are positioned further away.

Beyond labels and inputs, look to simplify long and daunting forms by grouping related fields, creating the illusion of smaller, less overwhelming forms.

- https://www.nngroup.com/articles/form-design-white-space/

### Place form labels above the field

Users complete top aligned labeled forms at a much higher rate than left aligned labels. Top aligned labels also translate well on mobile. However, consider using left aligned labels for large data-set entry with variable optionality because they are easier to scan together, they reduce height, and prompt more consideration than top aligned labels.

- https://www.uxmatters.com/mt/archives/2006/07/label-placement-in-forms.php
- https://baymard.com/blog/mobile-form-usability-label-position
- https://www.nngroup.com/articles/form-design-placeholders/

### You probably don't want to use a dropdown

Dropdown menus are an overused and inefficient input type, with a variety of usability implications from the hiding of options to overwhelming the user with a long and daunting list of choices, not to mention their role in negatively impacting conversation rates.

On iOS devices, a dropdown required 4 separate interactions to make a single selection. What's more, if the dropdown has options that are more than 36 characters long, the description will be automatically truncated on smaller iPhones.

As a general rule of thumb, avoid dropdowns when there are more than 10, but fewer than 5 options. The most common use-case is the sorting-preference of a list, where space is limited, and the interaction non-essential.

- https://designsmarts.co/the-problem-with-dropdowns
- https://www.lukew.com/ff/entry.asp?1950
- https://baymard.com/blog/drop-down-usability
- https://www.nngroup.com/articles/drop-down-menus/

### Make the process as simple as possible

One of our primary objectives as data collectors is to make the process of proving information as frictionless and simple as possible. Look for opportunities where data can be inferred, excluded, imported, or even captured automatically (for example, via a wearable device).

### Don’t hide important supplementary helper text

Make sure any essential instructions (e.g. the format of a new password), are visible at all times. Hiding such information within helper text, tooltips, or in error messages only increases the likelihood of failed submissions and abandoned sessions.

- https://www.nngroup.com/articles/form-design-placeholders/

### Write implied, actionable error messages

Avoid using software-driven words such as 'error' or 'invalid'; the very presence of an error message, along with steps to address the issue, imply that there's a problem.

### Present error messages inline

Rather than collating and presenting errors at the top of the form, help the user to locate errors in their submission by presenting the relevant guidance next to the input in question.

### Use field length as an affordance

When possible, use the width of a field as an affordance to the length of expected user-input. A set of full-width inputs look great at a glance, but fail as visual constraints.

### Use address capture to infer relevance

The variance between address formats Worldwide is considerable, from the order and naming of information, to what's included at all; for example, in China Postal codes (not a postcode or a ZIP code) are optional.

Language and field presentation is a great way to communicate to your users who your product is intended for, and who it isn't.

- https://ux.shopify.com/designing-address-forms-for-everyone-everywhere-f481f6baf513

## Accessibility

- [Use meaningful link and button text](#use-meaningful-link-and-button-text)
- [Add clear, useful alt tags to images](#add-clear-useful-alt-tags-to-images)
- [Use descriptive headings](#use-descriptive-headings)
- [Ensure an appropriate level of colour contrast](#ensure-an-appropriate-level-of-colour-contrast)
- [Don't ever rely on colour alone](#dont-ever-rely-on-colour-alone)
- [Always include a document language](#always-include-a-document-language)
- [Always include a main element](#always-include-a-main-element)
- [Include captions when including audio or video](#include-captions-when-including-audio-or-video)
- [Useful links](#useful-links)

### Use meaningful link and button text

Where screen readers typically skip from link to link 'read more' offers little or no context.

### Add clear, useful alt text to images

Use alt tags to describe the content of the image. If the image contains data visualisations (e.g. a pie chart), use the alt text to describe the insight.

### Use descriptive headings

Screen readers allow users to skip between headings, making the headings themselves an important part of navigating a page.

### Ensure an appropriate level of colour contrast

The Web Content Accessibility Guidelines (WCAG) recommend a minimum level for colour contrast between text and background elements, ensuring accessible content for users who struggle to distinguish between particular shades or colours.

For any project, the colour contrast should pass [WCAG 2.0 AA standards](https://webaim.org/blog/wcag-2-0-and-link-colors/), with Level AAA conformance recommended for projects where a significant number of users may suffer from some sort of sight impairment.

- https://accessibility.blog.gov.uk/2016/06/17/colour-contrast-why-does-it-matter/

### Don't ever rely on colour alone

Colour shouldn't be used in isolation to indicate or infer meaning or feedback to the user. For example, the use of colour to highlight particular rows in a table, or an error on an input, should be supplemented with text and/or iconography.

- https://webaim.org/articles/contrast/

### Always include a document language

Each language has its own pronunciation rules, and you should use the `lang` attribute on the `html` element to tell assistive technologies which primary language the page content is written in. If your page  is in English for example, you'd want `<html lang="en">`.

### Always include a main element

By wrapping your page content (everything that isn't a header, navigation, or footer) in a  `<main>` element, you're defining a page landmark that assistive technologies understand.

### Include captions when including audio or video

Captions are synchronised text equivalents of the spoken word, intended primarily for users who cannot hear audio, and should be included alongside any audio and video content.

### Useful links

- https://a11yproject.com
- https://webflow.com/blog/5-ways-content-can-improve-your-websites-accessibility-and-overall-ux
- https://moritzgiessmann.de/accessibility-cheatsheet
- https://www.gov.uk/service-manual/helping-people-to-use-your-service/understanding-wcag
- https://adrianroselli.com/2017/02/not-all-screen-reader-users-are-blind.html

## Psychology

- [Organise your content into smaller groups](#organise-your-content-into-smaller-groups)
- [Only show additional features if the user asks for them](#only-show-additional-features-if-the-user-asks-for-them)
- [Position key items at the top and bottom of a section](#position-key-items-at-the-top-and-bottom-of-a-section)
- [Limit the number of choices you present to a user](#limit-the-number-of-choices-you-present-to-a-user)
- [Increase the chance of important items being noticed first](#increase-the-chance-of-important-items-being-noticed-first)
- [Make sure to include all relevant information](#make-sure-to-include-all-relevant-information)
- [Offer suggestions for faster decision making](#offer-suggestions-for-faster-decision-making)
- [Useful links](#useful-links)

### Organise your content into smaller groups

According to Miller’s Law, most people can only hold around 5 to 9 items in their short-term memory. Presenting users with long lists of content makes it harder for them to keep track of the information and remember it effectively.

If you’re working with written content for example, you can create clear visual hierarchies with headings and subheadings, and use short paragraphs with white space to separate them. By breaking content into smaller groups, it helps the user scan the information faster and recall what they’ve read more accurately.

- https://www.nngroup.com/articles/chunking/

### Only show additional features if the user asks for them

Progressive Disclosure shows the most important or common features first, and hides more advanced and secondary actions unless the user requests them. Deferring rarely used or advanced features makes applications easier to learn, and allows people to prioritise their attention on the more common or easier tasks.

A settings page is a great example of showing advanced options when requested. Instead of presenting all of the controls at once, you should only display the key settings that will benefit all users. This helps less experienced users avoid mistakes, and means they don’t have to spend time trying to understand features they don’t need.

- https://www.nngroup.com/articles/progressive-disclosure/
- https://www.shopify.com/partners/blog/progressive-disclosure

### Position key items at the top and bottom of a section

When viewing an unfamiliar list, we tend to remember the first and last items better than the items in the middle. This is known as the serial position effect, and is caused by the way in which our long and short-term memory stores new information.

Product pages are a good example of where this effect can be applied. You can help cement the key information in the users long-term memory by including the benefits of buying at the top of the page. You can also help the users short-term memory and decision making by placing the actionable purchase options at the bottom.

- https://medium.com/@coffeeandjunk/design-psychology-serial-position-effect-ca0e4cf299cb
- https://www.interaction-design.org/literature/article/serial-position-effect-how-to-create-better-user-interfaces

### Limit the number of choices you present to a user

Hick’s law states that the more choices you offer someone, the longer it takes them to reach a decision. Too many options cause people to overthink their decision, increasing the likelihood of them not choosing anything at all.

If you’re dealing with a navigation that has lots of links for example, presenting all of the links at once could become overwhelming for the user. Instead, aim to categorise the links into smaller parent groups to help users find the choices they need much faster.
 
- https://www.designorate.com/hicks-law-building-usable-navigations/
- https://uxdesign.cc/ux-inspiration-4-hicks-law-d7a8c4d9c007

### Increase the chance of important items being noticed first

The Von Restorff effect explains how we can isolate an object to make it stand out against other, similar objects. By creating a visual contrast using size, shape, or colour, the object is more likely to be noticed first and remembered for longer.

Highlighting a recommended subscription plan is a good example of using visual differences to increase the focus on one option over the others. Design cues such as a contrasting border or recommended banner (e.g. Most popular), help increase the chance of users noticing the preferred plan first.

- https://uxdesign.cc/ux-inspiration-3-the-von-restorff-effect-d0cb73f7adc5
- https://lawsofux.com/von-restorff-effect

### Make sure to include all relevant information

The ambiguity effect is when people view missing or unclear information negatively, which can impact the users' trust in your brand and make them less likely to continue using your product.

Clearly explain what your links and call to actions do, and avoid writing vague instructions or copy that could be open to more than one meaning. Being completely up-front about your intentions and what the user can expect means they don’t become confused or make a mistake.

- https://medium.com/@michaelgearon/cognitive-biases-ambiguity-effect-e0fe2c213061

### Offer suggestions for faster decision making

The default effect shows that making an option the default choice increases the chance that someone will stick with that option. Defaults can be a recommended option that predict the user's intention based on common choices, and help them understand what the expected action normally is.

If a user is entering their payment details in a checkout flow for example, you can look for opportunities to reuse previously entered information such as defaulting the payment address to match the shipping address. You could also pre-select an option such as the delivery cost. Users often scan the choices available, and if a suggested choice has already been made, users will be less inclined to decide against it.

- https://www.shopify.com/partners/blog/cognitive-load
- https://www.nngroup.com/articles/the-power-of-defaults/
- https://uxplanet.org/how-to-influence-choice-through-default-options-50e59152dc1a

### Useful links

- https://lawsofux.com/aesthetic-usability-effect.html
- https://careerfoundry.com/en/blog/ux-design/psychology-principles-for-ux-designers/#2-jakobs-law
- https://blog.prototypr.io/7-principal-psychological-phenomena-in-ux-design-1104e09fc974
- https://uxdesign.cc/the-psychology-of-ux-design-859439bc8a32
- https://www.nngroup.com/topic/psychology-and-ux/
- https://mopinion.com/guide-to-psychology-principles-in-ux-design/
