# Week 1 — App Containerization

## Issues faced

### while trying to run docker, the port is already allocated 

![error image]()

On further trial and error I found the fault to be already existing containers pointing to the port 

![image showing allocated port]()

And it was solved by running the ```docker kill container``` command
