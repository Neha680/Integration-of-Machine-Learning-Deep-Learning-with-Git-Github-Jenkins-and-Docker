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
![5](https://user-images.githubusercontent.com/64469502/85157018-80815280-b278-11ea-8768-c6f9577bc412.png)

6. Job3 : Train your model and predict accuracy or metrics, if metrics accuracy is less than 80%  , then tweak the machine learning model architecture.

![6](https://user-images.githubusercontent.com/64469502/85157053-8a0aba80-b278-11ea-8101-331868e4c761.png)
![7](https://user-images.githubusercontent.com/64469502/85157078-91ca5f00-b278-11ea-8f13-5cd8e2ba5d33.jpg)
![8](https://user-images.githubusercontent.com/64469502/85157360-00a7b800-b279-11ea-8126-4f7bcfe0ae27.png)


7. Job4 : Retrain the model or notify that the best model is being created

![9](https://user-images.githubusercontent.com/64469502/85157367-030a1200-b279-11ea-82b4-34d8233e6ff6.png)
![10](https://user-images.githubusercontent.com/64469502/85157369-03a2a880-b279-11ea-806a-08178308c2ae.png)

8. Create One extra job job5 for monitor : If container where app is running. fails due to any reason then this job should automatically start the container again from where the last trained model left
![11](https://user-images.githubusercontent.com/64469502/85169531-93e8e980-b289-11ea-99f1-e6e6917473d9.png)
