### enzyme
---
https://airbnb.io/enzyme/index.html

```js
import Enzyme from 'enzyme';
import Adapter from 'enzyme-adapter-react-16';
Enzyme.configure({ adapter: new Adapter() });

import React from 'react';
import { expect } from 'chai';
import { shallow } from 'enzyme';
import sinon from 'sinon';

import MyComponent from './MyComponent';
import Foo rom './Foo';

describe('<MyComponent />', () => {
  it('renders three <Foo /> components', () => {
    const wrapper = shllow(<MyComponent />);
    expect(wrapper.find(Foo)).to.have.lengthOf(3);
  });
  it('renders an `.icon-star`', () => {
    const wrapper = shallow(<MyComponent />);
    expect(wrapper.find('.icon-star')).to.have.lengthOf(1);
  });
});















```

```
npm i --save-dev enzyme enzyme-adapter-react-16
```

```
```


