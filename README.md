# dm_count

해당 내용은 2021년 2학기 컴퓨터비전에서 사용하는 군중 계산 관련 데이터입니다.

데이터셋은 data 폴더 내에 있으며, 해당 데이터에 문제가 있을 경우 다운받아 Part A만 사용하시기 바랍니다.

링크 주소 : https://www.kaggle.com/tthien/shanghaitech

## Process
train -> test -> val 로 진행하며, 최종 val을 통해 result 폴더의 submission.csv로 저장하게 됩니다.

1. train
```
python train.py --dataset sha --data-dir <path to dataset> --device <gpu device id>
```

2. test
```
python test.py --model-path <path of the model to be evaluated> --data-path <directory for the dataset> --dataset sha
```

3. val
```
python val.py --model-path <path of the model to be evaluated>
```

## References
If you find this work or code useful, please cite:

```
@inproceedings{wang2020DMCount,
  title={Distribution Matching for Crowd Counting},
  author={Boyu Wang and Huidong Liu and Dimitris Samaras and Minh Hoai},
  booktitle={Advances in Neural Information Processing Systems},
  year={2020},
}
```
