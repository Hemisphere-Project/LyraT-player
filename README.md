# LyraT-player

### compile -> upload

cd [projectpath]/
export ADF_PATH=~/esp/esp-adf
. $HOME/esp/esp-idf/export.sh
idf.py set-target esp32
# idf.py menuconfig 
idf.py build
idf.py -p /dev/ttyUSB0 -b 921600 flash monitor   # Push reset