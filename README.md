# Horiseon Social Solutions Code Refactor Project
A marketing agency has enlisted help to refactor an existing site to make it more accessible. Accessibility practices ensure that people with disabilities can access a website using assistive technologies such as video captions, screen readers, and braille keyboards.

**Deployment**: https://katsign.github.io/horiseon-code-refactor/

The prompt:
## User Story

```
AS A marketing agency
I WANT a codebase that follows accessibility standards
SO THAT our own site is optimized for search engines
```

## Acceptance Criteria

```
GIVEN a webpage meets accessibility standards
WHEN I view the source code
THEN I find semantic HTML elements
WHEN I view the structure of the HTML elements
THEN I find that the elements follow a logical structure independent of styling and positioning
WHEN I view the image elements
THEN I find accessible alt attributes
WHEN I view the heading attributes
THEN they fall in sequential order
WHEN I view the title element
THEN I find a concise, descriptive title
```
# Changes
Updated the website [title] tag to be more descriptive ("Horiseon | Social Solution Services")
  
Went through each [img] tag and added alt text for screen reading, made even more specific on second run

Fixed the closing [img] tags (some extra spacing, extraneous syntax)

Changed unspecified [divs] to [section]s, including [header] [nav] [main] [article] [aside] and [footer] tags to create document flow

Linked navigation to section ids

Moved hero image from a [span] to an [img] tag in the HTML, added alt text for screen reading

Changed the h3 tags to h2 and uniformly styled, consolidated many CSS selectors for the aside and article content

Rearranged the CSS to align with document flow

Added comments to guide through the sections of HTML and CSS

# Details

The following image shows the web application's appearance and functionality:

![code refactor demo](./Assets/01-html-css-git-homework-demo.png)

**BUG:** While the appearance of the webpage matches spec and the internal links function correctly, the webpage doesn't scale down properly in a browser window.
This issue could be fixed with responsive CSS properties to ensure cross-browser compatibility.
