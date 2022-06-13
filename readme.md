# Entry Point Decorator
Mark a function as an entry point
```js
const main = entryPoint(import.meta)(async () => {
    const response = await fetch("https://jsonplaceholder.typicode.com/todos/1")
    const json = await response.json()
    console.debug(`Got JSON from ${response.url}: ${JSON.stringify(json, undefined, "\t")}`)
})
```
