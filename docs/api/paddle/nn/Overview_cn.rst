.. _cn_overview_nn:

paddle.nn
---------------------

paddle.nn 目录下包含飞桨框架支持的神经网络层和相关函数的相关API。具体如下：

-  :ref:`容器相关 <about_container>`
-  :ref:`卷积层 <convolution_layers>`
-  :ref:`Pooling层 <pooling_layers>`
-  :ref:`Padding层 <padding_layers>`
-  :ref:`激活层 <activation_layers>`
-  :ref:`Normalization层 <normalization_layers>`
-  :ref:`循环神经网络层 <RNN_layers>`
-  :ref:`Transformer相关 <Transformer>`
-  :ref:`线性层 <linear_layers>`
-  :ref:`Dropout层 <dropout_layers>`
-  :ref:`Embedding层 <embedding_layers>`
-  :ref:`Loss层 <loss_layers>`
-  :ref:`Vision层 <vision_layers>`
-  :ref:`Clip相关 <about_clip>`
-  :ref:`公共层 <common_layers>`
-  :ref:`卷积相关函数 <convolution_functional>`
-  :ref:`Pooling相关函数 <pooling_functional>`
-  :ref:`Padding相关函数 <padding_functional>`
-  :ref:`激活函数 <activation_functional>`
-  :ref:`Normalization方法 <normalization_functional>`
-  :ref:`线性处理相关函数 <linear_functional>`
-  :ref:`Dropout方法 <dropout_functional>`
-  :ref:`Embedding相关函数 <embedding_functional>`
-  :ref:`损失函数 <loss_functional>`
-  :ref:`公用方法 <common_functional>`
-  :ref:`初始化相关 <about_initializer>`




.. _about_container:

容器相关
::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.Layer <cn_api_fluid_dygraph_Layer>` ", "基于OOD实现的动态图Layer"
    " :ref:`paddle.nn.LayerList <cn_api_fluid_dygraph_LayerList>` ", "用于保存子层列表"
    " :ref:`paddle.nn.ParameterList <cn_api_fluid_dygraph_ParameterList>` ", "参数列表容器"
    " :ref:`paddle.nn.Sequential <cn_api_fluid_dygraph_Sequential>` ", "顺序容器；子Layer将按构造函数参数的顺序添加到此容器中"
    " :ref:`paddle.nn.LayerDict <cn_api_nn_LayerDict>` ", "保存子层到有序字典中，它包含的子层将被正确地注册和添加"

.. _convolution_layers:

卷积层
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    


    " :ref:`paddle.nn.Conv1D <cn_api_paddle_nn_Conv1D>` ", "一维卷积层"
    " :ref:`paddle.nn.Conv1DTranspose <cn_api_paddle_nn_Conv1DTranspose>` ", "一维转置卷积层"
    " :ref:`paddle.nn.Conv2D <cn_api_paddle_nn_Conv2D>` ", "二维卷积层"
    " :ref:`paddle.nn.Conv2DTranspose <cn_api_paddle_nn_Conv2DTranspose>` ", "二维转置卷积层"
    " :ref:`paddle.nn.Conv3D <cn_api_paddle_nn_Conv3D>` ", "三维卷积层"
    " :ref:`paddle.nn.Conv3DTranspose <cn_api_paddle_nn_Conv3DTranspose>` ", "三维转置卷积层"
    
.. _pooling_layers:

pooling层
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.AdaptiveAvgPool1D <cn_api_nn_AdaptiveAvgPool1D>` ", "一维自适应平均池化层"
    " :ref:`paddle.nn.AdaptiveAvgPool2D <cn_api_nn_AdaptiveAvgPool2D>` ", "二维自适应平均池化层"
    " :ref:`paddle.nn.AdaptiveAvgPool3D <cn_api_nn_AdaptiveAvgPool3D>` ", "三维自适应平均池化层"
    " :ref:`paddle.nn.AdaptiveMaxPool1D <cn_api_nn_AdaptiveMaxPool1D>` ", "一维自适应最大池化层"
    " :ref:`paddle.nn.AdaptiveMaxPool2D <cn_api_nn_AdaptiveMaxPool2D>` ", "二维自适应最大池化层"
    " :ref:`paddle.nn.AdaptiveMaxPool3D <cn_api_nn_AdaptiveMaxPool3D>` ", "三维自适应最大池化层"
    " :ref:`paddle.nn.AvgPool1D <cn_api_nn_AvgPool1D>` ", "一维平均池化层"
    " :ref:`paddle.nn.AvgPool2D <cn_api_nn_AvgPool2D>` ", "二维平均池化层"
    " :ref:`paddle.nn.AvgPool3D <cn_api_nn_AvgPool3D>` ", "三维平均池化层"
    " :ref:`paddle.nn.MaxPool1D <cn_api_nn_MaxPool1D>` ", "一维最大池化层"
    " :ref:`paddle.nn.MaxPool2D <cn_api_nn_MaxPool2D>` ", "二维最大池化层"
    " :ref:`paddle.nn.MaxPool3D <cn_api_nn_MaxPool3D>` ", "三维最大池化层"
    " :ref:`paddle.nn.MaxUnPool2D <cn_api_nn_MaxUnPool2D>` ", "二维最大反池化层"
    
