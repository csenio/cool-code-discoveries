#  ✨Cool code discoveries

 - [JavaScript](#JavaScript)
 - [React](#React)
 - [css](#css)
 - [html](#html)
 
 
 
## JavaScript

- there's a lot of standard built in objects in JavaScript that you may never have heard of https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects

- `({text})=><div>{text}</div> ` is the same as `function(props){return <div>{props.text}</div>}`

 - `+false` becomes 0 and `+true` becomes 1
 
 - `+"1"` becomes `1`

 - `new Set()` is similar to an array but has unique values and can be more easilly modified.
 
 - you can cache the array length in a for loop like this `for (let i = 0, length = array.length; i < length; i++){...`
 
 - if you want to cut off part of  `const arr = [1,2,3,4,5]`  you can do `arr.length = 3` and `arr` will be `[1,2,3]` 
 
  - long conditional chains like this `name === 'foo' || name === 'bar' || etc..` can be simplified like this `['foo','bar',etc...].includes(name)`

 - you can destructure nested objects: `const { object: {nestedProp, nestedObj: {deeperNestedProp}}} = parentObj`

 - `a === 5 ? true : false` is the same as just writing `a=== 5`. This can be combined with the tips before to shorten some code `+(a===5) //1 : 0` (in production the ternary operator is prob. a better idea though)
 
 - you can get all the remaining items that you did not specifically destructure out of an object like this: 
```
const foo = {
  a:1,
  b:2,
  c:3
}

const {b,...rest} = foo
console.log(b) // 2
console.log(rest) // {a:1, c:3}
```

 - there is a shorthand for declaring methods 
```
const arr = {
  sayHi(name){console.log('hi',name)}
}
```
is the same as
```
const arr = {
  sayHi: function(name){console.log('hi',name)}
}
```

## React

 - `<> ... </>` can be used in React instead of `<Fragment>...</Fragment>`

 - you can use the `useReducer` hook with just simple arrow function `const [toggle, setToggle] = useReducer(toggle=>!toggle, true)` (more of a shift in mindset than a hack)
 
 - need to access dom properties of mapped/many elements? simply put a `ref` on the parent and use `ref.current.childNodes`
 
 ## css

 - `*{margin: 0; padding: 0;}` is a common way to get rid of all predefined margins/paddings. 
 
 ## webpack

 - you can configure aliases so that you can do `import {btn} from 'components'` instead of `import {btn} from '../../../components'` https://webpack.js.org/configuration/resolve/
 
 ## html
 
  - there is a `<picture>` tag that lets you create images with responsive resolutions. The video tag does the same.

