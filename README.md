# QtBuild
Build Qt6.3.2 universal version(Intel & Apple silicon) with namespace "SD_QT" on MacOS.

1. Download Qt6.3.2 source code from　https://download.qt.io/archive/qt/6.3/6.3.2/single/
   
2. We used the following compile options：

      ./configure -release -prefix YOUR_INSTALL_PATH -nomake examples -nomake tests -opensource -confirm-license -qtnamespace SD_QT
   
      ./configure -- -DCMAKE_OSX_ARCHITECTURES="x86_64;arm64"
   
      cmake --build --parallel
   
      cmake --install

4. You can obtain the compiled binary file from http://lt3d.oss-cn-hangzhou.aliyuncs.com/style3d/SD_QT_6.3.2_universal.zip