.. _padding_layers:

Padding层
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.Pad1D <cn_api_nn_Pad1D>` ", "一维填充层"
    " :ref:`paddle.nn.Pad2D <cn_api_nn_Pad2D>` ", "二维填充层"
    " :ref:`paddle.nn.Pad3D <cn_api_nn_Pad3D>` ", "三维填充层"
    " :ref:`paddle.nn.ZeroPad2D <cn_api_nn_ZeroPad2D>` ", "二维零填充层"
    
.. _activation_layers:

激活层
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.CELU <cn_api_nn_CELU>` ", "CELU激活层"
    " :ref:`paddle.nn.ELU <cn_api_nn_ELU>` ", "ELU激活层"
    " :ref:`paddle.nn.GELU <cn_api_nn_GELU>` ", "GELU激活层"
    " :ref:`paddle.nn.Hardshrink <cn_api_nn_Hardshrink>` ", "Hardshrink激活层"
    " :ref:`paddle.nn.Hardsigmoid <cn_api_nn_Hardsigmoid>` ", "Hardsigmoid激活层"
    " :ref:`paddle.nn.Hardswish <cn_api_nn_Hardswish>` ", "Hardswish激活层"
    " :ref:`paddle.nn.Hardtanh <cn_api_nn_Hardtanh>` ", "Hardtanh激活层"
    " :ref:`paddle.nn.LeakyReLU <cn_api_nn_LeakyReLU>` ", "LeakyReLU 激活层"
    " :ref:`paddle.nn.LogSigmoid <cn_api_nn_LogSigmoid>` ", "LogSigmoid激活层"
    " :ref:`paddle.nn.LogSoftmax <cn_api_nn_LogSoftmax>` ", "LogSoftmax激活层"
    " :ref:`paddle.nn.Maxout <cn_api_nn_Maxout>` ", "Maxout激活层"
    " :ref:`paddle.nn.PReLU <cn_api_nn_PReLU>` ", "PReLU激活层"
    " :ref:`paddle.nn.ReLU <cn_api_nn_ReLU>` ", "ReLU激活层"
    " :ref:`paddle.nn.ReLU6 <cn_api_nn_ReLU6>` ", "ReLU6激活层"
    " :ref:`paddle.nn.SELU <cn_api_nn_SELU>` ", "SELU激活层"
    " :ref:`paddle.nn.Sigmoid <cn_api_nn_layer_Sigmoid>` ", "Sigmoid激活层"
    " :ref:`paddle.nn.Silu <cn_api_nn_Silu>` ", "Silu激活层"
    " :ref:`paddle.nn.Softmax <cn_api_nn_Softmax>` ", "Softmax激活层"
    " :ref:`paddle.nn.Softplus <cn_api_nn_Softplus>` ", "Softplus激活层"
    " :ref:`paddle.nn.Softshrink <cn_api_nn_Softshrink>` ", "Softshrink激活层"
    " :ref:`paddle.nn.Softsign <cn_api_nn_Softsign>` ", "Softsign激活层"
    " :ref:`paddle.nn.Swish <cn_api_nn_Swish>` ", "Swish激活层"
    " :ref:`paddle.nn.Tanh <cn_api_nn_Tanh>` ", "Tanh激活层"
    " :ref:`paddle.nn.Tanhshrink <cn_api_nn_Tanhshrink>` ", "Tanhshrink激活层"
    " :ref:`paddle.nn.ThresholdedReLU <cn_api_nn_ThresholdedReLU>` ", "Thresholded ReLU激活层"
    
