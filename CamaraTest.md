# MTF
1.打开文件
2.选择MTF.jpg（路径不要出现中文）
3.选择测试区域(ROI)
4.设置选项
    设置坐标单位
    CA测试选项
    勾选想要的结果
    缓存空间要求大（勾选Close figure after save）
    存放路径
    文件名设置
5.结果读取
    锐度读取-一般看overshoot
    MTF-一般LW/PH单位结果为准
    MTF50-值为0.5时对应的空间频率
    MTF50P-值为曲线峰值的一般对应的空间频率
    Cycle/Pixel与LW/PH间的转换公式
    多个区域一起测试-Multi——ROI界面读取
    
    CA测试结果
    1.CA测试结果-CA的值越大RGB三根曲线的重合率越低-说明边缘色散约严重
    用SFRplus测试
    CA调试方法-加大边缘饱和度

# 色彩偏差、饱和度、白平衡
24色卡
D65、CWF、TL84、F/A五种光源
占据整体85%的范围

选择页面的color check选项
ROI选择方框范围在色块中心不要超过黑边
设置选项-噪声结果显示方式-色彩空间默认-噪声色块选择-设置想要的测试结果
得到色彩偏差结果-饱和度结果

白平衡测试结果

# 信噪比测试SNR
D65光源
XXX_summery.csv更方便

# Shading测试
亮度均匀性测试和色彩均匀性测试

选择Light Falloff Shading
测试选项一般不做改变
测试结果 
Lens shading Coners-Sides
Color shading-R/B值中心与四周最差值和平均值-Worst/Mean

# 灰阶stepchart/Dynamic Range 
选项也可测试其他 但是一般不会用
结果-Gamma-查看曲线是非递增分布-有些要求不能翘
亮度差值大于8就能区分

# 曝光偏差测试
直接使用色差测试的结果
ExposureError测试结果

# Gamma测试
直接使用色差测试的结果

# Density Range测试
Pixel noise

# 畸变测试
结果-SMIA TV Distortion

# CA测试
SFRplus auto
结果 CA （area）

# FOV视场角测试
测试结果-FoV 计算