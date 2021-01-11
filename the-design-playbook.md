# The Design Playbook

## Table of contents

- [Purpose of the playbook](#purpose-of-the-playbook)
- [Initial questions](#initial-questions)
- [Forms](#forms)
- [Accessibility](#accessibility)
- [Microcopy](#microcopy)
- [Modals and overlays](#modals-and-overlays)
- [Microinteractions](#microinteractions)
- [Icons](#icons)
- [Psychology](#psychology)
- [Ethics](#ethics)

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

What is their fundamental reason for investing in this work? Projects aren't undertaken on a whim, but rather to solve a problem. To determine our own approach, we first need to understand why we're doing it.

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

There may be times where existing assets do exist, but are out dated, poorly constructed, or simply not fit for purpose. However, this should always be a conscious decision, and an audit of current design materials should always be undertaken.

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
- [More on accessibility](#more-on-accessibility)

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

Each language has its own pronunciation rules, and you should use the `lang` attribute on the `html` element to tell assistive technologies which primary language the page content is written in. If your page is in English for example, you'd want `<html lang="en">`.

### Always include a main element

By wrapping your page content (everything that isn't a header, navigation, or footer) in a `<main>` element, you're defining a page landmark that assistive technologies understand.

### Include captions when including audio or video

Captions are synchronised text equivalents of the spoken word, intended primarily for users who cannot hear audio, and should be included alongside any audio and video content.

### More on accessibility

- https://a11yproject.com
- https://webflow.com/blog/5-ways-content-can-improve-your-websites-accessibility-and-overall-ux
- https://moritzgiessmann.de/accessibility-cheatsheet
- https://www.gov.uk/service-manual/helping-people-to-use-your-service/understanding-wcag
- https://adrianroselli.com/2017/02/not-all-screen-reader-users-are-blind.html

## Microcopy

- [Build trust with your users by addressing their concerns](#build-trust-with-your-users-by-addressing-their-concerns)
- [Be concise with your writing](#be-concise-with-your-writing)
- [Keep your writing conversational](#keep-your-writing-conversational)
- [Make sure buttons clearly explain what will happen next](#make-sure-buttons-clearly-explain-what-will-happen-next)
- [Provide clear feedback for error messages](#provide-clear-feedback-for-error-messages)
- [Don’t let microcopy become a crutch for poor design](#don’t-let-microcopy-become-a-crutch-for-poor-design)
- [More on microcopy](#more-on-microcopy)

### Build trust with your users by addressing their concerns

Unfamiliarity, ambiguity, or a previous bad experience are just a couple of reasons why users are often distrustful online. One way to increase their confidence is to anticipate and address potential concerns whenever you’re asking for access, permissions, or personal information.

When signing up for a mailing list for example, well-written microcopy can help reassure the user, explaining how easily they can later opt out as well as providing clarity on how their personal information is stored.

### Be concise with your writing

Microcopy should be scannable, easily understood, and have a sense of urgency that encourages the user to take action. It should also be succinct, using clear but compact writing to help intuitively guide the user with as fewer words as possible.

The text inside a button is a good example of where conciseness is key. If you’re asking the user to upload documents for example, using “Upload your documents” can be shortened to “Upload documents”, or even “Upload” if the action is already implied within the page.

### Keep your writing conversational

Language is the number one tool for communication, so it shouldn’t be something reserved for those with stronger reading skills. Simpler words and a more casual tone of voice help an interface feel friendlier and less intimidating, and a good rule of thumb is to only use language you'd say out loud; if you wouldn't speak it, don't write it.

One way you can create a conversational tone is by avoiding complex jargon so that the copy is easily understood by everyone. Complicated words not only make your product more confusing to use, but also less inclusive considering that roughly 1 in 10 people have [some form of dyslexia][dyslexia].

[dyslexia]: https://www.nhs.uk/conditions/dyslexia/

### Make sure buttons clearly explain what will happen next

Unclear, misleading, or generic call-to-actions such as “Click here” all cause unnecessary doubts for the user about what they can expect. Not only do unclear buttons cause uncertainty for people when deciding whether to click, but it can also cause ambiguity by giving users a chance to misinterpret what will happen when they take a certain action.

Adding products to a basket for example, allows people to save items for future consideration. Users aren’t committing to a purchase at this stage, so a button labelled “Add to cart” will clearly represent this action, whereas a label such as “Get this now” would sound like a more final action that goes against the users expectations.

### Provide clear feedback for error messages

You should clearly imply that an error has occurred along with a concise explanation if more information is needed, and offer users a proactive, actionable solution to further increase the helpfulness of the message.

If someone’s login details are incorrect for example, saying something like “Your email and password do not match” doesn’t provide any helpful feedback for the user. If you were to instead use “Your password is incorrect. Want to reset it?”, not only is the error now clear and concise, but you also provide a possible solution as well.

### Don’t let microcopy become a crutch for poor design

Users should be able to immediately understand how to use your product. If the interface is poorly designed, trying to patch the experience together with microcopy results in users becoming entirely reliant on instructions in order to complete their tasks.

If you find yourself having to use lots of words for an instruction, or resorting to using copy to explain how a feature or component works, then reconsidering the actual design will be a better option then trying to write intuitive microcopy to support your users.

### More on microcopy

- https://www.ecomdash.com/writing-masterful-ecommerce-microcopy/
- https://blog.prototypr.io/writing-microcopy-e77d7bac1c0e
- https://www.smashingmagazine.com/2013/06/five-ways-prevent-bad-microcopy/
- https://www.invisionapp.com/inside-design/ecommerce-microcopy/
- https://xd.adobe.com/ideas/process/information-architecture/four-cornerstones-writing-ux-microcopy/

## Modals and overlays

- [Avoid showing modals too early](#avoid-showing-modals-too-early)
- [Keep modals relevant to the task at hand](#keep-modals-relevant-to-the-task-at-hand)
- [Don’t use too many pop-ups](#don’t-use-too-many-pop-ups)
- [Aim to keep content to a minimum](#aim-to-keep-content-to-a-minimum)
- [Always present a clear close option](#always-present-a-clear-close-option)
- [Consider the value of the modal](#consider-the-value-of-the-modal)
- [More on modals](#more-on-modals)

### Avoid showing modals too early

Presenting a pop-up as soon as someone lands on the page can feel intrusive and demanding of attention. Users may have a specific task in mind, and presenting a pop-up too early could make them more likely to close the modal, or pay no attention to it at all if it doesn’t relate to their intended goal.

If someone is new to your product for example, allow them to familiarise themself with the page and understand what the purpose of your product is. The aim is to give people a reason to stick around, and provide real value before hitting them with a 50% discount offer before they’ve even decided if your product is useful to them.

### Keep modals relevant to the task at hand

If a user is in the middle of a task, to have a modal suddenly appear would distract them from their journey. Not only can this cause them to lose track of where they are in the content, but it can be especially annoying if the modal contains information that isn’t relevant to their task.

Unless the modal relates to what the user is doing, like confirming that they’re happy to submit a form, you should really consider the value of the information and whether or not it is important enough to warrant someone’s full attention at that time.

### Don’t use too many pop-ups

Having multiple pop-ups appear within a short period of time not only creates further obstructions for the user, but too many distractions can also overwhelm people and make your site feel cluttered and disorganised.

If you find yourself needing to use lots of overlays to convey information, you should instead look for opportunities to show the content within the page itself. Not only will the user be able to refer back to the information if needed, but you also avoid repeatedly interrupting people.

### Aim to keep content to a minimum

A modal should relate to a single area of focus, and the content should be kept to a minimum so that users can easily consume the information and make a decision quickly. If you find yourself trying to fit a lot of content into the confines of an overlay, a new page or section would probably be a better solution.

Always include a heading that clearly describes the purpose of the modal, and allow for faster decision making by limiting any calls to action to no more than two. You should also keep the copy to a minimum, helping the user scan the content faster, and also reducing the risk of the overlays height becoming so big that a scrollbar is required.

### Always present a clear close option

An annoying modal is one thing, but when it’s not immediately obvious how to close it, the frustration factor can increase as users have to then spend time figuring out how to get rid of the modal before they can continue with their task.

As well as having a clear close option, both the escape button and surrounding space of the modal should be clickable, allowing users to dismiss the overlay and return to their task as quickly as possible.

### Consider the value of the modal

The content of the modal should be highly relevant to the user's task, and provide additional support to help move people along in their journey. For information that isn’t important, using a modal is distracting, and can leave people feeling annoyed and more likely to abandon what they’re doing.

If you’re asking a user to subscribe to your mailing list for example, consider a more passive approach, like placing a section at the bottom of the page that asks them for their email address once they've finished reading one of your blog posts. Not only will you avoid obscuring the content, but you won’t come across as being pushy either.

### More on modals

- https://www.nngroup.com/articles/popups/
- https://uxplanet.org/modal-vs-page-a-decision-making-framework-34453e911129
- https://uxplanet.org/best-practices-for-modals-overlays-dialog-windows-c00c66cddd8c
- https://xd.adobe.com/ideas/process/ui-design/best-practices-for-designing-overlays/
- https://uxplanet.org/modality-the-one-ux-concept-you-need-to-understand-when-designing-intuitive-user-interfaces-e5e941c7acb1

## Microinteractions

- [Consider the purpose of the microinteraction](#consider-the-purpose-of-the-microinteraction)
- [Keep the interaction simple](#keep-the-interaction-simple)
- [Encourage people to use your product](#encourage-people-to-use-your-product)
- [Be consistent with the branding](#be-consistent-with-the-branding)
- [Use what’s available](#use-what’s-available)
- [Create microinteractions with longevity in mind](#create-microinteractions-with-longevity-in-mind)
- [More on microinteractions](#more-on-microinteractions)

A microinteraction indicates that something is happening on screen in response to either a user action, or a system trigger such as a push notification. Despite being subtle, microinteractions can have a big impact on usability. Not only do they reassure users that their actions have had an effect, but they also create a more engaging experience.

### Consider the purpose of the microinteraction

Microinteractions should only be used when it’s clear they will benefit the user, and provide purposeful reassurance such as highlighting something they’ve entered as invalid. If it isn’t clear that a microinteraction will make the user’s task easier, then you may run the risk of confusing people rather than helping them.

When designing a form for example, you can use microinteractions for inline validation such as checking if an email address format is correct, or whether a reconfirmed password matches. By providing relevant and real-time validation, you give people immediate reassurance instead of greeting them with an error when they try to move onto the next step.

### Keep the interaction simple

Similar to being purposeful, microinteractions should also require minimal effort from the user in order for them to understand what is happening. If you aren’t able to clearly communicate to users what is taking place on screen, you run the risk of leaving people unsure about what the interface is telling them.

With inline validations for example, the presence of a checkmark would be enough to quickly confirm that the information is valid. Not only that, but the simplicity of the microinteraction means it avoids becoming annoying or distracting to the user.

### Encourage people to use your product

A product should be easy to use, but that doesn’t mean it can’t be enjoyable for people and keep them engaged through fun and meaningful microinteractions. These tiny details can create a more memorable experience that encourages people to continue using your product.

If you’re designing a to-do list for example, you could add a subtle effect such as a confetti explosion when a task is marked as complete. The actual interaction would remain clear and functional, but the extra attention to detail would make the experience feel fun and unique, leaving a more lasting impression on your users.

### Be consistent with the branding

Every element or feature on a page, including microinteractions, should look and feel like they are part of the same brand. Without consistency, the microinteractions will feel out of place from the rest of your product.

If your branding is fun and geared towards creating enjoyable experiences for example, you could use more creative animations such as a donut themed loading spinner when refreshing the page. If your brand has a more corporate identity however, then dial back on the adventurous animations in order to match a more professional tone.

### Use what’s available

Using what’s available means you don’t add more components than is necessary to feedback information. Although budget and time constraints should be considered, if you do have the scope to be more intricate with your microinteractions, you should definitely aim to reuse elements where possible to create a more seamless interaction.

A ‘Submit’ button that transitions into a loading bar for example, shows that the action has had an effect, and also creates a more connected experience that doesn’t require the use of multiple components or seperate screens to confirm that an action has taken place.

### Create microinteractions with longevity in mind

Microinteractions should be equally helpful or enjoyable every time the user interacts with them. This ties into keeping microinteractions both simple in terms of animation, and purposeful for the context in which the microinteraction is needed. Will people still find value in the interaction after the 100th time they see it? Will the interaction become more frustrating than fun over time?

Making sure the microinteractions provide value at all times is important, but you also don’t want to end up annoying your users either. A menu that bounces in with a spring may look impressive at first, but when someone needs to use that menu regularly for work, is it really better than having no animation at all?

### More on microinteractions

- https://microinteractions.com/what-is-a-microinteraction/
- https://www.nngroup.com/articles/microinteractions/
- https://www.toptal.com/designers/product-design/microinteractions-better-ux
- https://www.uxpin.com/studio/blog/ux-design-best-practices-refined-microinteractions/
- https://webflow.com/blog/3-essential-microinteraction-design-tips
- https://uxdesign.cc/microinteractions-101-essential-tips-for-powerful-microinteractions-f1f52089a801

## Icons

- [Include text labels where necessary](#include-text-labels-where-necessary)
- [Keep it simple and avoid lots of detail](#keep-it-simple-and-avoid-lots-of-detail)
- [Maintain a consistent style in your icon set](#maintain-a-consistent-style-in-your-icon-set)
- [Favour optical over mathematical alignment](#favour-optical-over-mathematical-alignment)
- [Design with size and structure in mind](#design-with-size-and-structure-in-mind)
- [Use an icon set that suits your brand personality](#use-an-icon-set-that-suits-your-brand-personality)
- [Remember the 5 second rule](#remember-the-5-second-rule)
- [More on icons](#more-on-icons)

### Include text labels where necessary

Unless an icon is universally recognised (e.g. a house to represent the homepage), its meaning may not be immediately clear without an associated label that describes the icon in plain text. When someone has to work to interpret an icon, you run the risk of not only slowing them down, but leaving them feeling less in control.

For icons that aren’t as well recognised or understood, make sure to include a label that clearly describes the icon’s meaning, and avoid hiding the label behind a hover action so that there’s no risk of users missing it. As well as better communicating meaning, a label will also create a larger click/tap area where the icon is used as part of a link.

### Keep it simple and avoid lots of detail

Icons should be easily scannable, and easily remembered. Too much detail can actually slow users down, and hinder their ability to recognise an icon's meaning quickly. More complicated icons can also make it harder for people, especially first-time users, to understand what an icon represents when interacting with it.

Be sure to minimise the amount of detail in the icon, and focus on the most important and recognisable elements of the object or action you’re representing. If you’re creating a home icon for example, square walls and a triangular roof will be much easier to understand at a glance.

### Maintain a consistent style in your icon set

Inconsistent icon styles can quickly make a design feel unbalanced and disorganised. When using icons within close proximity of one another, make sure that their weight, colour, and general form are consistent across all of the assets.

When using an icon set, or creating one from scratch, make sure that every icon looks and feels like it’s from the same gene pool. This means using the same stroke widths, colour palette, and attributes the set collectively share.

### Favour optical over mathematical alignment

An icon may be perfectly aligned, but the more abstract a shape becomes, the harder it is for our brains to process the alignment properly. This tends to be more noticeable if the icon has prominent variations in weight, such as the left side of a play button being taller, and thus heavier than the right side.

You should always favour your own instincts and align optically if you’re unsure, as any imbalances, no matter how small, can have an impact on our perception of the icons alignment. By creating an icon that appears to be perfectly aligned, they will feel more premium and balanced, and also work better for your users natural perception.

### Design with size and structure in mind

Icons that are designed at one scale but used at another may suffer from alignment or distortion issues when they’re resized. These problems can make it harder for users to understand what the icon represents, and ruin the aesthetic of both the icon and the product as a whole.

Always design your icons for the size they will be used at, and where possible, use a grid system to maintain a level of structure and consistency across the set. Not only will your icons feel more harmonious overall, but you’ll make it easier to create new icons in the future if the scale and grid template are already in place.

### Use an icon set that suits your brand personality

Icons can help embed your brand's identity into the product, showing customers that you care about the small details, and even enhancing brand recognition if your icons are particularly distinctive. Icons that are off-brand can make the experience feel inconsistent, and potentially confuse users if they feel like they shouldn’t be a part of the overall experience.

Try to use colours and styles that match the tone of your brand, like simple flat icons for corporate organisations, or playful illustrations for the more creative brands. When done right, you can bring your brand’s personality to life in unique and interesting ways, whilst also helping to enhance the aesthetic appeal of your product.

### Remember the 5 second rule

If it takes you longer than 5 seconds to think of an icon, it probably means the action or instruction you’re trying to represent can’t clearly be expressed visually alone.

When deciding whether to use icons, make sure you research your competitors beforehand to see what kind of icons they are using. Through this research, you’ll be able to determine whether or not an icon is the best approach, and what the alternatives are if not.

### More on icons

- https://www.nngroup.com/articles/icon-usability/
- https://uxdesign.cc/7-principles-of-icon-design-e7187539e4a2
- https://www.toptal.com/designers/ui/icon-usability-and-design
- https://www.smashingmagazine.com/2016/10/icons-as-part-of-a-great-user-experience/
- http://blog.icondesignlab.com/en/2018/10-mistakes-in-icon-design-that-confuse-users/
- https://medium.com/ringcentral-ux/eyeballing-or-optical-alignment-in-design-4ef5ab2d326f

## Psychology

- [Organise your content into smaller groups](#organise-your-content-into-smaller-groups)
- [Only show additional features if the user asks for them](#only-show-additional-features-if-the-user-asks-for-them)
- [Position key items at the top and bottom of a section](#position-key-items-at-the-top-and-bottom-of-a-section)
- [Limit the number of choices you present to a user](#limit-the-number-of-choices-you-present-to-a-user)
- [Increase the chance of important items being noticed first](#increase-the-chance-of-important-items-being-noticed-first)
- [Make sure to include all relevant information](#make-sure-to-include-all-relevant-information)
- [Offer suggestions for faster decision making](#offer-suggestions-for-faster-decision-making)
- [More on psychology](#more-on-psychology)

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

### More on psychology

- https://lawsofux.com/aesthetic-usability-effect.html
- https://careerfoundry.com/en/blog/ux-design/psychology-principles-for-ux-designers/#2-jakobs-law
- https://blog.prototypr.io/7-principal-psychological-phenomena-in-ux-design-1104e09fc974
- https://uxdesign.cc/the-psychology-of-ux-design-859439bc8a32
- https://www.nngroup.com/topic/psychology-and-ux/
- https://mopinion.com/guide-to-psychology-principles-in-ux-design/

## Ethics

- [Give users full control over how they share their data](#give-users-full-control-over-how-they-share-their-data)
- [Always be transparent about additional costs](#always-be-transparent-about-additional-costs)
- [Never deliberately trick or mislead users](#never-deliberately-trick-or-mislead-users)
- [Consider the value of default options](#consider-the-value-of-default-options)
- [Don’t persuade users to do something that benefits only you](#dont-persuade-users-to-do-something-that-benefits-only-you)
- [Respect your users and their choices](#respect-your-users-and-their-choices)
- [Be mindful of addictive design patterns](#be-mindful-of-addictive-design-patterns)
- [More on ethics](#more-on-ethics)

### Give users full control over how they share their data

Not only should sharing data be something that’s entirely at the user's discretion, but companies should never leave a user feeling suspicious by asking for personal information without a reason as to why it’s necessary.

When getting a user to sign up to a mailing list for example, make sure to explicitly ask for their consent as well as explain why the information is needed. You should also give reassurance that the details will be kept private, and that consent can be removed at any time.

### Always be transparent about additional costs

Additional costs have always existed, but it becomes unethical when companies lead the user into thinking they’ll be paying less for a product by not showing any additional prices at the start of the process.

When creating a checkout flow for example, every cost including VAT and shipping should be visible as early as the basket. This allows users to make a more informed decision about continuing, and doesn’t give them any negative surprises at the end once they’ve already invested their time and effort into the process.

### Never deliberately trick or mislead users

Misleading users can potentially cause them to lose trust in your company and feel suspicious of how you operate. This can be through unclear instructions or calls to action that deliberately trick people into doing something, purely for the needs of the business as opposed to the user.

A checkbox that asks if the user would like to receive marketing emails for example, should require the user to check the box in order to consent. Having them check the box to opt out goes against the normal expectation, and means they may accidentally agree without realising.

### Consider the value of default options

Users tend to trust suggestions as they believe you have their best interests at heart. Although this can speed up decision making, companies can also take advantage of the psychology behind sticking with defaults because users trust that we want what’s best for them.

When automatically defaulting a subscription plan for example, make sure that the recommended option is truly the most appropriate for the majority of users. As soon as you default an option purely for the benefit of the business, you’re unethically placing your own goals above the needs of the user.

### Don’t persuade users to do something that benefits only you

Persuasive design is good for encouraging users to do something, but it can also be used to tempt users to perform an action simply because it stands out as being correct, regardless of whether it truly benefits them.

If you’re asking someone if they’d like to consent to sharing their data for example, both the agree and disagree options should hold equal weight to remove any bias towards one option. This isn’t the same as an action that affects only the user though, such as confirming whether someone really wants to delete a file by making the ‘Delete’ button red for example.

### Respect your users and their choices

Deliberately making a user feel bad in an attempt to change their mind or get them to do something can often have the opposite effect, leaving them feeling annoyed, guilty, and potentially hesitant to continue using your product.

An example would be asking a user if they’d like to keep up with daily health tips, with the decline option being “No, I don’t want to be healthy”. Make sure to list the benefits clearly, but don’t try and force them into making a decision. A simple “No thanks” is enough to allow the user to decline without the added guilt of saying no or feeling like they're missing out.

### Be mindful of addictive design patterns

Infinite scroll, push notifications, and autoplay are just a few features that can drive addiction. Although these patterns are intended to improve the user experience, they can form addictive behaviors that designers should be aware of.

When thinking about push notifications for example, make sure to really consider the value of the notification, and give people full control over how they receive alerts. By offering users a way to customise their notifications, such as what they receive and when, you encourage them to minimise distractions and reduce the urge to routinely check their phone.

### More on ethics in design

- https://blog.prototypr.io/design-ethics-c739bcf511fe#:~:text=Ethics%20within%20UX%20design%20can,our%20pursuit%20of%20ethical%20design.
- https://uxdesign.cc/10-principles-for-ethical-ux-designs-21faf5ab243d
- http://ethicalstorytelling.com/unethical-design/
- https://darkpatterns.org/types-of-dark-pattern
- https://www.vice.com/en_us/article/jpggwk/confirmshaming
- https://uxplanet.org/app-addiction-the-invisible-plague-73447926d734
- https://blog.rescuetime.com/why-addicted-to-notifications/
- https://3sidedcube.com/ethics-in-ux-design/
