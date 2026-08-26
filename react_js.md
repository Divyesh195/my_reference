# OG React

1. To create an app with typescript (with forlder name "frontend")

```
npx create-react-app@latest frontend --template typescript
```

2. React Tips and Tricks <br>
(1). Wrapping elements in <Fragment> or <>..</>, will be good in case you do not want to pass a new div/section in DOM.
```
function App() {
  return (
    <>
      <h1>Hello</h1>
      <p>Welcome</p>
    </>
  );
}
```
This will return this HTML. 
```
<h1>Hello</h1>
<p>Welcome</p>
```
Without <Fragment> it will return them wrapped under a parent <div> tag, which will require adding extra CSS.
