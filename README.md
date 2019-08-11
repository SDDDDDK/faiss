# faiss
faissの使い方まとめ。Qiitaで手順を紹介して、Githubではパラメータなどの説明をしています。

- 公式：https://github.com/facebookresearch/faiss
- 公式チュートリアル：https://github.com/facebookresearch/faiss/wiki/Getting-started

## Qiita解説記事
- k-NN: 
- k-Means: 

## Install
#### cudaのバージョンチェック
```
cat /usr/local/cuda/version.txt
```

### anacondaでインストール
- [ここ](https://github.com/facebookresearch/faiss/blob/master/INSTALL.md)の通りに

### Colaboratory上でインストール(cuda 9.2)
Driveをマウントしたあと…

- ダウンロード（一度ダウンロードすればこの2行は実行しなくて良い）
```
!wget https://anaconda.org/pytorch/faiss-gpu/1.4.0/download/linux-64/faiss-gpu-1.4.0-py36_cuda9.2.148_1.tar.bz2
!tar xvjf faiss-gpu-1.4.0-py36_cuda9.2.148_1.tar.bz2
```
（リンクは[ここ](https://anaconda.org/pytorch/faiss-gpu/files)から選択

- インストール（毎回必要）
```
!cp -r lib/python3.6/site-packages/* /usr/local/lib/python3.6/dist-packages/
!pip install mkl
```