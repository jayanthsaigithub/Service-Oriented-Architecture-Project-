# InNews🇮🇳: News Summarizer App

[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)  
[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-360/)


## [Demo of App](https://share.streamlit.io/spidy20/innews/App.py)

## Source

- For summarizing the news I have used [Newspaper3k](https://newspaper.readthedocs.io/en/latest/)
- For scraping the news I have used Google News RSS API.

## Features

- Trending News
- Favorite Topics
- Search News
- Quantity control

## Usage

- Clone my repository.
- Open CMD in working directory.
- Run following command.
  ```
  pip install -r requirements.txt
  ```
- `App.py` is the main Python file of Streamlit Web-Application.
- To run app, write following command in CMD. or use any IDE.
  ```
  streamlit run App.py --server.port 80

  ## Use AWS RedHat Linux to deploye the application
##  Deploying the News Application on AWS RedHat Linux
Prerequisites
An AWS account with access to EC2 instances.
Basic knowledge of Linux command-line interface (CLI) and SSH.
Step 1: Launch an EC2 Instance

Log in to your AWS Management Console.
Navigate to EC2 and launch a new instance using RedHat Linux AMI.
Configure security groups to allow inbound traffic on port 80 (HTTP) and 22 (SSH).
Step 2: Connect to Your EC2 Instance
Open your terminal or command prompt.
Use SSH to connect to your EC2 instance:
bash
Copy code
ssh -i your-key.pem ec2-user@ec2-instance-public-ip
Step 3: Install Python and Other Dependencies
Update your package manager:

bash--
Copy code
sudo yum update -y
Install Python and pip:

bash--
Copy code
sudo yum install python3 -y
sudo yum install python3-pip -y
Install necessary Python libraries:

bash--
Copy code
sudo pip3 install streamlit newspaper3k pillow beautifulsoup4 nltk
sudo pip3 install --upgrade setuptools
sudo python3 -m nltk.downloader punkt
Step 4: Clone and Configure the News Application
Clone your GitHub repository containing the news application:

bash--
Copy code
git clone (https://github.com/jayanthsaigithub/Service-Oriented-Architecture-Project-.git)
cd your-repo
Edit the Streamlit configuration in your application:

bash--
Copy code
nano app.py
Update the page configuration:

python--
Copy code--
st.set_page_config(page_title='InNews🇮🇳: A Summarised News📰 Portal', page_icon='./Meta/newspaper.ico')
Step 5: Run the Application
Start the Streamlit application:

bash--
Copy code
streamlit run app.py
Access your application in a web browser:

vbnet--
Copy code--
http://ec2-instance-public-ip:8501
Step 6: Optional - Set Up a Production Server

Install a production-grade web server like Nginx or Apache.
Configure the web server to proxy requests to Streamlit on port 8501.

Step 7: Additional Configuration (if needed)
Configure environment variables or settings specific to your deployment environment.
Implement SSL/TLS certificates for HTTPS if required.

Step 8: Maintenance and Monitoring
Set up monitoring and logging to track application performance and errors.
Schedule periodic updates and backups to maintain application reliability.

Step 9: Conclusion
Your news application is now deployed on AWS RedHat Linux. Test thoroughly and ensure it meets your requirements before making it publicly accessible.
