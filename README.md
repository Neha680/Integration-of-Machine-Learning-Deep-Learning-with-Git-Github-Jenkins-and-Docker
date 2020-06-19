# Integration-of-Machine-Learning-Deep-Learning-with-Git-Github-Jenkins-and-Docker

1. Create container image that’s has Python3 and Keras or numpy  installed  using dockerfile
![pic](https://user-images.githubusercontent.com/64469502/85156257-70b53e80-b277-11ea-8199-1d8e8cfc56a8.jpg)

2. When we launch this image, it should automatically starts train the model in the container.

3. Create a job chain of job1, job2, job3, job4 and job5 using build pipeline plugin in Jenkins

4.  Job1 : Pull  the Github repo automatically when some developers push repo to Github.
   ![1](https://user-images.githubusercontent.com/64469502/85112979-2a8abb80-b234-11ea-9884-9c08fe751991.png)
   ![2](https://user-images.githubusercontent.com/64469502/85113161-79d0ec00-b234-11ea-9fbf-10e670490cbb.png)
   ![3](https://user-images.githubusercontent.com/64469502/85156010-1a480000-b277-11ea-888e-cb04d3d1ab81.png)
   

5.  Job2 : By looking at the code or program file, Jenkins should automatically start the respective machine learning software installed interpreter install image container to deploy code  and start training( eg. If code uses CNN, then Jenkins should start the container that has already installed all the softwares required for the cnn processing).
![4](https://user-images.githubusercontent.com/64469502/85156769-297b7d80-b278-11ea-8a50-b89ce7c6654e.png)

6. Job3 : Train your model and predict accuracy or metrics.

7. Job4 : if metrics accuracy is less than 80%  , then tweak the machine learning model architecture.

8. Job5: Retrain the model or notify that the best model is being created

9. Create One extra job job6 for monitor : If container where app is running. fails due to any reason then this job should automatically start the container again from where the last trained model left