.. _normalization_layers:

Normalization层
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.BatchNorm <cn_api_fluid_dygraph_BatchNorm>` ", "Batch Normalization层"
    " :ref:`paddle.nn.BatchNorm1D <cn_api_nn_BatchNorm1D>` ", "一维Batch Normalization层"
    " :ref:`paddle.nn.BatchNorm2D <cn_api_nn_BatchNorm2D>` ", "二维Batch Normalization层"
    " :ref:`paddle.nn.BatchNorm3D <cn_api_nn_BatchNorm3D>` ", "三维Batch Normalization层"
    " :ref:`paddle.nn.GroupNorm <cn_api_nn_GroupNorm>` ", "Group Normalization层"
    " :ref:`paddle.nn.InstanceNorm1D <cn_api_nn_InstanceNorm1D>` ", "一维Instance Normalization层"
    " :ref:`paddle.nn.InstanceNorm2D <cn_api_nn_cn_InstanceNorm2D>` ", "二维Instance Normalization层"
    " :ref:`paddle.nn.InstanceNorm3D <cn_api_nn_cn_InstanceNorm3D>` ", "三维Instance Normalization层"
    " :ref:`paddle.nn.LayerNorm <cn_api_nn_LayerNorm>` ", "用于保存Normalization层列表"
    " :ref:`paddle.nn.LocalResponseNorm <cn_api_nn_LocalResponseNorm>` ", "Local Response Normalization层"
    " :ref:`paddle.nn.SpectralNorm <cn_api_fluid_dygraph_SpectralNorm>` ", "Spectral Normalization层"
    " :ref:`paddle.nn.SyncBatchNorm <cn_api_nn_SyncBatchNorm>` ", "Synchronized Batch Normalization层"
    
.. _RNN_layers:

循环神经网络层
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.BiRNN <cn_api_paddle_nn_layer_rnn_BiRNN>` ", "双向循环神经网络"
    " :ref:`paddle.nn.GRU <cn_api_paddle_nn_layer_rnn_GRU>` ", "门控循环单元网络"
    " :ref:`paddle.nn.GRUCell <cn_api_paddle_nn_layer_rnn_GRUCell>` ", "门控循环单元"
    " :ref:`paddle.nn.LSTM <cn_api_paddle_nn_layer_rnn_LSTM>` ", "长短期记忆网络"
    " :ref:`paddle.nn.LSTMCell <cn_api_paddle_nn_layer_rnn_LSTMCell>` ", "长短期记忆网络单元"
    " :ref:`paddle.nn.RNN <cn_api_paddle_nn_layer_rnn_RNN>` ", "循环神经网络"
    " :ref:`paddle.nn.RNNCellBase <cn_api_paddle_nn_layer_rnn_RNNCellBase>` ", "循环神经网络单元基类"
    " :ref:`paddle.nn.SimpleRNN <cn_api_paddle_nn_layer_rnn_SimpleRNN>` ", "简单循环神经网络"
    " :ref:`paddle.nn.SimpleRNNCell <cn_api_paddle_nn_layer_rnn_SimpleRNNCell>` ", "简单循环神经网络单元"
   
.. _Transformer:

Transformer相关
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.MultiHeadAttention <cn_api_nn_MultiHeadAttention>` ", "多头注意力机制"
    " :ref:`paddle.nn.Transformer <cn_api_nn_Transformer>` ", "Transformer模型"
    " :ref:`paddle.nn.TransformerDecoder <cn_api_nn_TransformerDecoder>` ", "Transformer解码器"
    " :ref:`paddle.nn.TransformerDecoderLayer <cn_api_nn_TransformerDecoderLayer>` ", "Transformer解码器层"
    " :ref:`paddle.nn.TransformerEncoder <cn_api_nn_TransformerEncoder>` ", "Transformer编码器"
    " :ref:`paddle.nn.TransformerEncoderLayer <cn_api_nn_TransformerEncoderLayer>` ", "Transformer编码器层"
    
.. _linear_layers:

线性层
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.Bilinear <cn_api_nn_Bilinear>` ", "对两个输入执行双线性张量积"
    " :ref:`paddle.nn.Linear <cn_api_paddle_nn_layer_common_Linear>` ", "线性变换层"
    
.. _dropout_layers:

