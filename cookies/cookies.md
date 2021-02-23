If you want to set some authentication system like jwt, then you have to store your token inside client(browser).You store them either in localStorage or as a cookie. But when you perform any kind of server side operation, then you don't have access to the client. So you don't have access the cookies from server side. Then what is the solution?

### The solution.

{% gist https://gist.github.com/thatanjan/44246988c063d881d24eb9cbbcd13b2a %}

I have created a youtube video about this. You can check that out.
[![](http://img.youtube.com/vi/RECwLOZdiR4/0.jpg)](http://www.youtube.com/watch?v=RECwLOZdiR4 'Nextjs Cookies from server side')
You can access the cookies from request object inside `getServerSideProps` data fetching method. You can learn about data fetching methods of nextjs from here

`getServerSideProps` method takes context as a parameter. Context is a giant object. Request and Response object is inside the context object.

```typescript
const { req, res } = ctx
```

In the `request` object you'll find a `cookies` object.

```typescript
const { cookies } = req
```

All your cookies will be inside `cookies` object.

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
