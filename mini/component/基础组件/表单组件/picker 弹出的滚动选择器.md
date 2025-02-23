# 简介

选择器包括一个或多个不同值的可滚动列表，每个值可以在视图的中心以较暗的文本形式显示。当用户正在编辑字段或点击菜单时，选择器通常会从屏幕底部弹起（iOS）或中间弹出（Android）。

## 使用说明

- picker 组件在 iOS 系统中从底部弹出，在 Android 系统中从中间弹出。
- 支持通过 [my.multiLevelSelect](https://opendocs.alipay.com/mini/api/multi-level-select)调用级联选择。
- 支持通过 [my.datePicker](https://opendocs.alipay.com/mini/api/ui-date) 打开日期选择列表。

## 扫码体验

![|127x157](https://gw.alipayobjects.com/zos/skylark-tools/public/files/6af93644fb19ed9be1d511fe208d4b20.png#align=left&display=inline&height=157&margin=%5Bobject%20Object%5D&originHeight=157&originWidth=127&status=done&style=none&width=127)

# 使用

## 在线示例

[小程序在线](https://opendocs.alipay.com/openbox/mini/opendocs/basic-component?view=preview&defaultPage=pages/picker/index&defaultOpenedFiles=pages/picker/index&theme=light)

## 属性说明

| **属性** | **类型** | **描述** |
| --- | --- | --- |
| title | String | 标题。 |
| range | String[] / Object[] | String[] 时表示可选择的字符串列表；Object[] 时需指定 range-key 表示可选择的字段。<br />**默认值：** [] |
| range-key | String | 当 `range` 为 Object[] 时，通过 range-key 来指定 Object 中 key 的值作为选择器显示内容。 |
| value | Number | 表示选择了 `range` 中的第几个（下标从 0 开始）。 |
| onChange | EventHandle | value 改变时触发，`event.detail = {value: value}`。 |
| disabled | Boolean | 是否禁用。<br />**默认值：** false |
