##  jsx

```
const HelloWorldComponent = () => (
        <div>hello world!</div>
        ); 
ReactDOM.render(<HelloWorldComponnet />, 
        document.getElementsById("root") );
```

compiled 
``` 
const HelloWorldComponent = () => (
        React.createElement("div", null, "hello world!");
        ); 
ReactDOM.render( 
        React.createElement(HelloWorldComponent), 
        document.getElementsById("root") ); 
```
