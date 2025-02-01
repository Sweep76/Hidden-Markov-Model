# Hidden-Markov-Model
 Statistical model that represents a system with hidden states and observable outputs

# Hidden Markov Model

## Structure

```sh
.
├── bigdata
│   ├── dev.conll
│   ├── test.conll
│   └── train.conll
├── data
│   ├── dev.conll
│   └── train.conll
├── results
│   ├── bhmm.txt
│   └── hmm.txt
├── config.py
├── hmm.py
├── README.md
└── run.py
```

## Usage

```sh
$ python run.py -h
usage: run.py [-h] [--bigdata] [--file FILE]

Create Hidden Markov Model(HMM) for POS Tagging.

optional arguments:
  -h, --help            show this help message and exit
  --bigdata, -b         use big data
  --file FILE, -f FILE  set where to store the model
# e.g. 
$ python run.py -b
```

## Results

| Big Data Set | Alpha |  dev/P   |  test/P  |     mT(s)      |
| :----------: | :---: | :------: | :------: | :------------: |
|      No      |  0.3  | 75.7428% |    *     | 0:00:00.723058 |
|      Yes     | 0.01  | 88.3546% | 88.4994% | 0:00:02.846564 |