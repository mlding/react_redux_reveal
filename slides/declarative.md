##  declarative

```
class FooterSummary extends React.Component {
// ...
    render() {
        return (
            <div className="footer-summary">
                <h1>FooterSummary</h1>
                <PricePoint total={ bookingTotal } template={ template } />
            </div>
        );
    }
};
```

- React is an abstraction away from the DOM
- Render a component returns description of what the UI should look like
- Encourages you to think of your application and UI in terms of state, rather than UI manipulations
