# パーセプトロン・ニューラルネットワーク

## パーセプトロンとは

* 複数の入力に対して「0」か「1」を返却する関数のこと
* イメージは以下  
![パーセプトロンイメージ](https://raw.githubusercontent.com/learn-ttm/AI_study/image/image/perceptron.png)  
* 入力値：![](https://latex.codecogs.com/gif.latex?\large&space;x_{1},x_{2})  
重み：![](https://latex.codecogs.com/gif.latex?\large&space;w_{1},w_{2})  
出力値：![](https://latex.codecogs.com/gif.latex?\large&space;y)
* 入力値に対して重みを乗算し、バイアス(イメージからは省略)を加算した結果が閾値を超えた場合に「1」、超えない場合に「0」を出力する
* 数式で表すと以下の通り(閾値を0とした場合)  
![](https://raw.githubusercontent.com/learn-ttm/AI_study/image/image/perceptron_formula.gif)
* 同じ入力値であっても、重みやバイアスを変化させることで出力結果をコントロールすることができる