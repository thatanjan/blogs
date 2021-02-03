# Access Cookies in nextjs from server side.

#### If you want to set some authentication system like jwt, then you have to store your token inside client(browser).You store them either in localStorage or as a cookie. But when you perform any kind of server side operation, then you don't have access to the client. So you don't have access the cookies from server side. Then what is the solution?

### The solution.

#### You can access the cookies from request object inside `getServerSideProps` data fetching method. You can learn about data fetching methods of nextjs from here

#### `getServerSideProps` method takes context as a parameter. Context is a giant object. Request and Response object is inside the context object.

```typescript
const { req, res } = ctx
```

#### In the `request` object you'll find a `cookies` object.

```typescript
const { cookies } = req
```

#### All your cookies will be inside `cookies` object.
