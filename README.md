## 车牌组件
#### Usage
定位到 components 目录下，运行：
```
npm --registry=http://<服务器IP:端口> install plate
```
### Example：
车牌颜色小块+车牌号码
```
<t-plate width="14px" height="14px" plateNumber="桂A123456" plateColor="2"></t-plate>

```
车牌号码在颜色块内部
```
<t-plate width="200px" height="60px" plateNumber="桂A123456" plateColor="2" :inside="true"></t-plate>

```
无车牌号码
```
<t-plate width="20px" height="20px" plateColor="2"></t-plate>

```

### Attributes

| 参数 | 说明       | 类型    | 可选值     | 默认值 |
|------|------------|---------|------------|--------|
| plateColor | 车牌颜色代码 | String  | 1/2/3/4/5         | --     |
| plateNumber | 车牌号 | String | -- | --  |
| inside | 车牌号显示位置，true为内部，仅在传入车牌时有效 | Bollean | true/false | false  |
| width | 车牌块宽度 | String | -- | 0  |
| height | 车牌块高度 | String | -- | 0  |

### 说明

> 车牌颜色块都有1px的边框，设定width和height时请注意减去边框

