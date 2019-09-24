### 结构
程序入口: ./example/run_\<dataset>_slam.cc  
配置文件: ./example/\<dataset>/*.yaml

### 流程
1. main(): 解析参数，调用mono_tracking()
2. mono_tracking(): 1. 处理不同数据 2. 实例化SLAM系统 3. 送入数据，运行SLAM 4. 控制结果输出，统计时间

SLAM类
负责初始化和控制 tracking, mapping, global_optimizer 的流程，不执行具体的工作 
