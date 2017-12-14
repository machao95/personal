## 头部逃费概况组件
#### Usage
定位到 components 目录下，运行：
```
npm --registry=http://<服务器IP:端口> install top-dodging
```
### Example：
```
# 所有效果
<t-top-dodging :data="eData" :edit="true" @edit="editCb"></t-top-dodging>
```
```
# 不可修改
<t-top-dodging :data="eData"></t-top-dodging>
```
![示例](C:\Users\Administrator\Desktop\top-dodging.png)

### Attributes

| 参数 | 说明       | 类型    | 可选值     | 默认值 |
|------|------------|---------|------------|--------|
| data | 绑定的数据 | Object  | --         | --     |
| edit | 是否可修改 | Boolean | true/false | false  |

### Events

| 名称 | 说明           | 回调参数     |
|------|----------------|--------------|
| edit | 金额修改时触发 | 修改的金额值 |

### 说明

data应包含以下字段:

| 字段名           | 说明                                              |
|------------------|---------------------------------------------------|
| escapeType       | 逃费类型，无此项时可不传，或传入undefined、null值 |
| plateNumber      | 车牌号码                                          |
| plateColor       | 车牌颜色                                          |
| judgeTime        | 系统判定时间                                      |
| escapeMoney      | 本次逃费金额                                      |
| escapeMoneyCount | 累加逃费金额                                      |
| escapeNumber     | 累加逃费次数                                      |


