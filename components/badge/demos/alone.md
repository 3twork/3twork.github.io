---
title: 独立使用
order: 3
---

不给组件指定子元素，可以展示单独的徽标

```vdt
import Badge from 'kpc/components/badge';
import Button from 'kpc/components/button';

<div>
    <Badge />
    <Badge text="new" />
    <Badge text={{ 19 }} />
    <Badge text={{ 100 }} max={{ 99 }} />
</div>
```

```styl
.k-badge
    margin-right 30px
```

```html
<div class="k-badge k-alone"><sup class="k-text"></sup>
</div>
<div class="k-badge k-has-text k-alone"><sup class="k-text">new</sup>
</div>
<div class="k-badge k-has-text k-alone"><sup class="k-text">19</sup>
</div>
<div class="k-badge k-has-text k-alone"><sup class="k-text">99+</sup>
</div>
```