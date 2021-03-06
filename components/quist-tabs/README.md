# Tabs

> 选项卡切换组件。


## 安装

```
$ npm install quist-ui -D
```

## 引入
```ux
<import name="quist-tabs" src="@quist-ui/quist-tabs/index"></import>
<import name="quist-tabs-item" src="@quist-ui/quist-tabsItem/index"></import>
```

## 例子

#### 默认样式：

```ux
<quist-tabs>
  <quist-tabs-item @on-click="select(tabIdx)" for="(tabIdx, tabItem) in tabs" tab="{{tabItem}}">
  </quist-tabs-item>
</quist-tabs>
```

#### 自定义样式（水平分布）:

```ux
<quist-tabs border-color="#1890ff">
  <quist-tabs-item layout="center" line-width="{{3}}" f-size="{{36}}" active-color="#fac450" default-color="#333333" @on-click="selectb(tabIdx)" for="(tabIdx, tabItem) in tabsb" tab="{{tabItem}}">
  </quist-tabs-item>
</quist-tabs>
```


更详细代码可以参考 [quist-tabs demo](https://github.com/JDsecretFE/quist-ui/tree/master/src/Tabs/index.ux)

## API 

| 属性 | 说明 | 类型 | 默认值 |
|-------------|------------|:--------:|:-----:|
| border-color | 选项卡底部边框颜色 | `String` | #d9d9d9 |
| tab | 选项卡标题 | `String` | - |
| default-color | 选项卡文字颜色 | `String` | #666666 |
| active-color | 选中的颜色 | `String ` | #1890ff |
| line-width | 选中时border的宽度(如不想显示border，请不要传此值) | `Number` | 0 |
| f-size | 选项卡文字大小 | `Number ` | 32 |
| selected | 是否选中 | `Boolean ` | false |
| layout | 对齐方式，可选的值有 `left` `center` | `String ` | left |


## 更新日志

#### v1.0.8（2018-11-01)  
* 新增 `Tabs` 组件
