# Longhorn
- #### Installation of Longhorn:
- #### Using the Environment Check Script
![image](https://user-images.githubusercontent.com/103019032/173506285-dc0ed176-2d86-4f3a-8759-09a41e392d7c.png)
![image](https://user-images.githubusercontent.com/103019032/173506186-54f076f4-da2e-4ccf-970d-7cde1b954999.png)
- #### I have install longhorn with kubectl command.
![image](https://user-images.githubusercontent.com/103019032/173509073-9b6dc415-4b93-4b8a-8d90-754c54c05195.png)
- #### One way to monitor the progress of the installation is to watch pods being created in the longhorn-system namespace
![image](https://user-images.githubusercontent.com/103019032/173509687-8e307794-2601-4fcf-9ee7-026f73c29d50.png)
- #### Check that the deployment was successful:
![image](https://user-images.githubusercontent.com/103019032/173510035-5d1f47f5-2a14-44fb-bd3a-8085abb60102.png)
- #### Using YAML file,create the storage class.
![image](https://user-images.githubusercontent.com/103019032/173511292-0ba2ffa8-8b78-4cf9-8110-bed92d7e3cb1.png)
- #### Create a Pod that uses Longhorn volumes by YAML file.
![image](https://user-images.githubusercontent.com/103019032/173511737-49cc7165-fab4-4164-8b15-2947bd1ba194.png)
- #### A Pod named nginx-pod is launched, along with a PersistentVolumeClaim named my-longhorn. The PersistentVolumeClaim references the Longhorn StorageClass.
![image](https://user-images.githubusercontent.com/103019032/173512336-be688b60-5e0d-4a90-ab0d-24e12925c238.png)
- #### Check nginx-pod status,it's running or not,using kubectl get pod<pod name>.
![image](https://user-images.githubusercontent.com/103019032/173512867-52cef3e2-5c5e-40b6-a6cd-4ce6636384b3.png)
- #### Check pvc is created or not,using kubectl get pvc.
![image](https://user-images.githubusercontent.com/103019032/173513185-1de0bc47-1767-4280-acb4-cc98a969101f.png)
- You can check through longhorn ui,but before that,you can type the command ip for frontend  for accessing ui.
![longhorn ui](https://user-images.githubusercontent.com/103019032/173514979-b341079c-af4d-42b3-a236-8540a8091665.PNG)
- #### It is the ui of Longhorn.
![image](https://user-images.githubusercontent.com/103019032/173515522-5b888a1b-3912-4a28-b706-891db8fcac5f.png)
- #### Now check the pvc through longhorn ui,click on volume option,then click name of pvc,and show the details of pvc.
![longhorn-pvc](https://user-images.githubusercontent.com/103019032/173516616-1ff9766a-42bc-4bf3-9cbe-c894d3fb2759.PNG)
- #### Show all the details of volume.
![image](https://user-images.githubusercontent.com/103019032/173517161-bc194890-19c8-4d6a-a0f8-6ff2b66c6efe.png)
- #### Node space Usage:
- #### In Dashboard page, Longhorn will show you the cluster space usage info
![image](https://user-images.githubusercontent.com/103019032/173517942-b07d22a1-334d-4b0b-817d-285111964035.png)
- #### In Node page, Longhorn will show the space allocation, schedule, and usage info for each node
![image](https://user-images.githubusercontent.com/103019032/173518084-e572330e-9ca7-4bb7-9268-49443b8fa7e0.png)



