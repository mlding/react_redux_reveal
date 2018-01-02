##  state

- internal data with state
- setState(nextState, callback) -- shallow merge

```
class Message extends React.component({
  state = { message: this.props.message }
  _messageChange = (e) {
    this.setState({ message: e.target.value });
  }
  render() {
    return (
      <div>
        <span>Message: {this.state.message}</span>
        <br />
        Message: 
        <input type="text" value={this.state.message} onChange={this._messageChange} />
      </div>
    );
  }
});
ReactDOM.render(<Message message="Hello World!!" />, document.querySelector("main"));

```

