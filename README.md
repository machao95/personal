## 判定图片 组件
#### Usage
定位到 components 目录下，运行：
```
npm --registry=http://<服务器IP:端口> install judgeImg
```
### Example：
默认效果
```
<t-judgeimg :data="imgsData"></t-judgeimg>
imgsData = [{
                credible: '0.5',
                plateNumber: '桂A123456',
                carInPic: 'http://www.sinaimg.cn/dy/slidenews/1_img/2017_50/88490_1557806_381226.jpg',
                carOutPic: 'http://www.sinaimg.cn/dy/slidenews/1_img/2017_50/88490_1557806_381226.jpg',
                carInAdress: '入口收费站',
                carOutAdress: '出口收费站',
                carInTime: '2017-09-23 12:00:00',
                carOutTime: '2017-09-23 19:00:00'
              }]
```
指定宽度
```
<t-judgeimg :data="imgsData" wdith="500px"></t-judgeimg>
```
疑似同伙
```
<t-judgeimg :data="imgsData" @judge="judgeEvent"></t-judgeimg>
```


### Attributes

| 参数 | 说明       | 类型    | 可选值     | 默认值 |
|------|------------|---------|------------|--------|
| data | 绑定的数据，长度为1时是本车图片 | Array  | --         | --     |
| width | 宽度 | String | -- | --  |
| autoplay | 疑似同伙时，是否自动播放 | Boolena | true/false | false  |

### Events

| 名称 | 说明           | 回调参数     |
|------|----------------|--------------|
| judge | 判定为同伙 | 当前条同伙数据 |

### 说明

data的类型必须为一个数组，当data.length == 1 时，为本车图片，否则为疑似同伙 
data每一项应包含以下字段:

| 字段名           | 说明                                              |
|------------------|---------------------------------------------------|
| credible       | 相似度 |
| plateNumber      | 车牌号码                                          |
| carInAdress       | 车辆进入地点                                          |
| carInTime        | 车辆进入时间                                      |
| carInPic      | 入口车身图                                      |
| carOutAdress       | 车辆出去地点                                          |
| carOutTime        | 车辆出去时间                                      |
| carOutPic      | 出口车身图                                      |

