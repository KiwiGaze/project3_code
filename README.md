
## Exploring In-Context Learning Capabilities of Transformer Models



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

3. For Shift in Data Distribution part, you can run data_distribution.ipynb for simplicity. To use .ipynb You should clone our github repo to your own Github repo, and the reposity could be 'project3_code' if you clone the whole repo as your repo. Remember to change other code here to your own github profile.
    ```
    username = 'Your_github_name'
    git_token = 'your_github_token'
    repository = 'where_you_store_our_github_repository'
    !git clone https://{git_token}@github.com/{username}/{repository}
    ```
    
