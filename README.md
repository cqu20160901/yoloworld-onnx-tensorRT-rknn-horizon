# yoloworld-onnx-tensorRT-rknn-horizon

yolovworld 目标检测部署版本，便于移植不同平台（onnx、tensorRT、rknn、Horizon），全网部署最简单、速度最快的部署方式，后处理为C++部署而写，python 测试后处理意义不大。

导出onnx参考[【yolo_world 瑞芯微芯片rknn部署、地平线芯片Horizon部署、TensorRT部署】](https://blog.csdn.net/zhangqian_1/article/details/138530486)。

# 文件夹结构说明

yoloworld_onnx：onnx模型、测试图像、测试结果、测试demo脚本

yoloworld_TensorRT：TensorRT版本模型、测试图像、测试结果、测试demo脚本、onnx模型、onnx2tensorRT脚本(tensorRT-7.2.3.4)

yoloworld_rknn：rknn模型、测试（量化）图像、测试结果、onnx2rknn转换测试脚本（rknn_toolkit2-2.0.0）（尝试过 rknn_toolkit2-1.3、1.6 模型转化可以成功，但实际上板子运行模型时会报错）

yoloworld_horizon：地平线模型、测试（量化）图像、测试结果、转换测试脚本、测试量化后onnx模型脚本

# 测试结果

![image](https://github.com/cqu20160901/yoloworld-onnx-tensorRT-rknn-horizon/blob/main/yoloworld_onnx/test_onnx_result.jpg)

# 在 rk3588板子上时耗

rknn 板端参考[【yolo world 目标检测 rknn 的C++部署】](https://blog.csdn.net/zhangqian_1/article/details/138530486)

![rk3588时耗](https://github.com/cqu20160901/yoloworld-onnx-tensorRT-rknn-horizon/assets/22290931/3c5f08a7-a395-4bca-81a6-42070f0bf942)

# TensorRT C++ 时耗参考

TensorRT部署参考[【yolo world tensorRT 的 C++ 部署】](https://blog.csdn.net/zhangqian_1/article/details/138532260)

![image](https://github.com/cqu20160901/yoloworld-onnx-tensorRT-rknn-horizon/assets/22290931/1e55e485-1ad4-4fb4-84e8-021ee0465da3)



