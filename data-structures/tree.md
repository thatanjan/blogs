In this blog you will learn about tree data structure.

Before you learn about tree data structure let me tell you why  
this is useful and a practical use of data structure.

### The practical example

If you are using a browser, that means you are using a tree data structure. If you don't believe open the developer tools of browser using F12 key. Go to inspect tab. If you are a front end developer you know these. The things you are seeing is a tree. Actually DOM(Document Object Model) is a tree. Even though it doesn't look like one. let's take a look of tree representation of what you are seeing right now.

Info: If you are a web developer you know this.

First we have something called a html tag. Inside the html tag there are two more tags called `head` and `body`. Inside `head` and body tags there are more tags. And again inside them there are more tags. You can also notice that these tags are getting nested more and more. Each tag is connected to a previous tag without the first tag. And you might have noticed some heirarchy in here. This is what we call a `tree` data structure.

## What is a tree data structure?

A tree data structure is a structure where each node is connected to a previous or parent node in a heirarchical order.

Ok. But that doesn't look like a tree. Let me prove it to you.

I hope this picture looks like a tree to you.

let's apply some css.

```css
.tree {
	transform: rotate(180deg);
}
```

We have just rotated our tree to 180 degrees. But it is still a tree. We have just rotated our tree to 180 degrees.

Let's see the properties and features of trees.

##### Types of Node

- Node: You can think of a node as a leaf in a tree. A node is nothing but just a element of a tree.
- Root Node: A root node is the top node that you see in the tree. It does not have any previous node.
- Parent Node: Parent node is immediate previous node connected to the current node. It is just like our real life parent. A parent can have multiple child.
- Child Node: Child node is the children of the parent node. And that makes sense right. A child can also be a parent.
- Leaf Node: Less node is a child node but not a parent node. Or simply, a leaf node is a child node that no other node is connected to it from bottom.
- Sibling Node: A sibling node is a child node connected to the same parent node. And that's what sibling means.

- Direction: The connection direction of a tree is always bidirectional or one way. It always go from top to bottom. From root node to child node and its child node and so on. If you notice the picture you will get that.
- Edge: An edge in a tree is the connection between two nodes. Suppose the connection between you and your parent.
- Path: A path is nothing but consecutive edges between source node to given node.
- Ancestor Node: All the nodes that are in the path of a source node and the target node are called Ancestor node. Like your Father ----> GrandFather -----> Great GrandFather -----> so on
- Desecendant Node: Every node in the path of your current node to the leaf node are called ancestor nodes.

- Level: Count the number of edges in the path from the root node to your current node. That number of edges are called level.
- Depth of Node: From the root node to the given node path, count the number of
  edges. Total Number of edges is the depth of that node.

- Height of Node: The total number of edges on the path from your current node to the most distant leaf node is the height of the node.
- Height of Tree: Maximum number of edges from the root node to the leaf node. A tree might have many leaf node. But you have to look for the most distant node. Then count the edges.

#### Some facts about Tree

- The height of a tree is always equal to the level of the tree
- Number of edges in the tree = (h - 1) [where h is the height of the tree]

#### Common types of Data Structures.

- General tree data
- Binary tree
- Binary Search Tree
- AVL tree
- Red-Black tree
- Splay tree
- Treap tree and ...so on

So that's it for this blog. Soon I will create a video about this blog. Until then stay safe.

### About me:

#### Who am I?

My name is Anjan. I am a full stack web developer from Dhaka, Bangladesh.

#### What problems do I solve?

I can create complex full stack web applications like social media application, blogging, e-commerce website and many more.

#### Why do I do what I do?

I love to solve problems and develop new ideas. I also enjoy sharing my knowledge to other people who are wiling to learn. That's why I write blog posts and run a youtube channel called [Cules Coding](https://www.youtube.com/channel/UCBaGowNYTUsm3IDaHbLRMYw?sub_confirmation=1)

#### Think we should work together?

##### Feel free to contact me

Email: anjancules@gmail.com

linkedin: [@thatanjan](https://linkedin.com/in/thatanjan/)

portofolio: [anjan](https://anjan.vercel.app/)

Github: [@thatanjan](https://github.com/thatAnjan/)

Instagram (personal): [@thatanjan](https://instagram.com/thatAnjan/)

Instagram (youtube channel): [@thatanjan](https://instagram.com/cules_coding/)

twitter: [@thatanjan](https://twitter.com/thatAnjan)

#### About My channel:

#### Why would you subscribe to [Cules Coding](https://www.youtube.com/channel/UCBaGowNYTUsm3IDaHbLRMYw?sub_confirmation=1)?

[ Cules Coding ](https://www.youtube.com/channel/UCBaGowNYTUsm3IDaHbLRMYw?sub_confirmation=1) will teach you full stack development. I will teach you not only the basic concepts but also the advanced concepts that other youtube channels don't cover. I will also teach you Data Structures and Algorithms with abstraction and without Math. You will also find many tutorials about developer tools and technologies. I also explain advanced concepts and technologies with simplicity.

#### So what are you waiting for?

Subscribe to [Cules Coding](https://www.youtube.com/channel/UCBaGowNYTUsm3IDaHbLRMYw?sub_confirmation=1) so that my friend you don't miss any of these cool stuffs.
