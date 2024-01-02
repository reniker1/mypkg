# パッケージ内容
![test](https://github.com/reniker1/mypkg/actions/workflows/test.yml/badge.svg)

talkerが0.5秒ごとにカウントした整数をlistenerが受け取り表示させる

## 必要なソフトウェア

* Python

* ROS2

## ノードの説明

### 機能

#### talker
* 数字をカウントしてトピック/countupを通じて送信

#### listener
* トピック/countupからメッセージをもらって表示

## トピックの説明
* Int16型のメッセージをtalkerから受け取りlistenerにつなぐ

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

## 実行結果

### 方法①

```
[INFO] [1704169029.422928264] [listener]: Listen: 0
[INFO] [1704169029.940791911] [listener]: Listen: 1
[INFO] [1704169030.402770100] [listener]: Listen: 2
[INFO] [1704169030.937259785] [listener]: Listen: 3
[INFO] [1704169031.418412331] [listener]: Listen: 4
[INFO] [1704169031.939150605] [listener]: Listen: 5
[INFO] [1704169032.413963090] [listener]: Listen: 6
[INFO] [1704169032.944447052] [listener]: Listen: 7
[INFO] [1704169033.400378366] [listener]: Listen: 8
[INFO] [1704169033.942804341] [listener]: Listen: 9
[INFO] [1704169034.408537345] [listener]: Listen: 10
```

### 方法②

```
[INFO] [launch]: All log files can be found below /home/cassilas/.ros/log/2024-01-02-13-21-31-234168-CASILLAS-1077
[INFO] [launch]: Default logging verbosity is set to INFO
[INFO] [talker-1]: process started with pid [1078]
[INFO] [listener-2]: process started with pid [1080]
[listener-2] [INFO] [1704169292.204619180] [listener]: Listen: 0
[listener-2] [INFO] [1704169292.681834134] [listener]: Listen: 1
[listener-2] [INFO] [1704169293.183231593] [listener]: Listen: 2
[listener-2] [INFO] [1704169293.691928525] [listener]: Listen: 3
[listener-2] [INFO] [1704169294.189156054] [listener]: Listen: 4
[listener-2] [INFO] [1704169294.686576589] [listener]: Listen: 5
[listener-2] [INFO] [1704169295.185302321] [listener]: Listen: 6
[listener-2] [INFO] [1704169295.682047661] [listener]: Listen: 7
[listener-2] [INFO] [1704169296.183680950] [listener]: Listen: 8
[listener-2] [INFO] [1704169296.685250597] [listener]: Listen: 9
[listener-2] [INFO] [1704169297.222503828] [listener]: Listen: 10
```

## テスト環境

* Ubuntu 22.04

## ライセンス

* このソフトウェアパッケージは，3条項BSDライセンスの下、再頒布および使用が許可されます。
* このパッケージのコードは、下記のスライド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを、本人の許可を得て自身の著作としたものです。

  * [ryuichiueda.github.io/my_slides/robosys_2022](https://ryuichiueda.github.io/my_slides/robosys_2022/lesson8.html#/22)
 
* © 2024 Ren Imai

