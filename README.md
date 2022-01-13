# mypkg
ロボットシステム学　課題2のリポジトリです。

# 内容
[上田先生の講義動画](https://www.youtube.com/watch?v=PL85Pw_zQH0)通りにROSのパッケージを作りました。count.pyで1ずつ大きくなっていく値を出力し、twice.pyで2倍にした値を返します。

#使用方法
端末を4つ用意し、端末1にて  `$ roscore`  

端末2にて  
作業ディレクトリに移動  
`$ cd ~/catkin_ws/src/mypkg/scripts$`  
実行権限確認  
`~/scripts$ ls -l count.py`  
実行権限付与  
`$  chmod +x count.py`  
実行  
`$ rosrun mypkg count.py`  
  
端末3にて  
作業ディレクトリに移動  
`$ cd ~/catkin_ws/src/mypkg/scripts$`   


# Youtubeのリンク
実際に動かしたところを下記のリンクより確認できます。  
[課題2の動画](https://www.youtube.com/watch?v=x592a3M3u0I)

# 参考動画
[ロボットシステム学第10回（ROS）(Youtube)](https://www.youtube.com/watch?v=PL85Pw_zQH0)
