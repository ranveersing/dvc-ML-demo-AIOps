git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/USER_NAME/REPO_NAME.git
git push -u origin main

conda create -n dvc-ml python=3.7 -y
conda activate dvc-ml


https://github.com/c17hawke/dvc-ML-demo-AIOps

touch requirements.txt
pip install -r requirements.txt


dvc init

mkdir -p src/utils

http://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/winequality-red.csv


from setuptools import setup

with open("README.md", "r", encoding="utf-8") as f:
    long_description = f.read()

setup(
    name="src",
    version="0.0.1",
    author="ranveer",
    description="A small package for dvc ml pipeline demo",
    long_description=long_description,
    long_description_content_type="text/markdown",
    url="https://github.com/ranveersing/dvc-ML-demo-AIOps",
    author_email="ranveersing@gmail.com",
    packages=["src"],
    python_requires=">=3.7",
    install_requires=[
        'dvc',
        'pandas',
        'scikit-learn'
    ]
)



data_source: http://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/winequality-red.csv

artifacts: 
  artifacts_dir: artifacts
  raw_local_dir: raw_local_dir
  raw_local_file: data.csv