sudo .github/scripts/init_linux_port_vm_network.sh
cmake -G Ninja -DVENDOR=PC -DBOARD=linux -Bbuild_linux .
cmake --build build_linux

sudo ./build_linux/demos/projects/PC/linux/iot-middleware-sample


sudo .github/scripts/init_linux_port_vm_network.sh

cmake -G Ninja -DVENDOR=PC -DBOARD=linux -Bbuild_linux . &&  cmake --build build_linux && sudo ./build_linux/demos/projects/PC/linux/iot-middleware-sample-pnp
