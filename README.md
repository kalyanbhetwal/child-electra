# child-electra


1. Download the AO-Childize dataset.

``` The dataset and respective vocab are already present in the repo.

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
