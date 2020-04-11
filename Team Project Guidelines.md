### The whole idea of the team project is to use what we learned in this course to solve some interesting and important problems. I will encourage you to define what is interesting and important from your business perspective. Team member may come from different background: if you are strong with business - try to contribute on business perspective, if you are strong in coding - try to contribute on coding.

- **Team link (Links to an external site.):** Teams are randomly formed - To work with any type of person in a team is an important ability.
- **Project requirements**
  - **Dataset**: Use suggested datasets or any large scale dataset
  - **Environment**: Use AWS EMR and other AWS services
  - **Programming Language**: Use Spark with R
  - **Functional Requirements**
    - **Ingest**: Ingest dataset to Hdfs or S3 and save as Parquet format.
    - **Basic**： statistics and analysis of the ingested dataset and display (use Jupyter notebook or other type of visualization)
    - **Others**: You guys to define what do you want to achieve in requirement phase.
  - **Performance Requirements**
    - Your applications should shows horizontal scale (i.e. when we adding more nodes the cluster, the processing should be faster also)

- **Timeline**
  - **Requirement phase (Due April 12th):** team discuss functional requirements and come up with requirement document to define what you want to accomplish. Things to do:
     - **Connect:** connect team members through email. Create slack team channels.
     - **Setup:** Join Github classroom (https://github.com/MSBX5420 (Links to an external site.)), join aws classroom (check your aws classroom to join) 
     - **Discuss:** Generate one page (or more thorough) spec documents to layout functional and non-functional requirements etc.
     - **Submit:** Create project Github repo inside Github classroom and check in the requirement spec document.

  - **Design, Development and Test (Due April 25th)**
     - Use Agile development to have several iterations of design, development and test.
     - **Submit:** Check in your design doc and code to Github repo.
  - **Deployment (Due April 28th)**
     - Deploy your program to a larger cluster.
  - **Presentation (Due April 28th)**
     - Present your work in class
- **Suggested DataSets**
  - COVID-19 datasets (such as https://www.kaggle.com/ryanxjhan/cbc-news-coronavirus-articles-march-26 (Links to an external site.))
  - Weather - (such as ftp://ftp.ncdc.noaa.gov/pub/data/gsod) (Links to an external site.)
- **AWS environment**
  - **AWS classroom**. Everyone has $50 credit and you can create small cluster for prototype.
  - **Leeds AWS Cluster:** Leeds school created a AWS account for us. Attached is the key pair file. To ssh to the EMR master node (ssh -                           i ./Leed_HadoopKeypair.pem hadoop@ec2-52-13-183-139.us-west-2.compute.amazonaws.com)
- **How to Score**
  - 50%. Activities to show your leadership and contribution: I will check your check in history in Github Repo. Your code review comments to others. Your slack channel messages etc.
  - 50%. Your project work will be also judged by other classmates during project presentation. (like what we did for class presentation). 