Dropout层
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.AlphaDropout <cn_api_nn_AlphaDropout>` ", "具有自归一化性质的dropout"
    " :ref:`paddle.nn.Dropout <cn_api_nn_Dropout>` ", "Dropout"
    " :ref:`paddle.nn.Dropout2D <cn_api_nn_Dropout2D>` ", "一维Dropout"
    " :ref:`paddle.nn.Dropout3D <cn_api_nn_Dropout3D>` ", "二维Dropout"
    
.. _embedding_layers:

Embedding层
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.Embedding <cn_api_nn_Embedding>` ", "嵌入层(Embedding Layer)"
    
.. _loss_layers:

Loss层
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.BCELoss <cn_api_paddle_nn_BCELoss>` ", "BCELoss层"
    " :ref:`paddle.nn.BCEWithLogitsLoss <cn_api_paddle_nn_BCEWithLogitsLoss>` ", "BCEWithLogitsLoss层"
    " :ref:`paddle.nn.CrossEntropyLoss <cn_api_nn_loss_CrossEntropyLoss>` ", "交叉熵损失层"
    " :ref:`paddle.nn.CTCLoss <cn_api_paddle_nn_CTCLoss>` ", "CTCLoss层"
    " :ref:`paddle.nn.HSigmoidLoss <cn_api_paddle_nn_HSigmoidLoss>` ", "层次sigmoid损失层"
    " :ref:`paddle.nn.KLDivLoss <cn_api_paddle_nn_KLDivLoss>` ", "Kullback-Leibler散度损失层"
    " :ref:`paddle.nn.L1Loss <cn_api_paddle_nn_L1Loss>` ", "L1损失层"
    " :ref:`paddle.nn.MarginRankingLoss <cn_api_nn_loss_MarginRankingLoss>` ", "MarginRankingLoss层"
    " :ref:`paddle.nn.MSELoss <cn_api_paddle_nn_MSELoss>` ", "均方差误差损失层"
    " :ref:`paddle.nn.NLLLoss <cn_api_nn_loss_NLLLoss>` ", "NLLLoss层"
    " :ref:`paddle.nn.SmoothL1Loss <cn_api_paddle_nn_SmoothL1Loss>` ", "平滑L1损失层"
    
.. _vision_layers:

Vision层
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.PixelShuffle <cn_api_nn_PixelShuffle>` ", "将一个形为[N, C, H, W]或是[N, H, W, C]的Tensor重新排列成形为 [N, C/r**2, H*r, W*r]或 [N, H*r, W*r, C/r**2] 的Tensor"
    " :ref:`paddle.nn.Upsample <cn_api_paddle_nn_Upsample>` ", "用于调整一个batch中图片的大小"
    " :ref:`paddle.nn.UpsamplingBilinear2D <cn_api_paddle_nn_UpsamplingBilinear2D>` ", "用于调整一个batch中图片的大小（使用双线性插值方法）"
    " :ref:`paddle.nn.UpsamplingNearest2D <cn_api_paddle_nn_UpsamplingNearest2D>` ", "用于调整一个batch中图片的大小（使用最近邻插值方法）"
    
.. _about_clip:

Clip相关
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.ClipGradByGlobalNorm <cn_api_fluid_clip_ClipGradByGlobalNorm>` ", "将一个 Tensor列表 t_list 中所有Tensor的L2范数之和，限定在 clip_norm 范围内"
    " :ref:`paddle.nn.ClipGradByNorm <cn_api_fluid_clip_ClipGradByNorm>` ", "将输入的多维Tensor X 的L2范数限制在 clip_norm 范围之内"
    " :ref:`paddle.nn.ClipGradByValue <cn_api_fluid_clip_ClipGradByValue>` ", "将输入的多维Tensor X 的值限制在 [min, max] 范围"
    
.. _common_layers:

公共层
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.BeamSearchDecoder <cn_api_fluid_layers_BeamSearchDecoder>` ", "带beam search解码策略的解码器"
    " :ref:`paddle.nn.CosineSimilarity <cn_api_nn_CosineSimilarity>` ", "余弦相似度计算"
    " :ref:`paddle.nn.dynamic_decode <cn_api_paddle_nn_dynamic_decode>` ", "循环解码"
    " :ref:`paddle.nn.Flatten <cn_api_tensor_Flatten>` ", "将一个连续维度的Tensor展平成一维Tensor"
    " :ref:`paddle.nn.PairwiseDistance <cn_api_nn_PairwiseDistance>` ", "计算两个向量之间pairwise的距离"
    " :ref:`paddle.nn.Unfold <cn_api_fluid_layers_unfold>` ", "实现的功能与卷积中用到的im2col函数一样，通常也被称作为im2col过程"

