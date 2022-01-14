# NN

## ***Neural Network***

ISO C++ 17 以降  
mini batch学習実装  
`main.cpp`内で学習データや各パラメータを変更

### Default DATA

人工データ 2ch-4class（lea:学習用，dis:テスト用，二つとも同じデータ）  
教師ラベルは4クラスのOne-hotベクトル列となっている．
(200 samples / 1 class)

- lea_sig.csv
- lea_T_sig.csv

XOR data `comment out`  
　batch_size：1~6

```cpp
 input_datas = { {0,0,0,},{1,0,1},{1,1,1},{1,1,0},{1,0,0},{0,0,1} };
 input_labels = { {0},{0},{1},{0},{1},{1} };
```

筋電データ（4ch）が4動作（背屈，掌屈，尺屈，撓屈）分で1データとなっており，4データ分のファイルがある．  `comment out`  
教師ラベルは4動作に対応した4クラスのOne-hotベクトル列となっている．  
(about 6000 samples / 1 class)
- input1.txt
  -- label1.txt
- input2.txt
  -- label2.txt
- input3.txt
  -- label3.txt
- input4.txt
  -- label4.txt