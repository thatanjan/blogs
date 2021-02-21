# What is Client Side Rendering?

Everybody talks about client side rendering, single page application. But

- What problems does it solve?
- What is it?
- How it works?

Let's learn the problem with the traditional Server side rendering.

## Problems with Server side rendering.

- Sends Request per page.
- Heavy loads on server.
- Full page reload.
- Poor ui/ux experience when data changes frequently.

Then what is the solution?

### The solution is Client Side Rendering.

## What is Client Side Rendering?

Client-side rendering (CSR) means rendering pages directly in the browser using JavaScript. All logic, data fetching, templating and routing are handled on the client rather than the server.

##### Let's see how Client-side rendering (CSR) works behind the scenes.

- Browser first sends the request to server.
- Server sends html css response to the client. But the html is almost empty. Because all the content is rendered by javascript.
- Client starts parsing html and css. While downloading the javascript where content lives. Parsing HTML and CSS is fast but not javascript.
- A blank page is rendered to the user until the javascript is executed. Because html has no content on it.
- After the javascript is executed, all the necessary content is rendered. Now the application becomes viewable and interactive.

Let's see the pros and cons of Client-side rendering (CSR).

## Client side rendering pros

- Less Frequent server calls. Fetches all needed data at once.
- Content loading is fast after the initial loading. Because all the needed the javascript file is present on the client.
- Faster navigation to routes.
- No page reload.
- Great performance when data is changing frequently (dynamic web applications).
- Less Pressure on Server. That's why server can serve the data quickly.

## Client side rendering cons

- Might take a huge amount of time when the javascript is heavy.If the application is big then the javascript will be big. Parsing Javascript is slower than HTML and CSS. But it can be optimized with code-splitting. If you want to learn more you can read it from here.
- Blank page flickering on initial load. Because no content on the HTML.

Client side rendering is not always good or bad. It depends on various factors. It is up to you now. Know what your application is and choose what is good for your application.

#### About me:

My name is Anjan. I am a full stack web developer. I run a youtube channel called [Cules Coding](https://www.youtube.com/channel/UCBaGowNYTUsm3IDaHbLRMYw) where I make videos about web development, data structure & algorithm and many more. I would really appreciate if you give a visit to my channel.

Please Subscribe: https://www.youtube.com/channel/UCBaGowNYTUsm3IDaHbLRMYw?sub_confirmation=1

#### Follow me

linkedin: [@thatanjan](https://linkedin.com/in/thatanjan/)

portofolio: [anjan](https://anjan.vercel.app/)

Github: [@thatanjan](https://github.com/thatAnjan/)

Instagram (perosnal): [@thatanjan](https://instagram.com/thatAnjan/)

Instagram (youtube channel): [@thatanjan](https://instagram.com/cules_coding/)

twitter: [@thatanjan](https://twitter.com/thatAnjan)