.. _convolution_functional:

卷积相关函数
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.functional.conv1d <cn_api_nn_functional_conv1d>` ", "一维卷积函数"
    " :ref:`paddle.nn.functional.conv1d_transpose <cn_api_nn_functional_conv1d_transpose>` ", "一维转置卷积函数"
    " :ref:`paddle.nn.functional.conv2d <cn_api_nn_functional_conv2d>` ", "二维卷积函数"
    " :ref:`paddle.nn.functional.conv2d_transpose <cn_api_nn_functional_conv2d_transpose>` ", "二维转置卷积函数"
    " :ref:`paddle.nn.functional.conv3d <cn_api_nn_functional_conv3d>` ", "三维卷积函数"
    " :ref:`paddle.nn.functional.conv3d_transpose <cn_api_nn_functional_conv3d_transpose>` ", "三维转置卷积函数"
    
.. _pooling_functional:

Pooling相关函数
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.functional.adaptive_avg_pool1d <cn_api_nn_functional_adaptive_avg_pool1d>` ", "一维自适应平均池化"
    " :ref:`paddle.nn.functional.adaptive_avg_pool2d <cn_api_nn_functional_adaptive_avg_pool2d>` ", "二维自适应平均池化"
    " :ref:`paddle.nn.functional.adaptive_avg_pool3d <cn_api_nn_functional_adaptive_avg_pool3d>` ", "三维自适应平均池化"
    " :ref:`paddle.nn.functional.adaptive_max_pool1d <cn_api_nn_functional_adaptive_max_pool1d>` ", "一维自适应最大池化"
    " :ref:`paddle.nn.functional.adaptive_max_pool2d <cn_api_nn_functional_adaptive_max_pool2d>` ", "二维自适应最大池化"
    " :ref:`paddle.nn.functional.adaptive_max_pool3d <cn_api_nn_functional_adaptive_max_pool3d>` ", "三维自适应最大池化"
    " :ref:`paddle.nn.functional.avg_pool1d <cn_api_nn_functional_avg_pool1d>` ", "一维平均池化"
    " :ref:`paddle.nn.functional.avg_pool2d <cn_api_nn_functional_avg_pool2d>` ", "二维平均池化"
    " :ref:`paddle.nn.functional.avg_pool3d <cn_api_nn_functional_avg_pool3d>` ", "三维平均池化"
    " :ref:`paddle.nn.functional.max_pool1d <cn_api_nn_functional_max_pool1d>` ", "一维最大池化"
    " :ref:`paddle.nn.functional.max_pool2d <cn_api_nn_functional_max_pool2d>` ", "二维最大池化"
    " :ref:`paddle.nn.functional.max_pool3d <cn_api_nn_functional_max_pool3d>` ", "三维最大池化"
    
.. _padding_functional:

