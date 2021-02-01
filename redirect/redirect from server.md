# Redirect in nextjs from server side

#### Suppose you want to create profile page that only a authenticated user can visit. If not authenticated then you want to redirect him/her to login page. If you are using nextjs then you have access to `useRouter` hook both on client and server side which returns a router object. That object has `push` method to `redirect` user to another url. But you can not use it on server side.

### So what is the solution?

#### You have to use nextjs one data fetching method called `getServerSideProps`. You can see the documentation from [here](https://nextjs.org/docs/basic-features/data-fetching#getserversideprops-server-side-rendering).

## The solution

#### For javascript

```javascript
export const getServerSideProps = async (ctx) => {
	// destructuring the request and response object from  the context object.
	const { req, res } = ctx

	// accessing the token from the cookies.
	const { cookies } = req
	const jwt = cookies.jwt

	// check if jwt token exist
	if (!jwt) {
		const url = `/authentication/login`
		res.writeHead(302, { Location: url })
		res.end()
	}

	return { props: {} }
}
```

#### For typescript

```typescript
import { GetServerSideProps } from 'next'

export const getServerSideProps: getServerSideProps = async (ctx) => {}
// destructuring the request and response object from  the context object.
const { req, res } = ctx

// accessing the token from the cookies.
const { cookies } = req
const jwt = cookies.jwt

// check if jwt token exist
if (!jwt) {
	const url = `/authentication/login`
	res.writeHead(302, { Location: url })
	res.end()
}

return { props: {} }
```

https://gist.github.com/thatanjan/8bddc62b3866e2b226a28b03c1225fa1

## Solution Explanation

### you have to export a function called getServerSideProps which is a async function. Function takes a parameter `ctx` which is a context object. this object has two properties. They are request and response object. Response object has a method called `writeHead`. It takes two parameter. One is status code, redirect url. If jwt is not found then call `res.writeHead` method. As a first parameter you will use `302` status code. You can read about the status code from [here](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/302). Pass the redirect url as second parameter.

```javascript
const url = `/authentication/login`
res.writeHead(302, { Location: url })
res.end()
```

#### About me:

#### My name is Anjan. I am a full stack web developer. I run a youtube channel called [Cules Coding](https://www.youtube.com/channel/UCBaGowNYTUsm3IDaHbLRMYw) where I make videos about web development, data structure & algorithm and many more. I would really appreciate if you give a visit to my channel.

#### Follow me

#### linkedin: [@thatanjan](https://linkedin.com/in/thatanjan/)

#### portofolio: [anjan](https://anjan.vercel.app/)

#### Instagram (perosnal): [@thatanjan](https://instagram.com/thatAnjan/)

#### Instagram (youtube channel): [@thatanjan](https://instagram.com/cules_coding/)

#### twitter: [@thatanjan](https://twitter.com/thatAnjan)
