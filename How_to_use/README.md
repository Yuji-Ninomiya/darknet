## How to train for recognition of vs087

> 実験室 Monster PC にて実行した手順

## 参照

YOLO : https://pjreddie.com/darknet/yolo/
学習の流れ ： http://demura.net/misc/14458.html
データセットの作成： http://demura.net/misc/14350.html

***
### 1. darknet

```
$ cd your_workspace/

$ git clone https://github.com/pjreddie/darknet`
```

#### 新規追加

```	
$ cd darknet/cfg/
$ vs087.data, vs087_train.cfg, vs087_test.cfg
```

#### テストデータ

```
$ cd darknet/data/test/vs087_real
```

***
### 2. Annotation

```
$ cd your_workspace/

$ mkdir ImageAnnotation & cd ImageAnnotation/

$ git clone https://github.com/tzutalin/labelImg.git
```

画像、.weights ファイル ---> `/ImageAnnotation/labelImg/data/robot/vs087`

自作したデータセット     ---> `/ImageAnnotation/image`

上記ファイルは NAS の `public/産ロボ会議/YOLO/ImageAnnotation` に保存

***
### 3. 必要な実行ファイルのインストール

```
$ cd your_workspace/

$ git clone https://github.com/demulab/divide_files.git
```
