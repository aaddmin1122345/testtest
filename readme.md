# ready build dir
mkdir build
cd build
# generate
cmake -DCMAKE_BUILD_TYPE=Release \
      -DCMAKE_INSTALL_PREFIX=/usr \
      -Dbuild_execsnoop_dl=ON \
      -Dbuild_static=OFF \
      ..
# compile
make
sudo make install