Padding相关函数
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.functional.pad <cn_api_nn_cn_pad>` ", "依照 pad 和 mode 属性对input进行填充"
    " :ref:`paddle.nn.functional.zeropad2d <cn_api_nn_functional_zeropad2d>` ", "依照 pad 对x进行零填充"
    
.. _activation_functional:

激活函数
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.functional.celu <cn_api_nn_cn_celu>` ", "celu激活函数"
    " :ref:`paddle.nn.functional.elu <cn_api_nn_cn_elu>` ", "elu激活函数"
    " :ref:`paddle.nn.functional.elu_ <cn_api_nn_cn_elu_>` ", "Inplace 版本的 elu API，对输入 x 采用 Inplace 策略"
    " :ref:`paddle.nn.functional.gelu <cn_api_nn_cn_gelu>` ", "gelu激活函数"
    " :ref:`paddle.nn.functional.gumbel_softmax <cn_api_nn_cn_gumbel_softmax>` ", "gumbel_softmax采样激活函数"
    " :ref:`paddle.nn.functional.hardshrink <cn_api_nn_cn_hard_shrink>` ", "hardshrink激活函数"
    " :ref:`paddle.nn.functional.hardsigmoid <cn_api_nn_cn_hardsigmoid>` ", "sigmoid的分段线性逼近激活函数"
    " :ref:`paddle.nn.functional.hardswish <cn_api_nn_cn_hardswish>` ", "hardswish激活函数"
    " :ref:`paddle.nn.functional.hardtanh <cn_api_nn_cn_hardtanh>` ", "hardtanh激活函数"
    " :ref:`paddle.nn.functional.leaky_relu <cn_api_nn_cn_leaky_relu>` ", "leaky_relu激活函数"
    " :ref:`paddle.nn.functional.log_sigmoid <cn_api_nn_cn_log_sigmoid>` ", "log_sigmoid激活函数"
    " :ref:`paddle.nn.functional.log_softmax <cn_api_nn_cn_log_softmax>` ", "log_softmax激活函数"
    " :ref:`paddle.nn.functional.maxout <cn_api_nn_cn_maxout>` ", "maxout激活函数"
    " :ref:`paddle.nn.functional.prelu <cn_api_nn_cn_prelu>` ", "prelu激活函数"
    " :ref:`paddle.nn.functional.relu <cn_api_nn_cn_relu>` ", "relu激活函数"
    " :ref:`paddle.nn.functional.relu_ <cn_api_nn_cn_relu_>` ", "Inplace 版本的 :ref:`cn_api_nn_cn_relu` API，对输入 x 采用 Inplace 策略"
    " :ref:`paddle.nn.functional.relu6 <cn_api_nn_cn_relu6>` ", "relu6激活函数"
    " :ref:`paddle.nn.functional.selu <cn_api_nn_cn_selu>` ", "selu激活函数"
    " :ref:`paddle.nn.functional.sigmoid <cn_api_fluid_layers_sigmoid>` ", "sigmoid激活函数"
    " :ref:`paddle.nn.functional.silu <cn_api_nn_cn_silu>` ", "silu激活函数"
    " :ref:`paddle.nn.functional.softmax <cn_api_nn_cn_softmax>` ", "softmax激活函数"
    " :ref:`paddle.nn.functional.softmax_ <cn_api_nn_cn_softmax_>` ", "Inplace 版本的 :ref:`cn_api_nn_cn_softmax` API，对输入 x 采用 Inplace 策略"
    " :ref:`paddle.nn.functional.softplus <cn_api_nn_cn_softplus>` ", "softplus激活函数"
    " :ref:`paddle.nn.functional.softshrink <cn_api_nn_cn_softshrink>` ", "softshrink激活函数"
    " :ref:`paddle.nn.functional.softsign <cn_api_nn_cn_softsign>` ", "softsign激活函数"
    " :ref:`paddle.nn.functional.swish <cn_api_nn_cn_swish>` ", "swish激活函数"
    " :ref:`paddle.nn.functional.tanhshrink <cn_api_nn_cn_tanhshrink>` ", "tanhshrink激活函数"
    " :ref:`paddle.nn.functional.thresholded_relu <cn_api_nn_cn_thresholded_relu>` ", "thresholded_relu激活函数"
    
.. _normalization_functional:

Normalization方法
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.functional.local_response_norm <cn_api_nn_functional_local_response_norm>` ", "Local Response Normalization函数"
    " :ref:`paddle.nn.functional.normalize <cn_api_nn_functional_normalize>` ", "归一化方法"
    " :ref:`paddle.nn.functional.remove_weight_norm <cn_api_nn_cn_remove_weight_norm>` ", "移除传入 layer 中的权重归一化"
    " :ref:`paddle.nn.functional.weight_norm <cn_api_nn_cn_weight_norm>` ", "对传入的 layer 中的权重参数进行归一化"
    " :ref:`paddle.nn.functional.spectral_norm <cn_api_nn_cn_spectral_norm>` ", "对传入的 layer 中的权重参数进行谱归一化"

.. _linear_functional:

线性处理相关函数
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.functional.bilinear <cn_api_nn_functional_bilinear>` ", "对两个输入执行双线性张量积"
    " :ref:`paddle.nn.functional.linear <cn_api_paddle_nn_functional_common_linear>` ", "线性变换"
    
.. _dropout_functional:

