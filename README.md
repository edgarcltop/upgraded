## BottleStack Upgraded
#The application allows for developers share infomation between 2 services alot quicker...
## Usage

```python
layer = BottleStack(
    dim = 256,              # channels in
    fmap_size = 64,         # feature map size
    dim_out = 2048,         # channels out
    proj_factor = 4,        # projection factor
    downsample = True,      # downsample on first layer or not
    heads = 4,              # number of heads
    dim_head = 128,         # dimension per head, defaults to 128
    rel_pos_emb = False,    # use relative positional embedding - uses absolute if False
    activation = nn.ReLU()  # activation throughout the network
)

fmap = torch.randn(2, 256, 64, 64) # feature map from previous resnet block(s)

layer(fmap) # (2, 2048, 32, 32)
```

    archivePrefix = {arXiv},
    primaryClass = {cs.CV}
}
