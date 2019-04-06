# Cool code discoveries ![scraa](https://emojis.slackmojis.com/emojis/images/1521814450/3718/dabbing_unicorn.png?1521814450)



 - `<> ... </>` can be used in React instead of `<Fragment>...</Fragment>`
 
 - `function({text}){ return <div>{text}</div> }` is the same as `function(props){ return <div>{props.text}</div> }`

- `()=>{return 'foo'}` is the same as `()=>('foo')`

 - `a === !!a` is a super quick way to check if something is a boolean.
 
 - `a*1===a` to check for typeof number

 - `+false` becomes 0 and `+true` becomes 1
 
 - `+"1"` becomes `1`

 - `new Set()` is similar to an array but has unique values
 
 - you can cache the array length in a for loop like this `for (let i = 0, length = array.length; i < length; i++){...`
 
 - if you want to cut off part of  `const arr = [1,2,3,4,5]`  you can do `arr.length = 3` and `arr` will be `[1,2,3]` 

 - you can use hooks `useReducer` with just simple arrow function `const [toggle, setToggle] = useReducer(toggle=>!toggle, true)` (more of a shift in mindset than a hack)

 - long conditional chains like this `name === 'foo' || name === 'bar' || etc..` can be simplified like this `['foo','bar',etc...].includes(name)`

 - you can destructure nested objects: `const { object: {nestedProp, nestedObj: {deeperNestedProp}}} = parentObj`

 - `a === 5 ? true : false` is the same as just writing `a=== 5`. This can be combined with the tips before to shorten some code `+(a===5) //1 : 0` (in production the ternary operator is prob. a better idea tho)
 
 - there is a `<picture>` tag that lets you create responsive images.
