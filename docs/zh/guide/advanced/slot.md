# 自定义页签模板

通过 RouterTab 组件的默认作用域插槽，我们可以自定义页签显示的内容

插槽的作用域提供页签项信息 `tab` 供模板使用，包括以下属性或方法

| 属性 | 类型 | 说明 |
| --- | --- | --- |
| base | Component | RouterTab 实例 |
| data | Object | 页签数据 |
| id | String | 页签 ID |
| title | String | 标题 |
| tips | String | 提示 |
| icon | String | 图标 |
| tabClass | String | 页签 class |
| closable | Boolean | 是否可关闭 |
| index | Number | 页签索引 |
| close | Function | 页签关闭方法 |

<doc-links demo="/slot/"></doc-links>

**示例：**

<<< @/src/components/frames/Slot.vue{3,4,5,6,7,8}
