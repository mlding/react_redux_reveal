##  props

props are read-only

```
<PricePoint total={ bookingTotal } />

this.props.total
```

PropTypes

```
static propTypes = {
          descList: object.isRequired,
          btnText: oneOfType([string, array]),
          totalAmountLabel: string.isRequired,
          footerSummaryType: string,
          onSubmit: func.isRequired,
          bookingTotal: number.isRequired
}
```
