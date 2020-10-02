# mol_finder
Project for finding synthesizable molecules with multiple properties.


## Install Dependencies

#### Install chemprop

    cd ..
    git clone https://github.com/chemprop/chemprop.git
    cd chemprop
    conda env create -f environment.yml -n molopt
    conda activate molopt
    pip install -e .
    cd ../mol_finder
    
#### Install multiobj-rationale

    cd ..
    git clone git@github.com:anonymous20201002/multiobj-rationale.git
    cd multiobj-rationale
    pip install -e .
    cd ../mol_finder
    
#### Install Other Env
    pip intstall -r requirements.txt
    

## Example to Run
    export CUDA_VISIBLE_DEVICES=0
    export TF_CPP_MIN_LOG_LEVEL=2
    export PYTHONPATH=$PWD
    python mol_finder/main.py --rounds=10 --epoch=1