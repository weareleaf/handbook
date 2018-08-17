# [The Design Handbook](#)

## Table of Contents

* [Welcome](#welcome)
* [What design means to us](#what-design-means-to-us)
* [Design tools](#design-tools)
* [Design process](#design-process)
* [Our approach](#our-approach)
* [Design standards](#design-standards)

## Welcome

Design is a loaded word, meaning very different things to different people, and the Designer's Handbook is intended to help define exactly what we think of as design.

## What design means to us

### Content is everything

An interface, in any form, is simply a window into the conversation you're attempting to have with your users. Whether you're using words, images, or any other medium to communicate, agonising over the content itself will always, always be the priority.

### Design isn't just for designers

At Leaf, it's important to recognise that design is not simply a skill or service applied solely by a designer. If the output of your work directly impacts the product, you're designing.

### Design is purposeful

If you're not solving a problem, you're not designing. Well understood design problems combine objectives, business considerations, and technical, time and resource constraints. If you're unsure of the problem you're solving, it's highly likely that you haven't got all of the answers yet.

## Design tools

You're encouraged to use the tools that enable you to get ideas out of your head and in front of people most efficiently, but there are some tools that we either recommend or require you to use so that we can all play nicely together.

### Sketch

[Sketch][1] is our primary design tool of choice. It's affordable, well documented, and has a big community behind it. It's also great at producing anything from low-fi wireframes to hi-res mockups.

### Photoshop

While [Photoshop][2] is no longer the industries de facto product design tool, it's still King for any kind of photo manipulation or batch-changing of imagery.

### Marvel

Selling a vision with words alone can be tough, but being able to share something tangible can make all the difference. [Marvel][3] quickly turns static designs into interactive prototypes, ensuring a shared understanding among stakeholders.

## Design process

While we're not big on overly proscribed processes, our approach to solving design problems tend to follow a similar pattern.

### Content

When people think of design, they rarely think of words. In reality, the words are by far the most important part of the design process; that purple gradient won't save you if users aren't finding the right words at the right time.

For content-heavy projects, we'll usually start our design work in [Google Docs][4]. Content should always be written with an awareness of not only who it's for, but how they will be consuming it; context, as usual, is everything.

Get in the habit of indulging in content rather than drop shadows. Write, read, and re-write; spending time to get the content right will make every additional step that much easier.


### Sketches, wireframes, and prototypes

With the content well shaped, a low-fidelity approach is often the next natural step. At this stage, you'll be exploring various ideas, considering a number of layouts, and chucking away more of your work than you keep.

By focusing our time on the hierarchy and layouts, we minimise our wastage. Sketching, either with pen and paper or digitally, helps us generate (and quickly rule-out) new ideas, while wireframing and prototyping enables us to validate our theories.

### Visual design

With the foundation solid, we're finally well placed to explore the visual design. At this point, brand guidelines can be added, and typography, colour and form explored for the first time.

When layering the various areas of design in this way, there has to be a degree of flexibility between the phases. After weeks or months of hard work, nobody wants a coloured-in wireframe; adhering to the wireframes is preferable where possible, but you shouldn't feel powerless to make design decisions at this stage.

## Our approach

### Design for everyone

It's easy to craft an interface for an able bodied individual, imagining they're using the same iMac with super-fast broadband as you are, but that's not how the World works. _Anyone_ should be able to enjoy the web, irrespective of their physical, mental, or situational ability to do so.

### What problems are we solving?

Time is our primary commodity in every area of the business, and design is no exception.

Always be lead by the actual issue we're collectively tackling; what are we looking to achieve? How best can we use our time budget to solve the problem? We have a finite amount of resource; stay focused on the issues at hand, and tackle them appropriately.

### Talk to people

No one person is ever right all the time, and it's essential we talk to the right people throughout the process. If you're unsure of anything, ask your teammates; a fresh set of eyes can be incredibly valuable.

From an external point-of-view, keep the conversation with stakeholders flowing to make sure we're on track, and wherever possible, ensure actual users involved; they'll know better than anyone if our solution is missing the mark.

### Remember who you're designing for

Above all else, the actual user is always the most important person. Throughout your work, from the first conversation to the final line code, be mindful of who you users are.

How are they consuming your work: are they relaxed in an office, or rushing to catch the tube? What does their environment look like? What concerns are they likely to have in this moment? Think deep, and put yourself in their shoes at all times.

### Embrace constraints

Constraints help narrow our field of vision, providing direction to immovable issues by allowing us to focus on the unsolved issues at hand.

Constraints can sit across any number of areas, from the budget or time allocated to solving an issue, to the structure of content being served from an existing CMS.

First, determine if it really is a constraint, or whether outdating or misguided thinking lead us to incorrectly believe as much? If it really is a constraint, embrace and own it.

### Design with scale in mind

Relative units, such as `em`s and `rem`s, allow us to use parent elements to manipulate the interface. By creating relationships between elements, design decisions are inherited by child elements, saving us both time and unnecessary lines of cumbersome code.

## Design Standards

### Optimisation of assets

Just as important as designing for slow and unstable connections is optimising assets at every opportunity. SVG's generated by design software such as Illustrator or Sketch rarely output efficient HTML, though Sketch's output can be improved vastly by installing the [SVGO Compressor plugin][5].

Images should always use the most appropriate file format, and be automatically compressed. Responsive images, where appropriate, should be used to serve only the most appropriate assets for any given situation.

### Animation

Well considered animations go far beyond visual interest, creating affordances that help the user interpret complex interactions.

Before introducing transitions into your work, consider exactly what the animation is bringing to the table; are the benefits worth the additional code and cognitive cost to the user? If the argument in favour is such that you do decide to add them, always use properties and techniques that allow us to achieve 60fps.

### Styleguides

Styleguides and Pattern libraries promote a consistent design language, informing future design decisions for more efficient development process.

Well-built digital products are simply a collection of reusable elements, either used in isolation or combined with one another,  to create a user interface.

Unless you can make a compelling argument for introducing additional variance and complexity to the design system, you should always look to reuse existing styles. That said, the needs of the user are always paramount, and should never be compromised for the benefit of the system or the the engineer.

### Atomic Design

We use [Brad Frost's Atomic Design][6] methodology to organise our design systems. In biology, collections of particles group together to form an organised system, and Atomic Design adopts the same hierarchical approach to product structure.

Elements that collectively form a product can be divided into five distinct areas: Atoms, Molecules, Organisms, Templates and Pages.

#### Atoms

The humble atom is the basic building block of any product, and is usually found is various combinations to create more complex artefacts. An atom can be anything that cannot be broken down further, such as headings, inputs, and buttons.

#### Molecules

Molecules are fairly simple collections of atoms, functioning together to form something purposeful. While atoms tend to lack usefulness in isolation, molecules create relationships that provide genuine functionality within the microsystem.

#### Organisms

Organisms are complex collections of atoms, modules, and even other organisms. If a collection of links (atoms) formed the primary navigation (molecule), that along with a logo (atom) would form the header (organism).

#### Templates

A template is a collection of atoms, modules and organisms that create the blueprint of an entire page. Templates are entirely reusable, and focus primarily on the content structure, rather than the content itself.

#### Pages

Finally, we're able to generate actual pages by applying real-World content to our templates. Pages are the most refined piece of the Atomic Design system, and the embodiment of a complex and  considered design system.

[1]: https://www.sketchapp.com
[2]: https://www.adobe.com/uk/products/photoshop.html
[3]: https://marvelapp.com
[4]: https://www.google.com/docs/about
[5]: https://github.com/BohemianCoding/svgo-compressor
[6]: http://atomicdesign.bradfrost.com/table-of-contents
