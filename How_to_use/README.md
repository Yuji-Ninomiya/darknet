## How to train for recognition of vs087

> 実験室 Monster PC にて実行した手順

##参照

YOLO : https://pjreddie.com/darknet/yolo/

学習の流れ ： http://demura.net/misc/14458.html

データセットの作成： http://demura.net/misc/14350.html

***
#### 1. darknet

```
$ cd ~Your_workspace/

$ git clone https://github.com/pjreddie/darknet`
```
	/cfg/ ~~.data, ~~_train.cfg, ~~_test.cfg <---新規追加したやつ
	/data/test/vs087_real <--- テストデータ

***
YOLO_denso/ImageAnnotation/labelImg `git clone https://github.com/tzutalin/labelImg.git`

	/data/robot/vs087 <---画像、.weight ファイル（git管理しない）

	/ImageAnnotation/imagae <---自作したデータセット

***
YOLO_denso/divide_files <- git clone https://github.com/demulab/divide_files.git　<---git 管理しない

