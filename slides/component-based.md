##  component-based

```
class FooterSummary extends React.Component {
// ...
    render() {
        return (
            <div className="footer-summary">
                <DescList />
                <PricePoint total={ bookingTotal } template={ template } />
                <Buttons />
            </div>
        );
    }
};
```

Build each component that manage their own state, then compose them to make complex UIs
