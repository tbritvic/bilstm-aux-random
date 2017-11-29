bi-LSTM tagger with auxiliary task and random as a not known tags handling method

Tagger is created as an extention of a Bidirectional Long-Short Term Memory tagger: https://github.com/bplank/bilstm-aux
and a paper: http://arxiv.org/abs/1604.05529

Requirements: 
    python3
    DyNet 2.0

Installation: as in https://github.com/bplank/bilstm-aux

Training the tagger:

python src/bilty.py --dynet-mem 3500 --train new_data/da-train.conllu new_data/da-train-aux.conllu --test new_data/da-test.conllu --dev new_data/da-dev.conllu --iters 10 --pred_layer 2 --h_layer 2 --vocabulary_filename new_data/dictionaries/da.dic.clean

Embeddings

The Polyglot embeddings (Al-Rfou et al., 2013) can be downloaded from: http://www.let.rug.nl
