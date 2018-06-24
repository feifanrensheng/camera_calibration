张正友法相机内参标定
基于opencv-2.4.9,cmake工程，可在ubuntu系统下编译执行

编译
mkdir build
cd build
cmake ..
make 


执行
事先对你准备的标定棋盘图从不同角度拍摄14张图片
放入到build文件目录下，执行类似如下命令
./cb chess1.bmp ./chess2.bmp ./chess3.bmp ./chess4.bmp ./chess5.bmp ./chess6.bmp ./chess7.bmp ./chess8.bmp ./chess9.bmp ./chess10.bmp ./chess11.bmp ./chess12.bmp ./chess13.bmp ./chess14.bmp
标定结果保存在caliberation_result.txt文件中
