

## 1. Download the models

```shell
cd gpt-2
python3 download_model.py 117M
# python3 download_model.py 345M
# python3 download_model.py 774M
# python3 download_model.py 1558M
```

The download models will be stored in `gpt-2/models/`.
If you've already download the models beforehand, then just link the models to `gpt-2/models/`:

```shell
cd gpt-2
ln -s /path/to/your/downloaded/models ./models
cd models
ls
117M 345M 774M 1558M
```

## 2. Run the example

```shell  
cd gpt-2
python3 src/interactive_conditional_samples.py --model_name 117M --top_k 40 --length 256
#python3 src/interactive_conditional_samples.py --model_name 345M --top_k 40 --length 256
#python3 src/interactive_conditional_samples.py --model_name 774M --top_k 40 --length 256
#python3 src/interactive_conditional_samples.py --model_name 1558M --top_k 40 --length 256
```



