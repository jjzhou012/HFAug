# HFAug

This is a python implementation of HFAug, as described in the following:

> [HFAug: Heterogeneous Feature Augmentation for Ponzi Detection in Ethereum]((https://arxiv.org/abs/2204.08916))
> 



## Dependencies

For software configuration, all model are implemented in:

- dgl-cuda10.2  0.8.0
- pytoch  1.10.0
- scikit-learn  1.0.1
- toch-geometric-temporal  0.50.0
- numpy  1.20.3

## Data

In `/data/data_het`, there are data about building heterogeneous graph, and others in `/data` are used in homogeneous graph. 

## Usage

1. Create metapaths with `/data/data_het/dgl_metapath.py` and embedding with `/random_walk/embedding.py`
2. Use *HFAug* in different methods. Use `HFAug_ML.py` for manual feature, `/random_walk/HFAug_RW.py` for embedding and GNNs in `/GNN/{methods}`
3. Repeat and report the best one



## Reference

```
@article{jin2022heterogeneous,
  title={Heterogeneous Feature Augmentation for Ponzi Detection in Ethereum},
  author={Jin, Chengxiang and Jin, Jie and Zhou, Jiajun and Wu, Jiajing and Xuan, Qi},
  journal={IEEE Transactions on Circuits and Systems II: Express Briefs},
  year={2022},
  publisher={IEEE}
}
```