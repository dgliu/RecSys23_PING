## RecSys2023_PING


Experiments codes for the paper:

Dugang Liu, Yuhao Wu, Weixin Li, Xiaolian Zhang, Hao Wang, Qinjuan Yang, Zhong Ming. Pairwise Intent Graph Embedding Learning for Context-Aware Recommendation. To appear in RecSys '23.

**Please cite our RecSys '23 paper if you use our codes. Thanks!**


## Requirement
- python==3.6.9
- tensorflow==1.15.3+nv


## Usage


Our implementation references UEG ([Link](https://github.com/dgliu/KDD22_UEG)) and KGIN ([Link](https://github.com/huangtinglin/Knowledge_Graph_based_Intent_Network)). For different data sets, the command line examples are as follows:

**For Amazon-Book:**

```bash
python PING.py --dataset Amazon-Book --num_gcn_layers 2 --reg 1e-3 --decoder_type FM --adj_norm_type ls --num_negatives 4 --intent_weight 0.7 --test_interval 5 --stop_cnt 10
```

**For LFM:**

```bash
python PING.py --dataset LFM --num_gcn_layers 2 --reg 1e-3 --decoder_type FM --adj_norm_type ls --num_negatives 4 --intent_weight 0.1 --test_interval 5 --stop_cnt 10
```

**For Yelp:**

```bash
python PING.py --dataset Yelp --num_gcn_layers 2 --reg 1e-3 --decoder_type FM --adj_norm_type ls --num_negatives 4 --intent_weight 0.9 --test_interval 5 --stop_cnt 10
```

## 华为的免责声明 (Huawei’s Disclaimer)

This open source project is not an official Huawei product, Huawei is not expected to provide support for this project.

## 
If you have any issues or ideas, feel free to contact us ([dugang.ldg@gmail.com](mailto:dugang.ldg@gmail.com)).