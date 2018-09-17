# python-for-data-science
Python for Data Science Tutorials used at Meetups in Iowa City

Welcome to my github repo! This is where all of the IPython Notebooks and datasets we use in Data Science Meetups will be housed. Please feel free to email me questions or comments to ross [at] coconicdata.com!

## Prerequisites
#### Please have Python installed on your computer.
We will be using Python 3 in this course, so I recommend you work in Python 3 as well. (3.5 or 3.6 are both fine)

Bonus points if you can work with virtual environments in Python (Anaconda makes this very easy, see below).

#### If you're a beginner, I recommend starting with an Anaconda installation.
### MacOS
https://www.datacamp.com/community/tutorials/installing-anaconda-mac-os-x
### Linux
https://www.digitalocean.com/community/tutorials/how-to-install-the-anaconda-python-distribution-on-ubuntu-16-04
### Windows
https://pythonforundergradengineers.com/installing-anaconda-on-windows.html

## Meetup 1: Manipulating Data and Working with APIs
If you have Anaconda, start by creating a virtual environment for this tutorial. 

I have named my environment `data_science1`, but you can name it whatever you want. Just be sure to keep it working below.

```bash
conda create --name data_science1 python=3.6
```
Then type `y` and `enter`

A virtual environment is just a walled garden for your Python so that none of the packages you install conflict with each other.

Now, activate your environment:

```bash
conda activate data_science1
```

All of the Data Science Meetups I run will use Jupyter Notebooks to make it easy to play around with your code.
To install jupyter notebooks and add your new python kernel to the options for those jupyter notebooks, run the code below.
```bash
pip install jupyter notebook
python -m ipykernel install --user --name data_science1 --display-name "Python 3.6 (data_science1)"
```
Install the additional packages needed for this tutorial. Please note that the `-y` just prevents Anaconda from asking you to confirm.
```bash
conda install -y requests
conda install -y pandas
conda install -y pymysql
conda install -y ggplot
conda install -y sqlalchemy
```
You can run the following to deactivate your Anaconda virtual environment: `source deactivate`

That should do it!
When the time comes to start our course, just go to your command line, and run:
```bash
jupyter notebook
```
I will walk you through the remaining steps during the Meetup.
