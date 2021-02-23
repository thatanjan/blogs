# What is Server side rendering?

### How does server side rendering work?

- First the client(browser) sends a request to the server.

- Browser starts parsing the HTML from top to bottom. When the parser sees the link tag for CSS it blocks the parsing process and starts downloading the CSS files. Then it starts parsing the CSS.

- After the CSS parsing is completed, the parser starts parsing the html again. As the parser parsing the html, the browser dom gets pained with content. Also with styles. Because the CSS is already parsed. That is why we put the CSS link tag at the top part of the HTML.

- After the dom is pained with the content, your webpage is now viewable. Then the parser gets the script tag at the bottom of the HTML. Now the browser will start downloading the JavaScript and then will parse the JavaScript.

- The JavaScript might be big and might take some time depends on how big the files are. Parsing javascript is heavier task than parsing HTML and CSS. That's why we put script tag at the bottom of the HTML.

- After the parsing is completed, now the webpage is now both viewable and interactive.
