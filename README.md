# ECC_CRC
<br>
a cyclic redundancy check(one kind of Error Correcting Code) software and hardware implementation.
一个循环校验码（一种ecc错误校验码）的软件和硬件实现
<br>
<br>
## Software Implementations
<br> <br> 
For the powerful matrix computing abilities, and gui features, I choose MATLAB for the software and algorithms implementation platform. The functions can be summarized as follows:

* 1. Calculating the data matrix and crc matrix used in the encoding circuits. Generating polynomial(in hex form), data width, and crc width are required as inputs. 
* 2. Calculating the error-location map used in the decoder-corrector circuits. Inputs requirements are the same.
* 3. Automatically generating the verilog HDL codes for encoder and decoder function modules.

由于MATLAB的高效矩阵运算性能，算法部分由MATLAB实现
mat文件夹下，generatorGUI.m ，目前已经实现的功能和算法：
* 1.求解任意生成多项式、数据校验位宽的循环校验码编码算法。包括计算Data矩阵，Crc矩阵，给定信息位求校验位3个功能；
* 2.求解任意生成多项式、数据校验位宽的循环校验码解码算法。可一键生成Error-Bits映射关系表；
* 3.输入生成多项式、（parallel data bits）并行度和校验位宽，一键生成对应的verilog HDL组合逻辑功能模块;

<br> <br> 

## Hardware Implementations
