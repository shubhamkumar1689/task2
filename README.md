DEVOPS ASSEMBLY LINES [TASK2]

Problem Statement :

Create a container image that’s has Jenkins installed using Dockerfile.

When we launch this image, it should automatically start the Jenkins service in the container.

Create a job chain of job1, job2, job3 and job4 using the build pipeline plugin in Jenkins.

Job1: Pull the GitHub repo automatically when some developers push the repo to GitHub.

Job2: By looking at the code or program file, Jenkins should automatically start the respective language interpreter install image container to deploy code ( eg. If code is of PHP, then Jenkins should start the container that has PHP already installed ).

Job3: Test your app if it is working or not.

Job4: If the app is not working, then send an email to the developer with error messages.

Create One extra job job5 for monitor: If the container where the app is running. fails due to any reason then this job should automatically start the container again.


SOLUTION :-

1)
Creating a docker image which install jenkins image and jenkins service
![Screenshot (200)](https://user-images.githubusercontent.com/60147097/81859812-738b8800-9583-11ea-9829-3859b9babot10.png)

2)After building the docker then i run docker image which has jenins install in port no 8084

3) After that creating the job1(Note:github is the name there), job2, job3 and job4 by using build pipeline
![Screenshot (198)](https://user-images.githubusercontent.com/60147097/81860535-8488c900-9584-11ea-9812-e0e635c4ba8d.png)

4)Configuring Job1 task which download data and copy in the docker environment
![Screenshot (201)](https://user-images.githubusercontent.com/60147097/81860833-ed704100-9584-11ea-8208-0c23d8dcd4fc.png)

![Screenshot (203)](https://user-images.githubusercontent.com/60147097/81860891-0547c500-9585-11ea-928e-aa42940153b3.png)

5)Configure the job2 task in my case i write python code which group the file accroding extension but i won't able to start docker inside another docker so i did whatever i know

![Screenshot (208)](https://user-images.githubusercontent.com/60147097/81861195-7dae8600-9585-11ea-8486-414dc71afbe7.png)
![Screenshot (205)](https://user-images.githubusercontent.com/60147097/81861214-843cfd80-9585-11ea-908a-fa9d3e10eab7.png)

6) In job3 testing is to be done
![Screenshot (204)](https://user-images.githubusercontent.com/60147097/81861293-a8004380-9585-11ea-82be-a2ba95fcda49.png)

7) After this if job3 fail then send email 
![Screenshot (206)](https://user-images.githubusercontent.com/60147097/81861438-ded65980-9585-11ea-9eb1-b1d0b56337fe.png)

8) This task in progress

