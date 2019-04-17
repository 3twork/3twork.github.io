---
title: 基础用法
order: 0
---

通过添加`to`属性，来展示超链接

> `to`属性支持`vue-router`或者`react-router` `push`方法参数用法

```vdt
import {Breadcrumb, BreadcrumbItem} from 'kpc/components/breadcrumb';

<Breadcrumb>
    <BreadcrumbItem to="#/">item 1</BreadcrumbItem>
    <BreadcrumbItem to="/components/breadcrumb/">item 2</BreadcrumbItem>
    <BreadcrumbItem>item 3</BreadcrumbItem>
</Breadcrumb>
```

```html
<div class="k-breadcrumb">
    <div class="k-item"><a class="k-item-link">item 1</a><span class="k-separator">></span>
    </div>
    <div class="k-item"><a class="k-item-link">item 2</a><span class="k-separator">></span>
    </div>
    <div class="k-item"><span class="k-item-link">item 3</span>
    </div>
</div>
```