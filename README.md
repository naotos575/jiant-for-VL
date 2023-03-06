# jiant-for-VL
これはjiantをベースにVisualBERTとLXMERTの言語的知識を分析できるようにしたレポジトリです。

## Getting Started
言語知識に関するデータセットは./probing/dataのスクリプトから取得してください。ただし、データセットは一部有料のため、本レポジトリでは共有できません。


## Running
depok.ymlと同じ環境を用意してください。

実行例

>nohup python main.py --config_file  jiant/config/edgeprobe/edgeprobe_bert.conf -o "exp_name=lxmert-mix_12-edges-rel-semeval, run_name=run, target_tasks=edges-rel-semeval, input_module=lxmert, transformers_output_mode=mix, transformers_max_layer=12" &

target_tasksには分類タスク、input_moduleにbert, visualbert,lxmertから選択してください。

## Acknowledgments
このモデルはjiantをベースに使用したものです。下記のレポジトリーを参照してください。

- https://github.com/nyu-mll/jiant-v1-legacy#
