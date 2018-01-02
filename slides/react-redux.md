##  react-redux

- Connect

```
import { connect } from 'react-redux'

class FooterSummary extends Component {
    render() {
        return (
            <div>......</div>
        )
    }
}

const mapStateToProps = state => {
    return {
        footerSummaryInStore: state.footerSummary
    };
};
const mapDispatchToProps = dispatch => {
    return {
        updateLoadingState: isShowLoading => dispatch(actions.updateLoadingState({ isShowLoading }))
    };
};
const FooterSummaryContainerComponent = connect(
  mapStateToProps,
  mapDispatchToProps
)(FooterSummary)
```


