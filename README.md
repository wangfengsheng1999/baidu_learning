# baidu_learning

There are several modules in this repo!

## tvm_learning
about tvm study!

## pybind_learning

just study about pybind 

## compiler_learning directory

In this directory, i write the traditional compiler!

The tool is a important compiler project for the translation from paddle code to the torch code

the compiler is implemented based the based on Flex/Bison.

## profile_learning
perf

### paddlebenchmark
test the backbone network on GPU
```bash
sh run.sh
-------------  Configuration Arguments -------------
                 amp_mode : O2
               batch_size : 128
              data_format : NCHW
                dy2static : True
           input_channels : 3
                    model : ResNet50
                run_steps : 100
           static_op_fuse : False
                  use_amp : True
                use_scale : False
             warmup_steps : 30
----------------------------------------------------
IPS: 1879.9288446672845 img/s
参数说明：

amp_mode, amp模式，默认是 O2，可选 O1
batch_size, 批次大小，默认 128
data_format, 数据格式，默认 "NCHW", 可选 "NHWC"
dy2static，是否动转静训练，默认不使用
input_channels, 输入通道数，默认是 3，可选 4, 只支持 ResNet 系列
run_steps，训练 benchmark 的总 step 数量，默认 100
static_op_fuse，是否使用静态图下的 op fuse 功能，默认不使用，因为部分模型使用后性能会下降
use_amp，是否使用 amp 训练，默认不使用
use_scale，使用 amp 训练时，是否使用 scale，默认不使用
warmup_steps，训练 benchmark 的 warmup step 数量，默认 30
需要其他配置时，修改 run.sh 中的参数即可。

```

## AIFramework_learning
study framework_learning