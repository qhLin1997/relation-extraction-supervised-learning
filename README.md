## Data
* [SemEval2010 Task8](https://drive.google.com/file/d/0B_jQiLugGTAkMDQ5ZjZiMTUtMzQ1Yy00YWNmLWJlZDYtOWY1ZDMwY2U4YjFk/view?sort=name&layout=list&num=50)
* [Google News - Mikolov et
al.(2010)](https://code.google.com/archive/p/word2vec/)

## Usage
1. Download and unzip data and put it in the folder `data`.
2. Run `preprocess.py`
```shell
python3 preprocess.py
```
3. Download and unzip word embedding and put it in the folder `embedding`.
4. Run `convert.py`
```shell
python3 convert.py
```
5. Run `run.py` to train and test the model.
```shell
python2 run.py
```
6. Use the official scorer to check the final predicted result.
```shell
perl semeval2010_task8_scorer-v1.2.pl proposed_answer.txt predicted_result.txt >> result.txt
```
7. Predicted labels are in the file `predicted_result.txt`.
8. The official evaluation results is available in `result.txt`.
