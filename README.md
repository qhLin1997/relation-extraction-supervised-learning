## Data
* [SemEval2010 Task8](https://drive.google.com/file/d/0B_jQiLugGTAkMDQ5ZjZiMTUtMzQ1Yy00YWNmLWJlZDYtOWY1ZDMwY2U4YjFk/view?sort=name&layout=list&num=50)
* [Google News - Mikolov et
al.(2010)](https://code.google.com/archive/p/word2vec/)

## Usage
1. 
1. Download the embedding and put it in the `embedding` folder.
2. Run `convert.py`
```shell
python3 convert.py
```
2. Run the following the commands to start the program.
```shell
python run.py
```
More details can be seen by `python run.py -h`.

3. You can use the official scorer to check the final predicted result.
```shell
perl semeval2010_task8_scorer-v1.2.pl proposed_answer.txt predicted_result.txt >> result.txt
```

## Result
The result of my version and that in paper are present as follows:
| paper | my version |
| :------: | :------: |
| 0.843 | 0.8156 |

The training log can be seen in `train.log` and the official evaluation results is available in `result.txt`.

*Note*:
* Some settings are different from those mentioned in the paper.
* No validation set used during training.
* Just complete the part of general *Attention-CNN*. WordNet and words around nominals are not used. More details are available in Section 4 in this paper.
* Although I try to set random seeds, it seems that the results of each run are a little different.
* The result of my version is not ideal. Maybe my understanding is wrong. If you find it, please let me know.

## Reference Link
