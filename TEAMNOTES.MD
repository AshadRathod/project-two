# Team notes
This is for maintaining communication about your team's working meetings to "ship" the project.


## Tuesday, October 19 In-Class:

Still have to do:

Color in the banner switches
dynamic import --> follow Joniahs shit
Removing a slot from the header and applying styling
Create the scaffold card and file



## Thursday, October 14 In-Class:
What did you take away from the portion of class about implementing SimpleColors?
  - Having something like SimpleColors that can be added and used uniformly allows for better consistency
 
What did you learn from other groups?
	- States and keyboard navigation should be considered for the entire card but implemented wihtin the individual component classes.
  - Some groups are using different card designs as their templates.

What are your next steps?
  - Get the CSS fixed up for the whole card
  - Start breaking card into components, start with icon then banner
  - Set icon up to be determined based on type attribute
  - Adding in Slots

## Thursday, October 7 In-Class:
Refer to check-in #1

## Tuesday, October 5 In-Class:
- What are the characteristics of the card?
    - Header and sub-header
    - Visual Icon
    - Content area
    - Colorized banner, white card background, black text
- What design considerations must we take into account?
    - Scaling with heading and list
    - Color-coding the cards according to content
    - Having changeable icons
    - Styling based upon content alterations
    - Size and style of cards need to be consistent
    - Page responsiveness
    - Margins and negative space
- What accessibility concerns do we potentially have?
    - Accessing the text within the card via screen reader
    - Readability based on text size (too small/large)
    - Contrast
    - Heading order
    - Translatability
- What security concerns do we potentially have?
    - Content modification
    - SVG vulnerabilities
- What "states" does this card have?
    - Visible
    - Disabled
    - Potentially a click state?
    - Potentially focus and hover states
    - Card type
- What do we call it?
    - Simple, embedded bulletin
    - Quick facts
- What areas do we need to account for flexible content / HTML entry of any kind?
    - Header
    - Icon
    - Content formatting
    - Banner color
    - Header font
    - List element font
- Do we have room for additional reusable atoms to be produced? (there are 4 total by my count)
    Yes
- What should we call each of them?
    - The top, colorized banner (3b4b-banner)
    - Icon (3b4b-icon)
    - Skeletal card (3b4b-card)
    - Entire card (3b4b-science-card)

## Meeting notes
These are notes to be maintained PER date that you meet. What you did and what the next steps are
### Meeting Date: 
- October 10

#### What we did: 
- Discussed Properties and Design Considerations for four elements.


#### What we'll do next
- Meet some time during the week to re-evaluate roles and set up a timeline.


## Status check ins
These are dedicated status check-ins as this is a multi-week project
### Check-in 1

**Four Elements**
- *Entire card:* 
  - Possible name: 3b4b-edu-card
  - Properties: Border Thickness, Border Color, Margin
  - Design Considerations: Color Contrast between Header and content, page responsiveness, "lazy loading"
- *Scaffold of card:* 
  - Possible name: 3b4b-edu-card-scaffold
  - Properties: Banner, Content
  - Design Considerations: Styling based on Length of header text, Scaling with heading and content
- *Banner:* 
  - Possible name: 3b4b-edu-banner
  - Properties: color; font; orientation; margin/padding; icon
  - Design Considerations: Styling based on Length of header text, color based on type of card
- *Icon:* 
  - Possible name: 3b4b-edu-icon
  - Properties: padding; color; size;
  - Design Considerations: Changeability, sizing ratio
  
Next Steps
  - Looking into best way to split up work **EVENLY**
  - Looking into named slot values.
  

### Check-in 2
- [x] Basic API to render the icon based on having the correct name leveraged
- [x] Header / banner element should have a basic API supporting two named slots and implementing your icon

- [ ] Definition should be dynamically imported in the constructor or firstUpdated life-cycle of the header / banner element (reading and examples before should help inform this)

The dynamic import was not working.  When just declaring the learning-icon on line 9 of LearningBanner.js and commenting out line 5 of LearningCardCopy.js, everything disappears when running "yarn start".  Is there something with HAX we are forgetting to change?

We also attempted to use a terenary operator to determine the icon but that wasn't working well either.  Can you show an example of a multiple condition terenary operator in-class?

How come I can't apply styling to the slot tag in LearningBanner.js and all styling has to be done on the actual <p> in LearningCardCopy.js?

Also once we get the banner working fully this branch "feature/Banner will be merged back into master".

### Check-in 3
#### Sunday, October 24

Meet for 1 hour to review completed requirements for 10/24 check in. 

This week 
- Continue to make our way through the issue queue including implementing simple colors, adding in our button, finish setting up CSS variables 
- Meet through the weekdays to ensure everything is completed by the due date
- Added new issues that need to be done by the due date

### Check-in 4
#### Sunday, October 31  
Meet to review completed requirements for check-in and tuesdays due date.
  
This week
- we completed dynamic resizing of the card based on page size
- fixed our type to be more usable
- completed storybook demo
  - working on making sure icon renders correctly in storybook by itself (background color issue)
- completed testing 
- correctly placed button so it is not required 

For the due date on tuesday we need to publish our card to npm and be sure to remove unused code.
