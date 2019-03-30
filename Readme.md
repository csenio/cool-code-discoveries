# Cool code discoveries

 - `<> ... </>` can be used in React instead of `<Fragment>...</Fragment>`
 
 - `function({text}){ return <div>{text}</div> }` is the same as `function(props){ return <div>{props.text}</div> }`

- `()=>{return 'foo'}` is the same as `()=>('foo')`

 - `a === !!a` is a super quick way to check if something is a boolean.
 
 - `a*1===a` to check for typeof number

 - `+false` becomes 0 and `+true` becomes 1

 - `new Set()` is similar to an array but has unique values
 
 - you can cache the array length in a for loop like this `for (let i = 0, length = array.length; i < length; i++){...`
