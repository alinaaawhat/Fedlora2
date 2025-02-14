
## Requirments
Install all the packages from requirments.txt
*pip install -r requirements.txt
*git clone https://github.com/EleutherAI/lm-evaluation-harness
*cd lm-evaluation-harness
*pip install -e .

## Data
*The training dataset of WizardLLM has already been downloaded and split in ./data_wiz/ fold.
*If you want to use your dataset, use the same format as ./data_wiz/.

## Running the experiments
* To run the FLoRA algorithm (--stacking: True) and FedIT (--stacking False) in a homogeneous LoRA setting:
```
*python main.py --global_model '***  "./data_wiz" --output_dir '***' --num_communication_rounds 3 --local_num_epochs 1 --stacking True
