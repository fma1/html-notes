## HTML Basics

### HyperText Markup Language

HyperText means text with links. Links from one document on the web to another. Markup Language is language used to annotate some content or text.

### Tags

A tag is an annotation for content in HTML. 

If we had some text `Hello World` and wanted to annotate that in a paragraph, we would use the paragraph tag which is represented by the letter `p`. So a tag takes its name and it wraps in greater and less than signs, also known as angle brackets. And then we have the content. And then we have the closing tag, but we need to add a forward slash before the tag name and after the less than sign:
`<p>Hello World</p>`

In general, msot tags will follow this format. But there are other exceptions.

### Empty Tags (self-closing tags)

There are tags that don't enclose any content. There would be no closing tag because there would be no content to wrap.

Let's say we want a thematic break, a horizontal line (horizontal rule tag), so there would be no need for a closing tag.
`<hr>`

But now we just have an opening tag and this can be confusing to read and you might not know if there is a closing tag coming up or not. We have a syntax to make this a little easier. So we remove the greater than sign, add a forward slash and then add the greater than sign.
`<hr />`

Either syntax will work, and this is personal preference, but consistency is best.

### Attributes

Attributes are way we pass extra data to tags that will change the way the browser interprets those tags. You can think of them as function parameters. So what if we wanted to make a checkbox? 

To do this, we use the input tag that this is a user tag. But it's fairly generic and used for all kinds of input. A text input, or a date picker input. And we will see a variety of inputs. But we need a way to specify that this is a checkbox input.

So we start with the attribute name. After the attribute name we have an equal sign, and a quotation with a string. Then we close the tag like normal:
`<input type="checkbox" />`

Don't feel you need to memorize. You should know the common ones and that will come with practice.

### Comments

Just like in regular programming languages, these comments allow us to write comments in the source code that don't affect the output. 

These look similar to tags. We have a less than sign and then two dashes. That is the opening tag of the comment. The comment will continue even on a new line until the closing tag. Then we have two dashes and a greater than sign as the closing tag for the comment.

```html
<-- This
is a
comment -->
```

### Whitespace

Whitespace refers to tabs, spaces and newlines. It is largely ignored in HTML.

```html
<p>This is text</p>

<p>This
is
text</p>
```

You might expect these to be displayed differently but they are displayed the same because whitespace is ignored.

However, this can be very useful because it allows us to indent our code as we nest tags and to break up long lines of text to keep our HTML easy to read. All that said, there are ways to get around this if you do need whitespace to be displayed.

### Complete HTML file

The first line of every HTML file will be something known as the doctype. We have a less than sign, exclamation sign and then `DOCTYPE`. Then we will say `html` and the greater than sign.

`<!DOCTYPE html>`

The DOCTYPE tag just tells the web browser we want to use the most recent version of HTML.

Next we will open the html tag, which will be the root of the document and contain all of the other HTML elements as its content. It will always contain two tags, the head and the body. The head is to hold any metadata about the webpage. Information not shown on the page but important to the browser in order to render the browser. The body contains all the elements that display on the page.

In the head one tag always required. It is the title. It gives a title of the page. Web browsers use the title typically for name of tab but it can be used for search engine results.

Here we could add a paragraph of `Hello World` just we saw earlier. And once we close this tag we will have a completed HTML file and we could give it to the browser.

```
<!DOCTYPE html>
<html>
    <head>
        <title>My Blog Post</title>
    </head>
    <body>
        <p>Hello World<p>
    </body>
</html>
```
