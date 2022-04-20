# CMPE279 : Software Security Technologies

# Team members
1. Krishnaa Satyanarayana
2. Saurabh Kannawar

# Assignment 1

## Contributions
1. Krishnaa - <br>
    Setting up the environment on a ubuntu machine with required libraries <br>
    Fork child processes and exit on completion 
2. Saurabh - <br>
    Identifying socket setup configuration and processing <br>
    Find UID for nobody user and perform privilege dropping for child processes
    
We performed these activities in parallel and proceeded further.

## Steps

<h2> Setting up the Ubuntu machine on Cloud - </h2>

In the below set of steps we will be detailing the instance setup on AWS.

Instance details

* Image - Ubuntu, 20.04 LTS, amd64 focal image build on 2021-11-29
* Instance Type - t2.micro
* 1 vCPU and 1GiB memory

<h2> Setting up the machine with the socket programming code </h2>

1. Committed the server.c and client.c base code into the following github repo https://github.com/krishna201294/CMPE279.git </i> 
2. Clone the code on the virtual machine environment
3. SSH into the AWS instance by using the ssh command provided on AWS instance configuration
4. Clone the repository <br><i> "git clone https://github.com/krishna201294/CMPE279.git" </i>
5. Install the following packages and dependencies 
    a. sudo apt-get install make
    b. sudo apt-get install gcc
6. Make two different windows of the SSH instance and compile the client and the server code
    a. gcc -o server server.c
    b. gcc -o client client.c
7. On one of the terminal run the server code and on the other terminal run the client code
    a. sudo ./server
    b. sudo ./client
  
## Assignment 1 Tasks
1. Identify data processing and socket setup code components
2. Fork child process using fork() operation
3. Perform privilege separation on child process using setuid() 

    
## Screenshot of Output

![Output](https://user-images.githubusercontent.com/9292835/163663691-21080607-ec7e-4323-ac91-cccc670266a7.jpeg)

<hr style="width:100%;text-align:left;margin-left:0">

# Assignment 2

## Contributions
1. Krishnaa - <br>
    Identifying partition between handling child process and parent process.
    Debug and triage issues along the changes performed
2. Saurabh - <br>
    Make changes to pass params to main function and call using execvp()
    
We performed these activities in parallel and proceeded further.

## Repo info
Github repo https://github.com/krishna201294/CMPE279/tree/main/Assignment2 </i> 

## Assignment 2 Tasks
1. Perform fork() + execvp() to create child process
2. Get nobody UID using getpwnam()
3. Identify arguments to be passed to child process

## Screenshot of Output

    
