- Container component

```
class FooterSummary extends Component {
    render() {
        return (
            <div className="footer-summary" aria-label="Booking Summary">
                <div className="footer-summary__desc">
                    <KVP value={ showWarning ? warning : desc } /></span>
                </div>
                <div className="footer-summary__label">
                    <KVP value={ totalAmountLabel } />
                </div>
                <FooterSummaryButton footerSummaryType={ footerSummaryType } />
             </div>
            );
    }
}

const mapStateToProps = state => {
    return {
        footerSummaryInStore: state.footerSummary
    };
};
```

