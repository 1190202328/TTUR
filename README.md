# FID评价

本仓库来源于[https://github.com/bioinf-jku/TTUR]

## 主要改动

1. 主要改动集中在[fid.py]的line[307,333]
    1. 对读取的图片进行了resize操作
    2. 可以读取子文件夹下的图片（为了读取CUB的测试集）


## 安装依赖库

1. `pip install -r requirements.txt`
2. 注意tensorflow为1.x版本，scipy为1.2.1版本

## 运行

1. `fid.py /path/to/images /path/to/other_images`  
2. 示例 `python fid.py ../text2image/saved_model/OneDrive-2022-05-29/finetune/cub/netG_550/test_every ../text2image/data/birds/CUB_200_2011/images/ --inception=../text2image/tmp/imagenet/ --gpu=0,1`
3. 其余用法请参考[https://github.com/bioinf-jku/TTUR]

[https://github.com/bioinf-jku/TTUR]:https://github.com/bioinf-jku/TTUR
[fid.py]:fid.py