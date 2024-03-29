
## Exploring In-Context Learning Capabilities of Transformer Models



## Setup

1. Install the dependencies using Conda. 

    ```
    conda env create -f environment.yml
    conda activate in-context-learning
    ```

2. For Shift in Data Distribution Part. Compare transformers to OLS and ridge. For training a transformer, we use the code here https://github.com/dtsip/in-context-learning. Once transformer are trained, specify the paths to their respective checkpoints in the YAML file (comparison_mlp_txformer.yaml) and run.

   
    Run the following for no shift without noise:
    ```
    python Comparisons_final.py --config confs/comparison_mlp_txformer.yaml
    ```
    Run the following for mild shift without noise:
    ```
    python Comparisons_final_m_2.py --config confs/comparison_mlp_txformer.yaml
    ```
    Run the following for severe shift without noise:
    ```
    python Comparisons_final_m_4.py --config confs/comparison_mlp_txformer.yaml
    ```
    Run the following for no shift with noise:
    ```
    python noised_Comparisons_final.py --config confs/comparison_mlp_txformer.yaml
    ```
    Run the following for mild shift with noise:
    ```
    python noised_Comparisons_final_m_2.py --config confs/comparison_mlp_txformer.yaml
    ```
    Run the following for severe shift with noise:
    ```
    python noised_Comparisons_final_m_4.py --config confs/comparison_mlp_txformer.yaml
    ```
4. For Shift in Data Distribution part, you can run data_distribution.ipynb for simplicity. Please open /Data_Distribution for more information.
    
