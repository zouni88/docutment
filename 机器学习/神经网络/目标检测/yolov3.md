### 准备数据集
labelImg 数据标注工具
![labelImg](res/labelImg.png)
### 模型结构 如下图：
![yolov3](res/yolov3.png)
网络输入 416x416 经过一系列卷积层之后分成了三个分支，最终得到三个输出：[13,13,c],[26,26,c],[52,52,c] **c是通道数**  
feature map 越大，感受野越小，适合预测小目标，  
[13,13] feature map适合预测大目标

# 数据 target转换
同等变换，[512,512,3] => [13,13,5]  
意思是 512x512的图片上的真是框 映射到13x13的 feature map上，缩放32倍  
每个图片上 最多有 gtbox_max个框，每个box 有5个值[x,y,w,h,confidence]  
因为网络输出是中心点坐标，所以x,y得转换成中心点坐标
