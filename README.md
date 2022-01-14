# ROSpackage-twice
[上田先生の講義動画](https://www.youtube.com/watch?v=PL85Pw_zQH0)通りにROSのパッケージを作りました。count.pyで1ずつ大きくなっていく値を出力し、twice.pyで2倍にした値を返します。

## 準備
ROSのインストールは[こちら](https://github.com/ryuichiueda/ros_setup_scripts_Ubuntu20.04_server)から
### ワークスペースの構築 
`$ mkdir -p catkin_ws/src`  
`$ cd ~/catkin_ws/src`  
`$ catkin_init_workspace`  
.bashrcの末尾に以下を追加  
`source ~/catkin_ws/devel/setup.bash`  
### 環境構築のビルド
`$ cd ~/catkin_ws`
`$ catkin_make`
`$ source ~/.bashrc`

## インストール方法
このリポジトリをforkして`~/catkin_ws/src`内に`git clone`でcloneして使用してください。

## 使用方法  
端末を4つ用意し、端末1にて  
`$ roscore`  

端末2にて  
作業ディレクトリに移動  
`$ cd ~/catkin_ws/src/mypkg/scripts$`  
実行権限確認  
`~/scripts$ ls -l count.py`  
実行権限付与  
`$ chmod +x count.py`  
実行  
`$ rosrun mypkg count.py`  
  
端末3にて  
作業ディレクトリに移動  
`$ cd ~/catkin_ws/src/mypkg/scripts$`   
実行権限確認  
`~/scripts$ ls -l twice.py`  
実行権限付与  
`$ chmod +x twice.py`  
実行  
`$ rosrun mypkg count.py`  

端末4にて  
トピック動作確認  
`$ rostopic list`  
実行結果確認  
`$ rostopic echo /twice`  

## デモ動画
実際に動かしたところを下記のリンクより確認できます。  
[課題2の動画](https://www.youtube.com/watch?v=x592a3M3u0I)

## 参考動画
[ロボットシステム学第10回（ROS）(Youtube)](https://www.youtube.com/watch?v=PL85Pw_zQH0)

## ライセンス
このプロジェクトは3条項BSDライセンスに基づいています。
