##  react-events
 binding events in React is similar to HTML, using camel-case

```
//HTML events
<button onclick="changeText()">Click me</button>
```

```
//React events
class DrawerMultiButton extends Component {
    render() {
        return (
            <button id="submit_button" type="submit" onClick={ onSubmit }>
                <KVP value={ btnText } />
            </button> 
        );
    }
}
```
