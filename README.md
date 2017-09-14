# KelpNet
KelpNetはC#で実装された深層学習のライブラリです

## 特徴
- 行列演算をライブラリに頼らないため全ソースが可読になっており、どこで何をしているかを全て観測できます
- KerasやChainerが採用している、関数を積み重ねるように記述するコーディングスタイルを採用しています
- C#特有の記述を極力避けているため、C#以外のプログラマーでも読み切れるようになっていると思います
- 並列演算にOpenCLを採用しているため様々な演算装置で処理の並列化が可能です。
> GPU（Geforce、Radeon、etc)、CPU(Intel、AMD、etc)、FPGA 等

### C#で作られているメリット
- 開発環境の構築が容易で、プログラミング初学者にも学びやすい言語です
- WindowsFormやUnity等、処理結果を視覚的に表示するための選択肢が豊富です
- 様々な環境で動作するため、公開したいアプリケーションに組み込むことが簡単です

## このライブラリについて
このライブラリの基幹部分はChainerを参考に実装されています。
そのため多くのパラメータがChainerと同じになっておりChainer向けのサンプルを参考にすることが容易になっています。
> ※ただし四則演算や初等関数の自動微分が実装されていないため、自動微分が必要なサンプルは参考にできません

このライブラリは、他に先行するライブラリと比較すると、まだまだ機能が少ない状態です。
また、私自身が深層学習を勉強中であり、間違っている点もあるかと思います。
細やかなことでも構いませんので、何かお気づきの点が御座いましたら、お気軽にご連絡ください。


## 連絡方法
ご質問、ご要望は Issues へご登録頂くか Twitter からご連絡ください

Twitter: https://twitter.com/harujoh


## License
- KelpNet [Apache License 2.0]
- Cloo [MIT License] https://sourceforge.net/projects/cloo/

## 実装済み関数
- Activations:
　・ELU
　・LeakyReLU
　・ReLU
　・Sigmoid
　・Tanh
　・Softmax
　・Softplus
- Connections:
　・Convolution2D
　・Deconvolution2D
　・EmbedID
　・Linear
　・LSTM
- Poolings:
　・AveragePooling
　・MaxPooling
- LossFunctions:
　・MeanSquaredError
　・SoftmaxCrossEntropy
- Optimizers:
　・AdaDelta
　・AdaGrad
　・Adam
　・MomentumSGD
　・RMSprop
　・SGD
- Others:
　・DropOut
　・BatchNormalization
 
 
 最後に、このライブラリが誰かの学習の助けになれば幸いです
