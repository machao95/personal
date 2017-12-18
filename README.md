## 车辆司机信息 组件
#### Usage
定位到 components 目录下，运行：
```
npm --registry=http://<服务器IP:端口> install carDriverInfo
```
### Example：
默认
```
<t-car-driver-info :data="cardriverData" ></t-car-driver-info>

cardriverData: {
    carData: {
      carPic: 'http://www.sinaimg.cn/dy/slidenews/1_img/2017_50/88490_1557806_381226.jpg',
      plateNumber: '桂A123456',
      plateColor: '0',
      alexNum: 4,
      tyreNum: 8,
      carType: '货5',
      carWeight: '25(吨)',
      loadWeight: '40(吨)'
    },
    driverData: {
      driverPic: 'http://www.people.com.cn/mediafile/pic/20160226/26/1191985824992231422.jpg',
      driverName: '王百万',
      sex: '男',
      drivingType: 'B2',
      licenseDate: '2018-09-09',
      licenseNumber: '423847293847509384',
      birth: '1983-1-5',
      idNumber: '45xxxxxxxxxxxxxxxx',
      address: '广西壮族自治区南宁市高新区中盟科技园'
    }
  }

```
指定宽度
```
<t-car-driver-info :data="cardriverData" width=750px></t-car-driver-info>

```

### Attributes

| 参数 | 说明       | 类型    | 可选值     | 默认值 |
|------|------------|---------|------------|--------|
| data | 车辆和司机信息 | Object  | --        | --     |
| width | 宽度 | String | -- | --  |

### 说明

data.carData 车辆信息字段:

| 字段名           | 说明                                              |
|------------------|---------------------------------------------------|
| carPic       | 车身图片 |
| plateNumber      | 车牌号码                                          |
| plateColor       | 车牌颜色                                          |
| alexNum        | 轴数                                      |
| tyreNum      | 轮胎数                                      |
| carType | 车辆类型                                      |
| carWeight     | 车重                                      |
| loadWeight     | 核载                                      |

 data.driverData 司机信息字段:
  
  | 字段名           | 说明                                              |
  |------------------|---------------------------------------------------|
  | driverPic       | 司机图片 |
  | driverName      | 司机姓名                                          |
  | sex       | 性别                                          |
  | drivingType        | 准驾车型                                      |
  | licenseDate      | 驾驶证有效期                                      |
  | licenseNumber | 驾驶证号码                                      |
  | birth     | 出生日期                                     |
  | idNumber     | 身份证号                                      |
  | address     | 地址                                      |

