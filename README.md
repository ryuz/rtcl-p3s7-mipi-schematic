English version: [README_en.md](README_en.md)

# グローバルシャッターMIPI高速度カメラ(PYTHON300 + Spartan7)

## 概要

[こちら](https://rtc-lab.com/products/rtcl-cam-p3s7-mipi/)で紹介しておりますグローバルシャッターMIPI高速度カメラの回路図のみの配布です。

オンセミコンダクター社 [PYTHON300イメージセンサー](https://www.onsemi.jp/products/sensors/image-sensors/python300) と AMD(Xilinx) の [Spartan7](https://www.amd.com/ja/products/adaptive-socs-and-fpgas/fpga/spartan-7.html) FPGA を用いた研究開発向けの小型のカメラモジュールです。

データシート上は VGA サイズながら 815fps の高速度撮影が可能と記載されているセンサーを利用しており、当方では [KV260](https://www.amd.com/ja/products/system-on-modules/kria/k26/kv260-vision-starter-kit.html) と [Zybo Z7](https://digilent.com/shop/zybo-z7-zynq-7000-arm-fpga-soc-development-board/) に接続して 320x320 サイズで 1000fps 撮像が出来ております。

![カメラ外観写真](camera_photo.png)

撮影動画なども[こちら](https://rtc-lab.com/products/rtcl-cam-p3s7-mipi/)で紹介しております。

## 回路図

回路図は以下です。

- [イメージセンサー子基板](sensor_python300.pdf)
- [FPGA親基板](mipi_spartan7.pdf)


## 基板設計データ

KiCAD の設計データは別途 [こちら](https://github.com/ryuz/rtcl-p3s7-mipi-pcb) にて公開しております。


## ライセンス(License)

本リポジトリの回路図などは MIT ライセンスにて配布いたします。


## 基板販売

当方で製造したものを[BOOTH](https://rtc-lab.booth.pm/)にて販売中です。

- [モノクロ版](https://rtc-lab.booth.pm/items/7427869)
- [カラー版](https://rtc-lab.booth.pm/items/7428802)


## 関連ソフトウェア

現時点では、KV260 に独自仕様でデータを送るプロジェクトがあります。

- [Spartan-7 のデザイン](https://github.com/ryuz/rtcl-designs/tree/main/projects/rtcl_p3s7_mipi/rtcl_p3s7_mipi)
- [KV260 の デザイン](https://github.com/ryuz/rtcl-designs/tree/main/projects/kv260/kv260_rtcl_p3s7_hs)
- [ZYBO の デザイン](https://github.com/ryuz/rtcl-designs/tree/main/projects/zybo_z7/zybo_z7_rtcl_p3s7_hs)



## 作者情報

渕上 竜司(Ryuji Fuchikami)
[リアルタイムコンピューティング研究所](https://rtc-lab.com/)
