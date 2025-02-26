# navicat-keygen for linux - 如何编译？

## 1. 前提条件

1. 安装最新的 `CMake`:

   ```bash
   sudo apt-get -y install cmake g++
   ```

2. 安装 `fmt`、`OpenSSL` 和 `rapidjson`:

   ```bash
   sudo apt-get -y install libfmt-dev libssl-dev rapidjson-dev pkg-config
   ```

## 2. 编译

1. clone仓库:

   ```bash
   git clone -b linux --single-branch https://notabug.org/doublesine/navicat-keygen.git
   cd navicat-keygen
   ```

2. 编译:

   ```bash
   mkdir build
   cd build
   cmake -DCMAKE_BUILD_TYPE=Release ..
   cmake --build . -- -j4
   ```

   编译完后你会在build文件夹里看到两个可执行文件 `navicat-keygen` 和 `navicat-patcher`。
