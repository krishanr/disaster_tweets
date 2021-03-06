## Intro

A well structured data science project using docker and docker-compose for the nlp-challenge Kaggle competition, with the objective of coming up with a high performing disaster tweet predictor from twitter data.

## Installation

With Docker 19.03+, nivida-container-toolkit 1.2.0, and GPUs installed, start jupyter with:

```bash
$ docker-compose up jupyter
```

Once the kaggle.json is added to the folder "~/.kaggle" and your Kaggle nlp-challenge data agreements have been accepted, navigate to the only notebook in "notebooks" and run it.

## Conclusion

Our fine-tuned BERT model obtained an accuracy of 0.83 and the following classification report on the test set with 762 samples:

```
            precision    recall  f1-score

        0       0.84      0.89      0.86
        1       0.83      0.77      0.80

accuracy                            0.83
macro avg       0.83      0.83      0.83
```

Our model recalled 77% of disaster tweets with a precision of 83%.

Here are some falsely predicted disaster tweets, do you think you can do better?

tweet 1 :'burned 129 calories doing 24 minutes of Walking 3.5 mph brisk pace #myfitnesspal',

tweet 2: 'Sound judgement by MPC - premature rises could derail recovery #Business http://t.co/fvLgU1naYr',

tweet 3: 'We The Free Hailstorm Maxi http://t.co/ERWs6IELdG',

tweet 4: 'U.S National Park Services Tonto National Forest: Stop the Annihilation of the Salt River Wild Horse... http://t.co/KPQk0C4G0M via @Change'