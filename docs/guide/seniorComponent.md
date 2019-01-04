# 高级组件
接下来大部分组件的配置要略为复杂，它们除了宽高之外，还需要配置一些特殊的属性，
通过不同的配置以达到多变，富有冲击力的展示效果

::: tip
部分高级组件需要配置`坐标轴`，你可能需要先阅读坐标轴的相关配置项

[坐标轴](/axis/)
:::

## 基本属性
大部分高级组件可能会包涵一个或多个但不局限于如下几个基本属性，在使用它们之前，你应该对此有所了解

::: tip
`labelLine`及`colors`的配置较为简单且不随组件发生改变，文档中涉及它们的组件不再列举其配置
:::

## data
`data`是高级组件最为重要的属性，如果存在该属性，那么该属性一定是必须的。
它的值应当为一个对象，包涵该组件的数据及相关配置。
该项为空、空对象或必须属性不存在时，组件不渲染，自动显示loading效果

## labelLine
部分高级组件内置了标签组件，这些组件会将`labelLine`的值分发给内置的标签组件，用于生成底部标签。
该属性为选填属性，不配置该项属性将不渲染底部标签

:::tip
并非所有高级组件都支持该属性，但你可以在任何你希望的时候通过标签组件去实现该效果
:::

具体配置参见 [标签](/other/label-line) 组件

## colors
colors用于配置高级组件的全局配色，如果不配置该项则采用默认配色方案，该值必须为hex十六进制色数组，
你也可以更改默认配色方案，详情参见 [配置项](/config)
```js
colors: ['#123456', '#654321']
```

::: tip
data及labelLine内部分颜色属性均可使用colors关键字指向全局配色
:::