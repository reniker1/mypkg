# パッケージ内容
![test](https://github.com/reniker1/mypkg/actions/workflows/test.yml/badge.svg)

talkerが0.5秒ごとにカウントした整数をlistenerが受け取り表示させる

## 必要なソフトウェア

* Python

* ROS2

## 利用手順

* 自身のターミナルに
```
 git clone https://github.com/reniker1/mypkg.git
```
を入力

* ```mypkg``` があることを確認

* ```mypkg```のリポジトリで実行

## 実行方法

### 方法①　端末を2つ用意
* 端末1 talker
  * 以下のコマンドをターミナル上で実行
```
 ros2 run mypkg talker
```
* 端末2 listener
  * 以下のコマンドをターミナル上で実行
```
 ros2 run mypkg listener
```
　   
### 方法②　端末を１つ用意
* 以下のコマンドをターミナル上で実行
```
  ros2 launch mypkg talk_listen.launch.py
```

## テスト環境

* Ubuntu 22.04

## ライセンス

* このソフトウェアパッケージは，3条項BSDライセンスの下、再頒布および使用が許可されます。
* このパッケージのコードは、下記のスライド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを、本人の許可を得て自身の著作としたものです。

  * [ryuichiueda.github.io/my_slides/robosys_2022](https://ryuichiueda.github.io/my_slides/robosys_2022/lesson8.html#/22)
 
* © 2023 Ren Imai

