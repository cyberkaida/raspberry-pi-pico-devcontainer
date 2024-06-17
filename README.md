# Raspberry Pi Pico Devcontainer

This devcontainer has everything you need to build
for the Raspberry Pi Pico.

The [pico-sdk](https://github.com/raspberrypi/pico-sdk) is
located in `/opt` and the environment variable `PICO_SDK_PATH`
is correctly set.

All the build requirements are installed.

To try, start the devcontainer and clone
[pico-examples](https://github.com/raspberrypi/pico-examples)
into it. Then build the examples!

```sh
# Inside the devcontainer
echo ${PICO_SDK_PATH}
git clone https://github.com/raspberrypi/pico-examples.git
mkdir build
cd build
cmake ../pico-examples
make
# ✨👩‍💻 Enjoy! Copy the build output to your pico!
```
