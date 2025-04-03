[![DOI](https://zenodo.org/badge/779008229.svg)](https://zenodo.org/doi/10.5281/zenodo.10892431)

# LLMCompass

## Installation

### If using Github
```bash
$ git clone -b main https://github.com/MrTang-Yuhan/LLMCompass.git
$ cd LLMCompass
$ git submodule init
$ git submodule update --recursive
```

### Set up the environment（法1）

```bash
$ conda create -n llmcompass_ae python=3.9
$ conda activate llmcompass_ae
$ pip3 install scalesim==2.0.2
$ conda install pytorch==2.0.0 -c pytorch
$ pip3 install matplotlib==3.9.4
$ pip3 install seaborn==0.13.2
$ pip3 install scipy==1.13.1
# 删除numpy到干净为止
$ pip3 uninstall numpy
$ pip3 uninstall numpy
$ pip3 install numpy==1.25.1
```
### Set up the environment（法2）（需要几分钟时间）
```bash
conda env create -f  ./environment.yaml
```

## AE Experiment workflow
```bash
# Figure 5 (around 100 min) 
$ cd ae/figure5
$ bash run_figure5.sh 

# Figure 6 (around 1 min)
$ cd ae/figure6
$ bash run_figure6.sh

# Figure 7 (around 20 min)
$ cd ae/figure7
$ bash run_figure7.sh

# Figure 8 (around 40 min)
$ cd ae/figure8
$ bash run_figure8.sh

# Figure 9 (around 30 min)
$ cd ae/figure9
$ bash run_figure9.sh

# Figure 10 (around 45 min)
$ cd ae/figure10
$ bash run_figure10.sh

# Figure 11 (around 5 min) 
$ cd ae/figure11
$ bash run_figure11.sh

# Figure 12 (around 4 hours) 
$ cd ae/figure12
$ bash run_figure12.sh
```

## AE Expected result

After running each script above, the corresponding figures
will be generated under the corresponding directory as suggested by its name.

For comparison, a copy of the expected results can be found in `ae\expected_results`


## User Guide

A guide on "How to Run a LLMCompass Simulation" is shown [here](./docs/run.md).
