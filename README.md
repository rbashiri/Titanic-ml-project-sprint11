## Project Structure

```text
titanic-ml-project/
├── training/
│   ├── Dockerfile
│   ├── requirements.txt
│   ├── train_model.py
│   └── data/
│       └── titanic.csv
├── serving/
│   ├── Dockerfile
│   ├── requirements.txt
│   ├── app.py
│   └── models/
├── notebooks/
│   └── expolration.ipynb
├── .gitignore
└── README.md
```
```text
Project Overview
We will:

1- Set up a training environment
2- Explore and clean the Titanic dataset
3- Train a simple classification model
4- Save the model and preprocessing artifacts
5- Create a FastAPI serving application
6- Build a Docker container
7- Test the container locally
8- Push to DockerHub
9- Document your work for others
10-Submit the link to your project on DockerHub for review
```

Data Dictionary

| Variable | Definition | Key |
| --- | --- | --- |
| survival | Survival | 0 = No, 1 = Yes |
| pclass | Ticket class | 1 = 1st, 2 = 2nd, 3 = 3rd |
| sex | Sex |  |
| age | Age in years |  |
| sibsp | # of siblings / spouses aboard the Titanic |  |
| parch | # of parents / children aboard the Titanic |  |
| ticket | Ticket number |  |
| fare | Passenger fare |  |
| cabin | Cabin number |  |
| embarked | Port of Embarkation | C = Cherbourg, Q = Queenstown, S = Southampton |

Variable Notes

**pclass**: A proxy for socio-economic status (SES)

1st = Upper

2nd = Middle

3rd = Lower

**age**: Age is fractional if less than 1. If the age is estimated, it is in the form of xx.5

**sibsp**: The dataset defines family relations in this way...

Sibling = brother, sister, stepbrother, stepsister

Spouse = husband, wife (mistresses and fiancés were ignored)

**parch**: The dataset defines family relations in this way...

Parent = mother, father

Child = daughter, son, stepdaughter, stepson

Some children travelled only with a nanny, therefore parch=0 for them.

Predict survival on the Titanic and get familiar with ML basics