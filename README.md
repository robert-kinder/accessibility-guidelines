# Web Content Accessibility Guidelines Summary

This document will help you quickly get up to speed with the [Web Content Accessibility Guidelines 2.1](https://www.w3.org/TR/WCAG21/) (WCAG), and avoid common accessibility-related mistakes.

Click on each guideline to see details and code examples.

This summary is a simplification. If you're not sure how to meet a requirement, check the official [Web Content Accessibility Guidelines 2.1](https://www.w3.org/TR/WCAG21/).

---

### 1. Easy to perceive

Your website/app must present information in ways people can recognise and use, no matter how they consume content (for example if they have low vision, or use assistive technologies like a screen reader).

#### 1.1. Provide text alternatives for images

Where | What
--- | ---
*Content Code Design* | [Text alternatives for images](guidelines/1.1.1.md): Provide a text description for images, unless they are purely decorative. Make sure the description conveys the same message or functionality.
*Code* | [Decorative images](guidelines/1.1.1.md): If an image doesn't convey any information, make sure that this is indicated in code.

#### 1.2. Provide alternatives for audio content, videos and presentations

Where | What
--- | ---
*Content* | [Transcript (audio-only content)](): For audio content that has no video (like a podcast), provide a transcript.
*Content* | [Captions (videos and presentations)](): For videos and presentations (both live and pre-recorded), provide captions.
*Content* | [Text or audio description (videos and presentations)](): For videos and presentations, provide an equivalent text description, or an audio description of what happens on screen.
*Content* | [Audio description (videos presentations if pre-recorded)](): For videos and presentations that are pre-recorded, provide an audio description of what happens on screen, even if you've already provided a text description. |


#### 1.3. Create content that can be presented in different ways

Where | What
--- | ---
*Design Code* | [Structure and relationships](guidelines/1.3.1.md): When designs convey a structure visually (like distinct sections within a page, or a label next to a checkbox) that structure must also be identified in code.
*Code* | [Order of elements in code](guidelines/1.3.2.md): Make sure that elements appear in a logical reading order in code, so that they are presented in a meaningful order to screen reader users.
*Design* | [Instructions don't rely on sensory characteristics](): If you give tips or instructions, don't assume that users can perceive colour, size, shape, sound or the location of elements on screen.
*Design Code* | [Orientation](guidelines/1.3.4.md): Make sure a page's view is not locked to either portrait or landscape mode, unless this is essential.
*Code* | [Purpose of text fields](): If a text input field collects information about the user, identify its specific purpose in code (e.g. email, password, street address).

#### 1.4. Make content easy for people to see and hear

Where | What
--- | ---
*Design* | [Audio control](): If any audio content plays automatically for more than three seconds, give people a way to stop it.
*Design* | [Use of colour](): Do not use colour as the only way to convey any piece of information.
*Design* | [Text contrast](): Make sure that text has enough contrast against the background colour.
*Design* | [Non-text contrast](): Make sure that visual information that identifies important graphics, interactive controls and their state has enough contrast against adjacent colours.
*Design Code* | [Resize text](guidelines/1.4.4.md): Make sure it is possible to complete all tasks when text is resized up to 200%.
*Design Code* | [Reflow](guidelines/1.4.10.md): Make sure users can access all information and functionality on a screen that's as wide as on the iPhone5, without needing to scroll in both directions.
*Design Code* | [Text spacing](): Ensure that no information or functionality gets lost if users increase the space between lines, paragraphs, letters and words.
*Code* | [Images of text](): Use real text rather than images of text.
*Code* | [Extra content on hover or focus](): If content (like a tooltip) appears when users hover over an element with their mouse (or tab to it with their keyboard), it must be easy to dismiss, easy to reach and remain visible.

---

### 2. Easy to operate

Your website/app must be easy to navigate and use, no matter how someone interacts with it. 

For example people who don't use a mouse may use their voice, or press the 'Tab' key to move their keyboard's focus to interactive controls.

#### 2.1. Make all functionality work with a keyboard

Where | What
--- | ---
*Code* | [Keyboard](): Make sure every task can be completed using just a keyboard.
*Code* | [No keyboard trap](): Make sure that keyboard-only users don't get trapped within any element.
*Design Code* | [Keyboard shortcuts](): If you've added custom keyboard shortcuts, provide a way to switch off or remap these shortcuts.

#### 2.2. Give people enough time to read and use content

Where | What
--- | ---
*Design Code* | [Timing adjustable](): If there is any time limit (like a session timeout), give people an easy way to extend it.
*Design Code* | [Visual distractions](): Do not show anything that automatically blinks, scrolls, animates or updates frequently if it lasts more than 5 seconds. Or give people a way to stop it.

#### 2.3. Do not cause seizures

Where | What
--- | ---
*Content Design* | [Flashes](): Do not show anything that flashes more than three times a second.

#### 2.4. Help people navigate and find content

Where | What
--- | ---
*Design Code* | [Skip to main content](): Give keyboard and screen reader users a way to go directly to the page's main content. [Web only]
*Design Code* | [Page titled](): Give every page a unique and helpful title that indicates the purpose of the page. [Web only]
*Design Code* | [Heading and labels](): Provide headings and form labels that help people find content and complete tasks.
*Design Code* | [Focus order](): Make sure that interactive controls receive focus in an order that makes sense, when users navigate through them with the keyboard.
*Design Code* | [Focus visible](): Make sure that keyboard-only users can clearly see which interactive control is focused when they tab through them.
*Design Code* | [Link purpose](): Make sure the purpose of every link is clear from the link text alone, or together with associated content (if screen readers recognise the association).
Design | [Multiple ways to find a page](): Give people different ways of finding each page (like searching or browsing links), unless the page is a step in a process.

#### 2.5. Make it work with other input methods beyond keyboard

Where | What
--- | ---
*Design* | [Complex gestures](): Do not require complex gestures or using more than one finger to do things.
*Code* | [Touch or click activation](): Make sure that custom buttons or links do not activate as soon as they are touched, so that users can slide their finger or mouse away to cancel the action.
*Code* | [Label in name](): When an interactive control has a name on screen, make sure that assistive technologies (like Voice Control) know it by the same name (or a name that includes the name on screen).
*Design Code* | [Device motion](): If a feature uses the device's motion (like shaking or tilting), make sure that responses to these motions can be turned off, and that the feature can be used in another way.

---

### 3. Easy to understand

Your website/app must make it easy for people to understand information and how to complete tasks.

#### 3.1. Make text easy to understand

Where | What
--- | ---
*Code* | [Language of page](): In code, identify the language that the content is written in. If the page uses several languages, identify the language of each section.

#### 3.2. Make things appear and behave in consistent, predictable ways

Where | What
--- | ---
*Design Code* | [Changes on focus](): Make sure that just navigating to an interactive control with the keyboard doesn't trigger any action, and doesn't move the keyboard focus somewhere else.
*Code* | [Changes on input](): Make sure that just changing the state of a form input (like a checkbox) does not cause anything surprising to happen (like submitting a form, or automatically moving the keyboard focus).
*Design* | [Consistent navigation](): Make sure that navigation controls that appear on multiple pages (like links in a header) look and behave consistently.
*Design Code* | [Consistent feature names](): If a feature exists on multiple pages, make sure that it looks the same and is named consistently.

#### 3.3. Help people avoid and correct mistakes

Where | What
--- | ---
*Design Code* | [Error identification](): When someone makes a mistake, provide an error message in text and make it obvious where the mistake was made.
*Design Code* | [Form labels and instructions](): Provide form labels to make it clear what information is expected, and optionally provide extra hints to help people avoid mistakes.
*Design Code* | [Error suggestions](): When someone makes a mistake, give them suggestions on how to correct it, unless it compromises security.
*Design Code* | [Error prevention](): If users are making a legal commitment, financial transaction, or updating personal data, give them a way to review and check the information they have entered.

---

### 4. Robust and compatible

Your website/app must work with different web browsers and/or assistive technologies.

Where | What
--- | ---
*Code* | [Valid HTML](): Make sure the code of each page does not contain errors that are known to cause conflicts. [Web only]
*Code Design* | [Name, Role and State of interactive controls](): Make sure the code of each page enables assistive technologies to discover the purpose of every feature, the way that feature is identified, and the state it is currently in.
*Code Design* | [Status messages](): Make sure status messages are identified in code, so that assistive technologies can convey them to users.