Dropout方法
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.functional.alpha_dropout <cn_api_nn_functional_alpha_dropout>` ", "一种具有自归一化性质的dropout"
    " :ref:`paddle.nn.functional.dropout <cn_api_nn_functional_dropout>` ", "Dropout"
    " :ref:`paddle.nn.functional.dropout2d <cn_api_nn_functional_dropout2d>` ", "一维Dropout"
    " :ref:`paddle.nn.functional.dropout3d <cn_api_nn_functional_dropout3d>` ", "二维Dropout"
    
.. _embedding_functional:

Embedding相关函数
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.functional.diag_embed <cn_api_functional_diag_embed>` ", "对角线Embedding 方法"
    " :ref:`paddle.nn.functional.embedding <cn_api_nn_functional_embedding>` ", "Embedding 方法"
    
.. _loss_functional:

损失函数
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.functional.binary_cross_entropy <cn_api_nn_functional_binary_cross_entropy>` ", "二值交叉熵损失值"
    " :ref:`paddle.nn.functional.binary_cross_entropy_with_logits <cn_api_paddle_nn_functional_binary_cross_entropy_with_logits>` ", "logits二值交叉熵损失值"
    " :ref:`paddle.nn.functional.ctc_loss <cn_paddle_nn_functional_loss_ctc>` ", "用于计算ctc损失"
    " :ref:`paddle.nn.functional.dice_loss <cn_api_fluid_layers_dice_loss>` ", "用于比较预测结果跟标签之间的相似度"
    " :ref:`paddle.nn.functional.hsigmoid_loss <cn_api_nn_functional_hsigmoid_loss>` ", "层次sigmoid损失函数"
    " :ref:`paddle.nn.functional.l1_loss <cn_paddle_nn_functional_loss_l1>` ", "用于计算L1损失"
    " :ref:`paddle.nn.functional.kl_div <cn_paddle_nn_functional_loss_kl_div>` ", "用于计算KL散度损失"
    " :ref:`paddle.nn.functional.log_loss <cn_api_fluid_layers_log_loss>` ", "用于计算负对数损失"
    " :ref:`paddle.nn.functional.margin_ranking_loss <cn_api_nn_cn_margin_ranking_loss>` ", "用于计算margin rank loss 损失"
    " :ref:`paddle.nn.functional.mse_loss <cn_paddle_nn_functional_mse_loss>` ", "用于计算均方差误差"
    " :ref:`paddle.nn.functional.nll_loss <cn_api_nn_functional_nll_loss>` ", "用于计算nll损失"
    " :ref:`paddle.nn.functional.npair_loss <cn_api_fluid_layers_npair_loss>` ", "成对数据损失计算"
    " :ref:`paddle.nn.functional.sigmoid_focal_loss <cn_api_nn_functional_sigmoid_focal_loss>` ", "用于计算分类任务中前景类-背景类数量不均衡问题的损失"
    " :ref:`paddle.nn.functional.smooth_l1_loss <cn_paddle_nn_functional_loss_smooth_l1>` ", "用于计算平滑L1损失"
    " :ref:`paddle.nn.functional.softmax_with_cross_entropy <cn_api_fluid_layers_softmax_with_cross_entropy>` ", "将softmax操作、交叉熵损失函数的计算过程进行合并"
    " :ref:`paddle.nn.functional.margin_cross_entropy <cn_api_paddle_nn_functional_margin_cross_entropy>` ", "支持 ``Arcface``，``Cosface``，``Sphereface`` 的结合 Margin 损失函数"
    
.. _common_functional:

公用方法
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.functional.affine_grid <cn_api_nn_functional_affine_grid>` ", "用于生成仿射变换前后的feature maps的坐标映射关系"
    " :ref:`paddle.nn.functional.cosine_similarity <cn_api_paddle_nn_cosine_similarity>` ", "用于计算x1与x2沿axis维度的余弦相似度"
    " :ref:`paddle.nn.functional.cross_entropy <cn_api_paddle_functional_cross_entropy>` ", "计算输入input和标签label间的交叉熵"
    " :ref:`paddle.nn.functional.grid_sample <cn_api_nn_functional_grid_sample>` ", "用于调整一个batch中图片的大小"
    " :ref:`paddle.nn.functional.label_smooth <cn_api_paddle_nn_functional_common_label_smooth>` ", "标签平滑"
    " :ref:`paddle.nn.functional.one_hot <cn_api_nn_functional_one_hot>` ", "将输入'x'中的每个id转换为一个one-hot向量"
    " :ref:`paddle.nn.functional.pixel_shuffle <cn_api_nn_functional_pixel_shuffle>` ", "将Tensor重新排列"
    " :ref:`paddle.nn.functional.square_error_cost <cn_api_fluid_layers_square_error_cost>` ", "用于计算预测值和目标值的方差估计"
    " :ref:`paddle.nn.functional.unfold <cn_api_fluid_layers_unfold>` ", "对每一个卷积核覆盖下的区域，将元素重新排成一列"
    " :ref:`paddle.nn.functional.gather_tree <cn_api_fluid_layers_gather_tree>` ", "整个束搜索结束后使用,获得每个时间步选择的的候选词 id 及其对应的在搜索树中的 parent 节点"
    " :ref:`paddle.nn.functional.glu <cn_api_nn_cn_glu>` ", "门控线性单元"
    " :ref:`paddle.nn.functional.interpolate <cn_api_paddle_nn_functional_interpolate>` ", "用于调整一个batch中图片的大小"
    " :ref:`paddle.nn.functional.sequence_mask <cn_api_fluid_layers_sequence_mask>` ", "根据输入 x 和 maxlen 输出一个掩码，数据类型为 dtype"
    " :ref:`paddle.nn.functional.temporal_shift <cn_api_fluid_layers_temporal_shift>` ", "用于对输入X做时序通道T上的位移操作，为TSM中使用的操作"
    " :ref:`paddle.nn.functional.upsample <cn_api_paddle_nn_functional_upsample>` ", "用于调整一个batch中图片的大小"
    " :ref:`paddle.nn.functional.class_center_sample <cn_api_paddle_nn_functional_class_center_sample>` ", "用于PartialFC类别中心采样"

