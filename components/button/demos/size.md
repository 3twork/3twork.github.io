---
title: 按钮尺寸
order: 4
---

通过`size`属性可以指定按钮的尺寸：`large`, `default`,`small`, `mini`。

```vdt
import Button from 'kpc/components/button';
import Icon from 'kpc/components/icon';

<div>
    <Button size="large">large</Button>
    <Button>default</Button>
    <Button size="small">small</Button>
    <Button size="mini">mini</Button>
    <br /><br />
    <Button icon circle size="large"><Icon class="ion-ios-search" size="large" /></Button>
    <Button icon circle><Icon class="ion-ios-search" /></Button>
    <Button icon circle size="small"><Icon class="ion-ios-search" size="small" /></Button>
    <Button icon circle size="mini"><Icon class="ion-ios-search" size="mini" /></Button>
</div>
```

```styl
.k-btn
    margin-right 20px
```

```jsx
import React from 'react';
import Button from 'kpc/components/button';

export default class extends React.Component {
    render() {
        return (
            <div>
                <Button size="large">large</Button>
                <Button>default</Button>
                <Button size="small">small</Button>
                <Button size="mini">mini</Button>
                <br /><br />
                <Button icon circle size="large"><i className="k-icon ion-ios-search"></i></Button>
                <Button icon circle><i className="k-icon ion-ios-search"></i></Button>
                <Button icon circle size="small"><i className="k-icon ion-ios-search"></i></Button>
                <Button icon circle size="mini"><i className="k-icon ion-ios-search"></i></Button>
            </div>
        )
    }
}
```
```html
<div>
    <button class="k-btn k-large" tabindex="0" type="button"><span>large</span>
    </button>
    <button class="k-btn" tabindex="0" type="button"><span>default</span>
    </button>
    <button class="k-btn k-small" tabindex="0" type="button"><span>small</span>
    </button>
    <button class="k-btn k-mini" tabindex="0" type="button"><span>mini</span>
    </button>
    <br>
    <br>
    <button class="k-btn k-btn-icon k-large k-circle" tabindex="0" type="button"><i class="k-icon ion-ios-search k-large"></i>
    </button>
    <button class="k-btn k-btn-icon k-circle" tabindex="0" type="button"><i class="k-icon ion-ios-search"></i>
    </button>
    <button class="k-btn k-btn-icon k-small k-circle" tabindex="0" type="button"><i class="k-icon ion-ios-search k-small"></i>
    </button>
    <button class="k-btn k-btn-icon k-mini k-circle" tabindex="0" type="button"><i class="k-icon ion-ios-search k-mini"></i>
    </button>
</div>
```