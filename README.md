# mrubyc-rp2
mruby/c for Raspberry Pi Pico

## ソースコードの取得
```
$ git clone https://github.com/k-mana/mrubyc-rp2.git --recursive
```
または
```
$ git clone https://github.com/k-mana/mrubyc-rp2.git
$ cd mrubyc-rp2
$ git submodule update --init --recursive
```

## ビルドツールのインストール
```
$ sudo apt install cmake build-essential gcc-arm-none-eabi libnewlib-arm-none-eabi libstdc++-arm-none-eabi-newlib python3
```

## ビルド
```
$ cd mrubyc-rp2
$ cmake -S . -B build
$ cmake --build build
$ ls build/blink.uf2
```
