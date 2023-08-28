# Docker for Beginners - Linux

Kujungi website ini [Docker for Beginners - Linux](https://training.play-with-docker.com/beginner-linux/).
![gb1](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/1-1.PNG)<br>

Login to access kernel linux.
![gb2](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/2-1.PNG)<br>

### Task

- Task 0: Prerequisites 
- Task 1: Run some simple Docker containers 
- Task 2: Package and run a custom app using Docker 
- Task 3: Modify a Running Website

## Task 0: Prerequisites

You will need all of the following to complete this lab: 
- A clone of the lab’s GitHub repo. 
- A DockerID.

### Clone the Lab’s GitHub Repo

Use the following command to clone the lab’s repo from GitHub (you can click the command or manually type it). This will make a copy of the lab’s repo in a new sub-directory called ```linux_tweet_app```.

![gb3](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/3-1.PNG)<br>

### Make sure you have a DockerID

If you do not have a DockerID (a free login used to access Docker Hub), please visit [Docker Hub](https://hub.docker.com/) and register for one. You will need this for later steps.

## Task 1: Run some simple Docker containers 

There are different ways to use containers. These include: 
1. To run a single task: This could be a shell script or a custom app. 
2. Interactively: This connects you to the container similar to the way you SSH into a remote server. 
3. In the background: For long-running services like websites and databases. 

In this section you’ll try each of those options and see how Docker manages the workload.

### Run a single task in an Alpine Linux container

![gb4](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/4-1.PNG)<br>
![gb5](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/5-1.PNG)<br>

### Run an interactive Ubuntu container

![gb6](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/6-1.PNG)<br>
![gb7](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/7-1.PNG)<br>
![gb8](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/8-1.PNG)<br>

### Run a background MySQL container

![gb9](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/9-1.PNG)<br>
![gb10](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/10-1.PNG)<br>
![gb11](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/11-1.PNG)<br>
![gb12](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/12-1.PNG)<br>
![gb13](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/13-1.PNG)<br>
![gb14](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/14-1.PNG)<br>

## Task 2: Package and run a custom app using Docker 

In this step you’ll learn how to package your own apps as Docker images using a [Dockerfile](https://docs.docker.com/engine/reference/builder/). 

The Dockerfile syntax is straightforward. In this task, we’re going to create a simple NGINX website from a Dockerfile.

### Build a simple website image

![gb15](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/15-1.PNG)<br>
![gb16](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/16-1.PNG)<br>
![gb17](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/17-1.PNG)<br>
![gb18](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/18-1.PNG)<br>
![gb19](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/19-1.PNG)<br>

## Task 3: Modify a Running Website

### Start our web app with a bind mount

![gb20](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/20-1.PNG)<br>
![gb21](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/21-1.PNG)<br>

### Modify the running website

![gb22](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/22-1.PNG)<br>
![gb23](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/23-1.PNG)<br>

### Stop the current container and re-run the 1.0 image without a bind mount.
![gb24](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/24-1.PNG)<br>
![gb25](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/25-1.PNG)<br>

### Update the image

![gb26](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/26-1.PNG)<br>
![gb27](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/27-1.PNG)<br>

### Test the new version

![gb28](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/28-1.PNG)<br>
![gb29](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/29-1.PNG)<br>
![gb30](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/30-1.PNG)<br>

### Push your images to Docker Hub

![gb31](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/31-1.PNG)<br>
![gb32](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/32-1.PNG)<br>
![gb33](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/33-1.PNG)<br>
![gb34](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/34-1.PNG)<br>
![gb35](https://github.com/AnggerFNS/tekn-cloud-computing/blob/a21ff41b040b23002aa4de463a4d68d69b5e85e0/minggu-09/35-1.PNG)<br>

