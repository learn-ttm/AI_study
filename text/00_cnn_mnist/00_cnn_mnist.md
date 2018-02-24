# 順伝播型ニューラルネットワークのチュートリアル

## チュートリアルのファイルを動かす

以下のファイルを動作させてみる。
tensorflow/examples/tutorials/layers/cnn_mnist.py

### ■動作結果

pythonファイルを最後まで実施すると以下の結果が表示される。  
20000回実行して、精度(accuracy)は約97%と高く、誤差は0.09と限りなく小さい。

    INFO:tensorflow:Saving dict for global step 20000: accuracy = 0.9711, global_step = 20000, loss = 0.093937814  
    {'accuracy': 0.9711, 'loss': 0.093937814, 'global_step': 20000}  

誤差がどのように変化していくのかはTensorBoardで可視化して確認可能。  
下記コマンドをプロンプト上で実行。

    tensorboard --logdir=/tmp/mnist_convnet_model

実行すると以下のような表示が出る。

    TensorBoard 1.5.0 at http://********:6006 (Press CTRL+C to quit)
    (********部分はおそらくPC名が表示される)

この状態で「http～」の部分をそのままブラウザに張り付ければ、TensorBoardが起動する。  
※localhost:6006で起動するらしいのだが、自分のPCでは起動せず…。

実際に表示されたグラフは以下。  
学習が進むにつれ、誤差が小さくなっていることが分かる。
![](https://raw.githubusercontent.com/learn-ttm/AI_study/image/image/loss.png)