.. _about_initializer:

初始化相关
:::::::::::::::::::::::

.. csv-table::
    :header: "API名称", "API功能"
    

    " :ref:`paddle.nn.initializer.Assign <cn_api_nn_initializer_Assign>` ", "使用Numpy数组、Python列表、Tensor来初始化参数"
    " :ref:`paddle.nn.initializer.Bilinear <cn_api_nn_Bilinear>` ", "该接口为参数初始化函数，用于转置卷积函数中"
    " :ref:`paddle.nn.initializer.Constant <cn_api_nn_initializer_Constant>` ", "用于权重初始化，通过输入的value值初始化输入变量"
    " :ref:`paddle.nn.initializer.KaimingNormal <cn_api_nn_initializer_KaimingNormal>` ", "实现Kaiming正态分布方式的权重初始化"
    " :ref:`paddle.nn.initializer.KaimingUniform <cn_api_nn_initializer_KaimingUniform>` ", "实现Kaiming均匀分布方式的权重初始化"
    " :ref:`paddle.nn.initializer.Normal <cn_api_nn_initializer_Normal>` ", "随机正态（高斯）分布初始化函数"
    " :ref:`paddle.nn.initializer.set_global_initializer <cn_api_nn_initializer_set_global_initializer>` ", "用于设置Paddle框架中全局的参数初始化方法"
    " :ref:`paddle.nn.initializer.calculate_gain <cn_api_nn_initializer_calculate_gain>` ", "获取某些激活函数的推荐增益值（增益值可用于对某些初始化API进行设置，以调整初始化值）"
    " :ref:`paddle.nn.initializer.Dirac <cn_api_nn_initializer_Dirac>` ", "通过狄拉克delta函数来初始化3D/4D/5D Tensor，一般用于卷积层，能最大程度保留卷积层输入的特性"
    " :ref:`paddle.nn.initializer.Orthogonal <cn_api_nn_initializer_Orthogonal>` ", "正交矩阵初始化方式，被初始化的参数为（半）正交的"
    " :ref:`paddle.nn.initializer.TruncatedNormal <cn_api_nn_initializer_TruncatedNormal>` ", "随机截断正态（高斯）分布初始化函数"
    " :ref:`paddle.nn.initializer.Uniform <cn_api_nn_initializer_Uniform>` ", "随机均匀分布初始化函数"
    " :ref:`paddle.nn.initializer.XavierNormal <cn_api_nn_initializer_XavierNormal>` ", "实现Xavier权重初始化方法（ Xavier weight initializer）"
    " :ref:`paddle.nn.initializer.XavierUniform <cn_api_nn_initializer_XavierUniform>` ", "实现Xavier权重初始化方法（ Xavier weight initializer）"
