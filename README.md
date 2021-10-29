
# An introduction to PySpark
### Level: Beginner
### [Presentation](https://docs.google.com/presentation/d/1UsU5pERa6HbD_qgXgt0kP5c9XZx90CNIBuGoTDgNeVQ/edit?usp=sharing)

## Project description
PySpark is a distributed data processing engine widely used in Data Engineering and Data Science. Another way to think of PySpark is a library that allows processing large amounts of data on a single machine or a cluster of machines. We will go through the basic concepts and operations so you will leave the workshop ready to continue learning on your own.

## Setup:
 
To set up your environment, create an account at https://community.cloud.databricks.com/

Then import the [notebook](https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/583179271718016/1249435828050903/222117274820398/latest.html) like on the gif:

![](workshop/pictures/databricks_setup.gif)

Upload the file on `workshop/SalesRecords.csv`:

![](workshop/pictures/databricks_upload.gif)
(There is no need to create a table after uploading a file)

You should be good to go back and start running your notebook now :)

Pro tip: run a cell with `Shift + Enter`

## Requirements
Create a trial account on https://community.cloud.databricks.com/

## Usage
* Clone the repository
* Follow the instructions to set up your notebook

## Credits
This workshop was set up by @pyladiesams and https://github.com/nataliapipas

## Option B

If, for some reason, Databricks is not available, we'll use a Zepl notebook.

Go to `My Notebooks` on your account on https://www.zepl.com/

![](workshop/pictures/your-notebooks.png)

Click `Import` in the top right corner of the page

![](workshop/pictures/import.png)

Name your notebook and use `Upload file` to import the file on `workshop/pyspark.zpln`
(it can also be found [here](https://www.zepl.com/viewer/notebooks/bm90ZTovL25hdGFsaWFwaXBhc0BnbWFpbC5jb20vZjNkNDgwZjFlNzA4NDc2NTkzZjAxMzQwOThlZWE0MTcvbm90ZS5qc29u)).

![](workshop/pictures/zpl.png)

On the notebook page, click the folder icon on the left and select `Upload file`

![](workshop/pictures/upload.png)

Upload the file on `workshop/SalesRecords.csv`

You should be good to start running your notebook now :)

(Pro tip: run a cell with `Shift + Enter`)

## Option C

Wow, have we really reached plan C? Alright, let's go local. Use this method if you don't have java installed on your computer.

Use docker if you don't have spark installed on your computer.

cd where the docker-compose.yml file is.

In the terminal, run the command `docker-compose up` which will automatically start building the image.

Click the link which can also be reached with `localhost:8888`

Type in the password `pyspark`

When you're done, close everything down by typing `docker-compose down -v` in the terminal.

## Option D

Alright, if your not comfortable with docker you can do this instead.

Requirements: Python 3 installed

Steps:

1) Create and activate a virtual environment with

```
python3 -m venv venv
source venv/bin/activate
```

Install the requirements with

```
pip install -r workshop/requirements.txt
```

Make your virtual environment available on Jupyter with

```
python -m ipykernel install --user --name=venv
```

Start your notebook with

```
jupyter-lab workshop/notebook.ipynb
```
