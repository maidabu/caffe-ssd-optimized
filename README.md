# Introduction

Original SSD source code training speed is too low, so I change the data preprocessing part to multithreading and optimize the preprocessing flow.


# Method of use
```bash
git clone https://github.com/maidabu/caffe-ssd-optimized.git
cd caffe-ssd-optimized
cp -r include/ your_caffe_ssd_source_code_root/
cp -r src/ your_caffe_ssd_source_code_root/
cp -r CMakeLists.txt your_caffe_ssd_source_code_root/
cp -r Makefile your_caffe_ssd_source_code_root/
cp -r Makefile.config.example your_caffe_ssd_source_code_root/
```

# The performance test

Environment : i7-7800X + GTX1080

The speed of data preprocessing is 10 to 20 times faster than original ssd

The speed of training(with data preprocessing, forward, backward) is 4 to 6 times faster than original ssd

