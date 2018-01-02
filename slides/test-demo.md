
```
describe('should render stuff', () => {
        it('for PricePoint components', () => {
            wrapper = shallow(<FooterSummary footerSummaryInStore={ footerSummaryInitState } bookingTotal={ 23 } kvps={ kvps } { ...propsData } onSubmit={ f=>f } onCancel={ f=>f } updateLoadingState={ f=>f } />);
            expect(wrapper.find('PricePoint').exists()).toBe(true);
        });

        it('for page', () => {
            wrapper = render(<FooterSummary footerSummaryInStore={ footerSummaryInitState } bookingTotal={ 23 } kvps={ kvps } { ...propsData } onSubmit={ f=>f } onCancel={ f=>f } updateLoadingState={ f=>f } />);
            const desc = wrapper.find('.footer-summary__desc').text();
            const btnText = wrapper.find('.footer-summary__button').text();

            expect(wrapper.find('#submit_button').hasClass('is-loading')).toBe(false);
            expect(desc).toBe('No flights selected');
            expect(btnText).toBe('Choose flight and continue');   
        });

        it('for PricePoint components', () => {
            wrapper = shallow(<FooterSummary footerSummaryInStore={ footerSummaryInitState } bookingTotal={ 23 } kvps={ kvps } { ...propsData } onSubmit={ f=>f } onCancel={ f=>f } updateLoadingState={ f=>f } />);
            expect(wrapper.find('PricePoint').exists()).toBe(true);
        });

        it('for page', () => {
            wrapper = render(<FooterSummary footerSummaryInStore={ footerSummaryInitState } bookingTotal={ 23 } kvps={ kvps } { ...propsData } onSubmit={ f=>f } onCancel={ f=>f } updateLoadingState={ f=>f } />);
            const desc = wrapper.find('.footer-summary__desc').text();
            const btnText = wrapper.find('.footer-summary__button').text();

            expect(wrapper.find('#submit_button').hasClass('is-loading')).toBe(false);
            expect(desc).toBe('No flights selected');
            expect(btnText).toBe('Choose flight and continue');   
        });
        it('when click the page submit button', () => {
            const callback = sinon.spy();
            wrapper = mount(<FooterSummary footerSummaryInStore={ footerSummaryInitState } bookingTotal={ 23 } kvps={ kvps } { ...propsData } onSubmit={ (e) => callback(e) } onCancel={ f=>f } updateLoadingState={ f=>f } />);

            wrapper.find('#submit_button').simulate('click');

            expect(callback.called).toBe(true);
        });
});
```
