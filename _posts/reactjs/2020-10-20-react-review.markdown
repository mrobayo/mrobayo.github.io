---
layout: single
title:  "React Review 16.x"
date:   2020-10-20 21:00:00 -0500
categories: reactjs
---
ReactJS is a javascript framework frontend to create awesome dynamic website. At the moment 
of this post, the last version for React is 16.14.0

This post will cover the following topics:

 - React.memo()
 - useEffect()
 - forceUpdate()

{% highlight js %}

    const lambda = ({ article }) => {
        return <h1>{article}</h1>
    } 
    #> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

### React.memo() Inside

**React.memo** is a function that takes in a function as an argument
and returns a memoized function. It's used to improve performance. It
prevents to re-render if its props haven't changed. 

React.memo is a higher order component that also takes in a function as 
2nd argument that let us to validate if the next props have changed.

```javascript
const BoardPiece = ({code, color}) => {
  // render
};
function areEqual(prevProps, nextProps) {
  // return true if passing nextProps to render would return
  // the same result as passing prevProps to render, otherwise return false
}
export default React.memo(BoardPiece, areEqual);
```

#### When use React.memo() 

Imagine that you have a big table with hundreds of cells. 
Like a big appointment scheduler. **React.memo** will help us in this case.


Check out the [ReactJS][ReactJS].

[ReactJS]: https://reactjs.org/
