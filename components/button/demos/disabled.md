---
title: 禁用状态
order: 5
---

添加`disabled`属性，可以禁用按钮

```vdt
import Button from 'kpc/components/button';

<div>
    <Button disabled>disabled</Button>
    <Button disabled type="none">disabled text</Button>
    <Button disabled icon circle><i class="k-icon ion-ios-search"></i></Button>
</div>
```

```jsx
import React from 'react';
import Button from 'kpc/components/button';

export default class extends React.Component {
    render() {
        return (
            <div>
                <Button disabled>disabled</Button>
                <Button disabled type="none">disabled text</Button>
                <Button disabled icon circle><i className="k-icon ion-ios-search"></i></Button>
            </div>
        )
    }
}
```
```html
<div>
    <button class="k-btn k-disabled" tabindex="-1" type="button"><span>disabled</span>
    </button>
    <button class="k-btn k-none k-disabled" tabindex="-1" type="button"><span>disabled text</span>
    </button>
    <button class="k-btn k-btn-icon k-circle k-disabled" tabindex="-1" type="button"><i class="k-icon ion-ios-search"></i>
    </button>
</div>
```