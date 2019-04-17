---
title: 按钮组
order: 1
---

将`Button`作为`ButtonGroup`的子元素，可以展示按钮组。给`ButtonGroup`添加`vertical`属性，
可以是按钮组纵向排列。给`ButtonGroup`添加`checkType`属性，可以使按钮组拥有单选或复选能力。

```vdt
import {Button, ButtonGroup} from 'kpc/components/button';

<div>
    <ButtonGroup>
        <Button>开机</Button>
        <Button>关机</Button>
        <Button>重启</Button>
    </ButtonGroup>
    <ButtonGroup>
        <Button type="primary">开机</Button>
        <Button type="primary">关机</Button>
        <Button type="primary">重启</Button>
    </ButtonGroup>
    <ButtonGroup>
        <Button type="primary">
            <i class="k-icon ion-ios-arrow-left"></i>上一页
        </Button>
        <Button type="primary">
            下一页<i class="k-icon ion-ios-arrow-right"></i>
        </Button>
    </ButtonGroup>
    <br /><br />
    <p>纵向按钮组</p>
    <ButtonGroup vertical>
        <Button type="primary">开机</Button>
        <Button type="primary">关机</Button>
        <Button type="primary">重启</Button>
    </ButtonGroup>
    <br /><br />
    <p>radio按钮组</p>
    <ButtonGroup checkType="radio" v-model="city">
        <Button value="beijing">北京</Button>
        <Button value="shanghai" ref="__radioShanghai">上海</Button>
        <Button value="guangzhou">广州</Button>
        <Button value="shenzhen">深圳</Button>
    </ButtonGroup>
    <p>checkbox按钮组</p>
    <ButtonGroup checkType="checkbox" v-model="cities">
        <Button value="beijing" size="small">北京</Button>
        <Button value="shanghai" size="small" ref="__checkboxShanghai">上海</Button>
        <Button value="guangzhou" size="small">广州</Button>
        <Button value="shenzhen" size="small">深圳</Button>
    </ButtonGroup>
</div>
```

```styl
.k-btns
    margin-right 20px
```

```js
export default class extends Intact {
    @Intact.template()
    static template = template;

    defaults() {
        return {
            city: 'beijing',
            cities: [],
        };
    }
}
```

```html
<div>
    <div class="k-btns">
        <button class="k-btn" tabindex="0" type="button"><span>开机</span>
        </button>
        <button class="k-btn" tabindex="0" type="button"><span>关机</span>
        </button>
        <button class="k-btn" tabindex="0" type="button"><span>重启</span>
        </button>
    </div>
    <div class="k-btns">
        <button class="k-btn k-primary" tabindex="0" type="button"><span>开机</span>
        </button>
        <button class="k-btn k-primary" tabindex="0" type="button"><span>关机</span>
        </button>
        <button class="k-btn k-primary" tabindex="0" type="button"><span>重启</span>
        </button>
    </div>
    <div class="k-btns">
        <button class="k-btn k-primary k-icon-left" tabindex="0" type="button"><i class="k-icon ion-ios-arrow-left"></i><span>上一页
        </span>
        </button>
        <button class="k-btn k-primary k-icon-right" tabindex="0" type="button"><span>
            下一页</span><i class="k-icon ion-ios-arrow-right"></i>
        </button>
    </div>
    <br>
    <br>
    <p>纵向按钮组</p>
    <div class="k-btns k-vertical">
        <button class="k-btn k-primary" tabindex="0" type="button"><span>开机</span>
        </button>
        <button class="k-btn k-primary" tabindex="0" type="button"><span>关机</span>
        </button>
        <button class="k-btn k-primary" tabindex="0" type="button"><span>重启</span>
        </button>
    </div>
    <br>
    <br>
    <p>radio按钮组</p>
    <div class="k-btns">
        <button class="k-btn k-active" tabindex="0" type="button"><span>北京</span>
            <input type="radio" tabindex="-1">
        </button>
        <button class="k-btn" tabindex="0" type="button"><span>上海</span>
            <input type="radio" tabindex="-1">
        </button>
        <button class="k-btn" tabindex="0" type="button"><span>广州</span>
            <input type="radio" tabindex="-1">
        </button>
        <button class="k-btn" tabindex="0" type="button"><span>深圳</span>
            <input type="radio" tabindex="-1">
        </button>
    </div>
    <p>checkbox按钮组</p>
    <div class="k-btns">
        <button class="k-btn k-small" tabindex="0" type="button"><span>北京</span>
            <input type="checkbox" tabindex="-1">
        </button>
        <button class="k-btn k-small" tabindex="0" type="button"><span>上海</span>
            <input type="checkbox" tabindex="-1">
        </button>
        <button class="k-btn k-small" tabindex="0" type="button"><span>广州</span>
            <input type="checkbox" tabindex="-1">
        </button>
        <button class="k-btn k-small" tabindex="0" type="button"><span>深圳</span>
            <input type="checkbox" tabindex="-1">
        </button>
    </div>
</div>
```