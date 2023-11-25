
## Coding Standards

https://github.com/qbrilliance/software-development-handbook/blob/main/coding_standards.md

## Install qbrilliance

```bash

# [Remark] Missing but required for qbrilliance
# Read-the-doc and README.md are inconsistent
sudo apt install build-essential cmake gfortran libboost-all-dev libcurl4-openssl-dev libssl-dev libopenblas-dev libpython3-dev python3 python3-pip

# Steps in read-the-docs
# https://qristal.readthedocs.io/en/latest/rst/getting_started.html#
git clone https://github.com/qbrilliance/qristal.git qristal
cd qristal
mkdir build && cd build
cmake .. -DINSTALL_MISSING=ON
make install

```

