# 3rd Project TEAM 2

## AIRFLOW 

### Pipeline
![image](https://github.com/user-attachments/assets/81b1f0f0-e69f-497c-b1ab-cf5f83db8bbd)
1. get_db : DB에서 예측할 데이터에 대한 정보를 가져온다.
2. task.branch : 예측할 데이터가 있는지 체크
```
if 예측할 데이터가 있으면
    => 다음 task 진행 (go to task_pred)
else
    => pipeline 종료 (go to task_end)
```
3. predict : 모델을 이용하여 얼굴 나이 예측 진행
> 가상환경 생성, Dependency 설치, 모델 load 등 소요시간이 길어 가상환경을 cache하였음
4. save.log : 예측한 정보 log파일로 저장
```bash
$ tail -n 1 pred.log
82,2,2024-10-08 16:33:21     # num, pred_rst, pred_dt
```

### Dependency
![airflow](https://img.shields.io/badge/apache--airflow-017CEE.svg?style=for-the-badge&logo=apacheairflow&logoColor=FFFFFF)
![transformers](https://img.shields.io/badge/transformers-FFD21E.svg?style=for-the-badge&logo=huggingface&logoColor=000000)
![torch](https://img.shields.io/badge/pytorch-EE4C2C.svg?style=for-the-badge&logo=pytorch&logoColor=FFFFFF)
![requests](https://img.shields.io/badge/python-3776AB.svg?style=for-the-badge&logo=python&logoColor=FFFFFF)
![pillow](https://img.shields.io/badge/python-3776AB.svg?style=for-the-badge&logo=python&logoColor=FFFFFF)
