## Data
* [SemEval2010 Task8](https://drive.google.com/file/d/0B_jQiLugGTAkMDQ5ZjZiMTUtMzQ1Yy00YWNmLWJlZDYtOWY1ZDMwY2U4YjFk/view?sort=name&layout=list&num=50)
* [Google News - Mikolov et
al.(2010)](https://code.google.com/archive/p/word2vec/)
* [StanfordCoreNLP](https://stanfordnlp.github.io/CoreNLP/) \[[download](https://nlp.stanford.edu/software/stanford-corenlp-full-2018-10-05.zip)\]

## Usage
1. Download and unzip data and put it in the folder `data`.
2. Download and uzip StanfordCoreNLP and put it in the folder `data`.
3. Run `preprocess.py`
```shell
python3 preprocess.py
```
4. Download and unzip word embedding and put it in the folder `embedding`.
5. Run `convert.py`
```shell
python3 convert.py
```
6. Run `run.py` to train and test the model.
```shell
python2 run.py
```
7. Use the official scorer to check the final predicted result.
```shell
perl semeval2010_task8_scorer-v1.2.pl proposed_answer.txt predicted_result.txt >> result.txt
```
8. Predicted labels are in the file `predicted_result.txt`.
9. The official evaluation results is available in `result.txt`.
