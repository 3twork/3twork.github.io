---
title: 基础用法
order: 0
---

给子元素展示红点

```vdt
import Badge from 'kpc/components/badge';
import Button from 'kpc/components/button';

<div>
    <Badge>Message</Badge>
    <Badge>
        <Button>Message</Button>
    </Badge>
</div>
```

```styl
.k-badge
    margin-right 30px
```

```html

<div class="k-badge">
	Message<sup class="k-text"></sup>
</div>
<div class="k-badge">
	<button class="k-btn" tabindex="0" type="button">
		<span>Message</span>
	</button>
	<sup class="k-text"></sup>
</div>

```