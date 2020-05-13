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
