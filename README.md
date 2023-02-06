# CogWear

1) Clone the CogWear repository 
2) Download the pilot and survey gamification data from https://physionet.org/
2) Place pilot.zip and survey_gamification.zip in the CogWear repository
3) Building an image...
```
docker build -t cogwear .
```
4) Take a look at the data and model loading notebook
```
docker run --rm --gpus all -p 8899:8899 cogwear:latest jupyter notebook --port=8899 --allow-root --no-browser --ip=0.0.0.0
```