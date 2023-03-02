# Week 1 — App Containerization

## Homework Tasks:

### while trying to run docker, the port is already allocated 

<img width="704" alt="week-1_port-error" src="https://user-images.githubusercontent.com/62908116/222452399-f7d7d595-4d0c-454c-8a57-28072e8e878f.png">


On further trial and error I found the fault to be already existing containers pointing to the port 

<img width="664" alt="week-1_docker-imgs" src="https://user-images.githubusercontent.com/62908116/222452544-50808dbe-fea8-43ef-8035-edd8c63422d3.png">

And it was solved by running the ```docker kill container``` command

<img width="697" alt="compose up success" src="https://user-images.githubusercontent.com/62908116/222452710-88a3769a-58db-4133-b3bd-4de506f59269.png">

## Added the Front-end and Back-end of Notifications Page

### Front-end Screenshot

![image](https://user-images.githubusercontent.com/62908116/222453680-20318980-8236-4e6b-91b6-7c1e7afacab1.png)

### Back-end API call Screenshot
![image](https://user-images.githubusercontent.com/62908116/222453791-afa8292b-08ac-4236-9a0c-7cfbe17475a2.png)

Faced no problem while doing so.

## Added PostgreSQL and DynamoDB to Gitpod

Copied the code as instrusted and was able to successfully run Postgres and DynamoDB

Ran the following command to check whether the Postgres was working or not:

```
psql -Upostgres --host localhost
```

![image](https://user-images.githubusercontent.com/62908116/222466940-2c01047c-7d38-41a9-9de9-9476faa246e0.png)
