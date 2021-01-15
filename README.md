# RDN

This repository is implementation of the ["Residual Dense Network for Image Super-Resolution"](https://arxiv.org/abs/1802.08797).


## Requirements

- PyTorch 1.0.0
- Numpy 1.15.4
- Pillow 5.4.1
- h5py 2.8.0
- tqdm 4.30.0

## Train

The DIV2K, Set5 dataset converted to HDF5 can be downloaded from the links below.

| Dataset | Scale | Type | Link |
|---------|-------|------|------|
| DIV2K | 2 | Train | [Download](https://www.dropbox.com/s/41sn4eie37hp6rh/DIV2K_x2.h5?dl=0) |
| DIV2K | 3 | Train | [Download](https://www.dropbox.com/s/4piy2lvhrjb2e54/DIV2K_x3.h5?dl=0) |
| DIV2K | 4 | Train | [Download](https://www.dropbox.com/s/ie4a6t7f9n5lgco/DIV2K_x4.h5?dl=0) |
| Set5 | 2 | Eval | [Download](https://www.dropbox.com/s/b7v5vis8duh9vwd/Set5_x2.h5?dl=0) |
| Set5 | 3 | Eval | [Download](https://www.dropbox.com/s/768b07ncpdfmgs6/Set5_x3.h5?dl=0) |
| Set5 | 4 | Eval | [Download](https://www.dropbox.com/s/rtu89xyatbb71qv/Set5_x4.h5?dl=0) |


## Test

Pre-trained weights can be downloaded from the links below.

| Model | Scale | Link |
|-------|-------|------|
| RDN (D=16, C=8, G=64, G0=64) | 2 | [Download](https://www.dropbox.com/s/pd52pkmaik1ri0h/rdn_x2.pth?dl=0) |
| RDN (D=16, C=8, G=64, G0=64) | 3 | [Download](https://www.dropbox.com/s/56topxdwm6rakwd/rdn_x3.pth?dl=0) |
| RDN (D=16, C=8, G=64, G0=64) | 4 | [Download](https://www.dropbox.com/s/yphiyivb1v7jya2/rdn_x4.pth?dl=0) |


## Results

PSNR was calculated on the Y channel.

### Set5

| Eval. Mat | Scale | RDN (Paper) | RDN (Ours) |
|-----------|-------|-------|-----------------|
| PSNR | 2 | 38.24 | 38.18 |
| PSNR | 3 | 34.71 | 34.73 |
| PSNR | 4 | 32.47 | 32.40 |

