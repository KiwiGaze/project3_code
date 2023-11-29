
## [A Closer Look at In-Context Learning under Distribution Shifts](https://arxiv.org/abs/2305.16704)



## Setup

1. Install the dependencies using Conda. 

    ```
    conda env create -f environment.yml
    conda activate in-context-learning
    ```

2. Compare transformers to OLS and tidge. For training a transformer, we use the code here https://github.com/dtsip/in-context-learning. Once transformer are trained, specify the paths to their respective checkpoints in the YAML file (comparison_mlp_txformer.yaml) and run.

    ```
    python Comparisons_final.py --config confs/comparison_mlp_txformer.yaml
    ```

3. For Shift in Data Distribution part, you can run data_distribution.ipynb for simplicity.
    ```
    python Comparisons_final.py --config confs/comparison_mlp_txformer.yaml
    ```
    
