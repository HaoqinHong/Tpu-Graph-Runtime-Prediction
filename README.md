
```sh
conda create -n tpugraphs python=3.10
conda activate tpugraphs

conda install -c conda-forge tensorflow
conda install -c conda-forge tqdm

pip install tensorflow_gnn --pre
pip install tensorflow-ranking
conda clean --all
```

python tiles_train.py --model=EarlyJoinSAGE



# On xla:random
python layout_train.py --source xla --search random --epochs 10 --max_configs 1000

# On xla:default
python layout_train.py --source xla --search default --epochs 10 --max_configs 1000

# On nlp:random
python layout_train.py --source nlp --search random --epochs 10 --max_configs 1000

# On nlp:default
python layout_train.py --source nlp --search default --epochs 10 --max_configs 1000

python combine_csvs.py
