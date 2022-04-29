# child-electra


1. Download the AO-Childize dataset.

``` 
The dataset and respective vocab are already present in the repo.
```

2. Tokenize dataset.

```bash
$ python pretraining/openwebtext/preprocess.py
```

3. Pre-train.

```bash
$ python pretraining/openwebtext/pretrain.py
```

4. Download GLUE dataset.

```bash
$ python examples/glue/download.py 
```

5. Fine-tune on the MRPC sub-task of the GLUE benchmark.

```bash
$ python examples/glue/run.py --model_name_or_path output/yyyy-mm-dd-hh-mm-ss/ckpt/200000
```


## Released Models

We are initially releasing three pre-trained models:

| Model | Layers | Hidden Size | Params | GLUE score (test set) | Download |
| --- | --- | --- | --- | ---  | --- |
| ELECTRA-1 | 12 | 256 | 14M |  | [link]() |
| ELECTRA-2 | 10 | 256 | 110M |  | [link]() |
| ELECTRA-3 |  8 | 256 | 335M |   | [link]() |


| Model | Layers | Hidden Size | Params | GLUE score (test set) | Download |
| --- | --- | --- | --- | ---  | --- |
| ELECTRA-1 | 12 | 256 | 14M |  | [link]() |
| ELECTRA-2 | 12 | 128 | 110M |  | [link]() |
| ELECTRA-3 |  12| 64 | 335M |   | [link]() |


| Model | Attention Head | Layers | Hidden Size | Params | GLUE score (test set) | Download |
| --- | --- | --- | --- | --- | ---  | --- |
| ELECTRA-1 |4 | 12 | 256 | 14M |  | [link]() |
| ELECTRA-2 | 2|12 | 256 | 110M |  | [link]() |

