## 头部逃费概况组件
#### Usage
定位到 components 目录下，运行：
```
npm --registry=http://<服务器IP:端口> install keyValue
```
### Example：
```
# 默认效果 空格分隔
<t-key-value label="label">value</t-key-value>
```
```
# 指定分隔符
<t-key-value label="label" separate="：">value</t-key-value>
```

```
# label的宽度和对齐方式
<t-key-value label="label" label-width="100px" label-align="left">value</t-key-value>
```

### Attributes

| 参数 | 说明       | 类型    | 可选值     | 默认值 |
|------|------------|---------|------------|--------|
| label | 绑定的数据 | Object  | --         | --     |
| label-width | label的宽度 | String | -- | 80px  |
| label-align | label的对齐方式 | String | center/left/right | right  |
| separate | label与value的分隔符 | String | -- | 空格  |
