.. _cn_api_paddle_row_stack:

row_stack
-------------------------------

.. py:function:: paddle.row_stack(x, name=None)

:ref:`cn_api_paddle_vstack` 的别名。沿垂直轴堆叠输入 ``x`` 中的所有张量。所有张量必须具有相同的数据类型。

下图展示了一个 row_stack 的情形，将一个形状为（1，3）的二维张量与另一个同样形状为（1，3），但是数据内容不同的二维张量进行 row_stack 操作，二者沿垂直轴堆叠成一个新的二维向量。通过图例能很好看出张量的变化。

.. image:: ../../images/api_legend/row_stack.png
    :width: 600
    :alt: 图例

参数
::::::::::::

    - **x** (list[Tensor]|tuple[Tensor]) - 输入 ``x`` 可以是张量的 list 或 tuple， ``x`` 中张量的数据类型必须相同。支持的数据类型： ``float16`` 、 ``float32`` 、 ``float64`` 、 ``int32`` 、 ``int64`` 或 ``bfloat16`` 。
    - **name** (str，可选) - 具体用法请参见 :ref:`api_guide_Name`，一般无需设置，默认值为 None。

返回
::::::::::::
Tensor，与输入数据类型相同的堆叠张量。

代码示例
::::::::::::

COPY-FROM: paddle.row_stack
