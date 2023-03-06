# jiant-for-VL
This is a repository based on [jiant](https://github.com/nyu-mll/jiant-v1-legacy#) that allows analysis of the linguistic knowledge of VisualBERT and LXMERT.Please refer to the previous study 'jiant' for the basics of usage.

## Getting Started
Datasets on language knowledge are available in . /probing/data from the script. However, some datasets are paid for and cannot be shared in this repository.


## Running
Prepare the same environment as in depok.yml.

### Execution example

>nohup python main.py --config_file  jiant/config/edgeprobe/edgeprobe_bert.conf -o "exp_name=lxmert-mix_12-edges-rel-semeval, run_name=run, target_tasks=edges-rel-semeval, input_module=lxmert, transformers_output_mode=mix, transformers_max_layer=12" &

Choose a classification task for target_tasks and bert, visualbert, or lxmert for input_module.

## Acknowledgments
This model is based on jiant. See repositories below.

- https://github.com/nyu-mll/jiant-v1-legacy#
