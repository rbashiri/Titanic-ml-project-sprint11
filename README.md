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