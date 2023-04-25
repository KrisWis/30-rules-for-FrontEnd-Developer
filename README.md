# 30 tips for FrontEnd Developer
#### This repository contains 30 tips for FrontEnd developers that will make your code cleaner and nicer. I have tried to write all these tips in clear language, so that even the greenest beginner would understand everything :)
## Rules of introducing code for HTML
1. In the title of article tag, the h1 tag should be used. [This can be used as many times as you wish, like all h tags.](https://webdesign.tutsplus.com/articles/the-truth-about-multiple-h1-tags-in-the-html5-era--webdesign-16824) The h2 tag is used for titles or subheadings. The h3 and h4 tags are used for names of sidebars, rubrics and so on. The h5 and h6 tags are for small elements of the page, which need to be separated from the rest of the text.
2. Do not specify "http:" in links to external elements.
3. details and summary tags are used to mark up a collapsible section of content. The summary tag is used to highlight the section title, and the details tag is used to highlight the content itself.
4. The mark tag is used to highlight text that was highlighted for a reason. 
5. The div and span tags are not semantic tags, so you should try not to use them.
6. Do not specify the "type" attribute when plugging in styles and scripts.
## Code rules for CSS
7. You should avoid selectors that are or include html tags.
8. If possible write abbreviated property entries (for example, instead of padding-left, padding-top, etc., write the values in padding).
9. Not to specify a unit for null values (for example, instead of margin: 0px, write margin: 0).
10. Not to put 0 in integer part in values between -1 and 1 (i.e. instead of, for example, 0.5em, write .5em).
11. do not use inverted commas in links.
12. Sort ads in CSS alphabetically.
13. Try to use [BEM](https://csswizardry.com/2013/01/mindbemding-getting-your-head-round-bem-syntax/) for CSS.
## Code rules for HTML and CSS
14. Always use 2 spaces for indentation.
15. If possible, explain your code with comments.
## Accessibility:
16. Make video elements [accessible](https://web.dev/media-accessibility/) for people with disabilities.
17. There is an attribute [tabindex](https://www.internet-technologies.ru/articles/kak-i-kogda-ispolzovat-atribut-tabindex.html#header-45156-1) to focus on certain elements. It is useful when you want to ensure accessibility for keyboard-only users.
18. For screen magnifier users, there are 3 rules for the content that appears when hovering:
      1. Content can be dismissed without moving the focus or cursor (e.g. using Esc).
      2. The cursor can be moved from the button to the content that appears and it does not disappear.
      3. Appearing additional content remains visible until the focus or cursor is removed from the button or additional content or until the user dismisses the content with the Esc key. 
19. The Aria-label attribute helps to assign a title to the element, which is visible only to the screen reader. The Aria-labelledby attribute helps to make the screen reader read another visible name or title when focusing on the element. 
20. Aria-describedby provides additional information for the screen reader to the existing visible title.
21. Aria-disabled allows an inactive element to be included in the focus order. This means that for the screen reader user, the element will sort of not exist.
22. The "alertdialog" role allows assistive technologies and the browser to recognize a pop-up warning or error message window and sound its appearance in a special way, e.g. by playing a system warning sound.
23. The focus can only be on interactive elements, i.e. buttons, links, checkboxes, etc. The order of the focus must follow the visual or logical order of the interactive elements on the screen. Inactive controls are not focused.  
24. To see how an element should enter itself when using the keyboard it is worth looking at ['Design Patterns and Widgets'](https://www.w3.org/TR/wai-aria-practices-1.1/#aria_ex).
25. It is worth specifying the primary language of each page using e.g. the lang attribute in html lang="en". You should use the lang attribute for certain elements when the language of the element is different from the rest of the page.
26. WAI-ARIA roles can give extra meaning to the code, e.g. using role="search" to define the search functionality.
27. Need to provide clear instructions, error messages and notifications to help users complete forms on your site.
28. It's worth making sure that the order of the elements in the code matches the logical order of the information provided. One way to check this is to remove the CSS style and make sure the order of the content makes sense.
29. It's worth using responsive-adaptive website design.
30. Use WAI-ARIA to provide function and status information for custom widgets such as accordion and custom buttons. For example, role="navigation" and aria-expanded="true" (aria-expanded is set for an element to indicate whether the control is expanded or collapsed, and whether controlled elements are displayed or hidden).
