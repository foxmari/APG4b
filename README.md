# APG4b
https://atcoder.jp/contests/APG4b


# Jupyternotebook　for cpp
Clingを用いる 

*anacondaを使う場合
https://github.com/jupyter-xeus/xeus-cling
conda install xeus-cling -c conda-forge

*anaconda ない場合
https://root.cern.ch/download/cling/  
サイトからバイナリを落とす（自分の環境はubuntu16なのでそれっぽい名前のバイナリ落としてきた）  
 
展開して、適当な位置に置き、動作確認をする   
```
$ ./tool/cling_2020-11-05_ROOT-ubuntu16/bin/cling  

****************** CLING ******************
* Type C++ code and press enter to run it *
*             Type .q to exit             *
*******************************************
[cling]$ 
```
動作確認できたらPathを通しておく。  

おわったらJupyterlabから呼び出せるようにする
```
$ cd ./tool/cling_2020-11-05_ROOT-ubuntu16/share/cling/Jupyter/kernel
$ sudo pip3 install -e .
$ jupyter-kernelspec install --user cling-cpp11
# ちなみに１１、１４、１７など好きなの選べる

```
