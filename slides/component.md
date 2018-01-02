
- Presentational component

```
class DrawerButton extends Component {
   // ... 
    render() {
        const { btnText } = this.props;

        return (
            <div>
                <button id="cancel_button" type="submit">
                        <KVP value={ btnText[0] } />
                </button> 
                <button id="submit_button" type="submit">
                        <KVP value={ btnText[1] } />
                </button> 
            </div>
        );
    }
}

```
