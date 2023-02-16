1. connect to bluemoon
2. Install conda
    1. `wget -c [https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh](https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh)`
    2. `sh Miniconda3-latest-Linux-x86_64.sh`
        1. Anaconda takes a long time so we use miniconda
3. Create conda env (dld)
    1. `conda create -n dld python=3.6`
    2. `conda activate dld`
    3. `pip install tensorflow-gpu==1.14 scipy==1.3.3 requests==2.22.0 Pillow==6.2.1 wandb`  
        1. (This takes a while)
4. Change dnn
    1. `cmd = 'nvcc --std=c++11 -DNDEBUG' + opts.strip()`
