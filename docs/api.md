# photoClip API
---

## 选项

选项 | 类型 | 默认值 | 描述
--- | ---- | ------- | -----------
width | Int | `200` | 裁剪框宽
height | Int | `200` | 裁剪框高
fileMinSize | Int | `20` | 图片质量最小值(kb)
defaultImg | String |  `'图片路径'` | 初始图片路径（未完善）
file | dom | `null` | (必须) file按钮
ok | dom | `null` | (必须) 确定裁剪按钮
outputType | String |  `'jpg'` | 指定输出图片的类型，可选 "jpg" 和 "png" 两种种类型，默认为 "jpg"
strictSize | Boolean |  `false` | 是否严格按照截取区域宽高裁剪。默认为false，表示截取区域宽高仅用于约束宽高比例。如果设置为true，则表示截取出的图像宽高严格按照截取区域宽高输出。
customOutput | Boolean |  `false` | 自定义选择完毕输出，不执行内部填充函数
loadStart | Function|  `null` | 开始加载的回调函数。this指向 fileReader 对象，并将正在加载的 file 对象作为参数传入。
loadProgress | Function|  `null` | 加载中的回调,传入参数 加载百分比
loadComplete | Function|  `null` | 加载完成的回调函数。this指向图片对象，并将图片地址作为参数传入。
loadError | Function|  `null` | 加载失败的回调函数。this指向 fileReader 对象，并将错误事件的 event 对象作为参数传入。
clipFinish | Function|  `null` | 裁剪完成的回调函数。this指向图片对象，会将裁剪出的图像数据DataURL作为参数传入。
formatError | Function|  `null` | 图片格式错误
imgSizeMin | Function|  `null` | 图片质量小于设置范围时回调
