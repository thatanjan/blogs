# What is Server side rendering?

### How does server side rendering work?

- First the client(browser) sends a request to the server.

- Browser starts parsing the HTML from top to bottom. When the parser sees the link tag for CSS it blocks the parsing process and starts downloading the CSS files. Then it starts parsing the CSS.

- After the CSS parsing is completed, the parser starts parsing the html again. As the parser parsing the html, the browser dom gets pained with content. Also with styles. Because the CSS is already parsed. That is why we put the CSS link tag at the top part of the HTML.

- After the dom is pained with the content, your webpage is now viewable. Then the parser gets the script tag at the bottom of the HTML. Now the browser will start downloading the JavaScript and then will parse the JavaScript.

- The JavaScript might be big and might take some time depends on how big the files are. Parsing javascript is heavier task than parsing HTML and CSS. That's why we put script tag at the bottom of the HTML.

- After the parsing is completed, now the webpage is now both viewable and interactive.

### Server Side Rendering Pros

- Great SEO. Because the content is already present on the HTML.

- Initial load is fast. Not the whole application data is not served by the browser. Only the necessary data for the page is sent.

- User doesn't have to see blank page on the initial load. Because the content is rendered by the HTML not JavaScript.

- No need of external libraries or frameworks.

### Server Side Rendering cons

- Frequent server calls.

- Slow navigation to any routes.

- Page refresh while visiting any routes (not necessarily).
