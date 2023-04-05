## Semantic HTML

Does your HTML file make sense without browser? Somebody might need to see your HTML output but they can't see the output by the browser. Someone using a Screen Reader can't see visually how the browser displays things. The Screen Reader needs to be able to read the content correctly so it can relay that to the visually disabled person.

There are tons of different tags to semantically mark them up but here are a few common ones.

### Common Semantic Tags

- `<article>` 
    - Self-contained content
    - Independently distributable
    - Content you can put somewhere else on the internet and still make sense
- `<section>` 
    - Thematic grouping of content
    - Not independently distributable
    - Sometimes subsections of an article, nested within an article
    - Sometimes independent of an article, but self-contained and could not exist w/o other sections
- `<header>` 
    - Introductory content
    - Heading of website
    - Description of tagline of website
    - Navigation links
- `<main>` 
    - Main Content
    - Should be only one of these
    - Really useful when you have a complex website
    - Need a way to tell assistive technologies what content should be focused on
    - Would be super overwhelming with a screen reader without a `<main>` tag
- `<nav>` - Section of Links
    - Most common use case is main links of website, inside of a header
    - Sometimes other sections of links rather than the main navigation, sometimes subnavigation, icons on tops of new articles, to jump to certain portions of news articles
- `<aside>` 
    - Things that are indirect to main content
    - Any content you can remove from the document without making the document confusing, can be in an aside tag
    - Usually used for sidebars but not always the case
- `<footer>` 
    - Footer of the document
    - Copyright info and all that information you see shoved at bottom of websites
