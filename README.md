# Python for Data Science -- Iowa City Meetups
Python for Data Science Tutorials used at Meetups in Iowa City

Welcome to my github repo! This is where all of the IPython Notebooks and datasets we use in Data Science Meetups will be housed. Please feel free to email me questions or comments to ross [at] coconicdata.com!

## Prerequisites
### 1) Please have Python installed on your computer.
We will be using Python 3 in this course, so I recommend you work in Python 3 as well. (3.5 or 3.6 are both fine)

Bonus points if you can work with virtual environments in Python (For beginners, Anaconda makes this very easy, please see below).

### 2) Please sign up for an AWS account at aws.amazon.com
Non-students: https://portal.aws.amazon.com/billing/signup#/start

Students: https://aws.amazon.com/education/awseducate/

It can take up to 24-hours for your account to be fully setup. If you are a student, you can get free credits by signing up through the AWS Educate link above. You will save time if you sign up ahead of time.

In our first Meetup, we will use AWS to create a free MySQL database that we will use for testing.  In later meetups, we will also utilize free EC2 cloud instances to do modeling and data processing exercises in the cloud (as most people do in the real world). We may also explore Google Cloud for Machine Learning Pipelines.

### OPTIONAL: If you're a beginner, I recommend starting with an Anaconda installation.
Please utilize the links below depending on your operating system.
#### MacOS
https://www.datacamp.com/community/tutorials/installing-anaconda-mac-os-x
#### Linux
https://www.digitalocean.com/community/tutorials/how-to-install-the-anaconda-python-distribution-on-ubuntu-16-04
#### Windows
https://pythonforundergradengineers.com/installing-anaconda-on-windows.html

## Meetup 1: Manipulating Data with Pandas + SQL and Working with REST APIs in Python
We'll be working in Jupyter Notebooks with the Quandl API. Please sign up for a *free* API Key at https://www.quandl.com/

If you have Anaconda, start by creating a virtual environment for this Meetup. 
A virtual environment is just a walled garden for your Python so that none of the packages you install conflict with each other.

I have named my environment `data_science1`, but you can name it whatever you want. Just be sure to use the same name in the code below each time.

On the command line:

```bash
conda create --name data_science1 python=3.6
```
Then type `y` and press return/enter

Now, activate your environment (also command line):

```bash
source activate data_science1
```

All of the Data Science Meetups I run will use Jupyter Notebooks to make it easy to play around with your code.
To install jupyter notebooks and add your new python kernel to the options for those jupyter notebooks, run the code below on your command line.
```bash
pip install jupyter notebook
python -m ipykernel install --user --name data_science1 --display-name "Python 3.6 (data_science1)"
```
Install the additional packages needed for this meetup via the command line. Please note that the `-y` just prevents Anaconda from asking you to confirm.
```bash
conda install -y requests
conda install -y pandas
conda install -y pymysql
conda install -y ggplot
conda install -y sqlalchemy
```
You can run the following on the command line to deactivate your Anaconda virtual environment: `source deactivate`

That should do it!
When the time comes to start our journey, just go to your command line, and run:
```bash
jupyter notebook
```
I will walk you through the remaining steps during the Meetup.
