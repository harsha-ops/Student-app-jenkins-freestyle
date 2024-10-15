Deploying the StudentApp using Jenkins free style job:
Job1
Create a job with the name “setup_tools”
Restrict the job on Slave node
Integrate the with GitHub repo
Add the Build Steps “Execute Shell”
sudo su -c "chmod +x install_tools_studentapp.sh"
sudo su -c "./install_tools_studentapp.sh" 

Test the Tools: -
	 http://52.51.140.10/
	 http://52.51.140.10:8080
	mysql -uroot

Job2: -
	Create a job with the name “Deploy_StudentApp”
	Restrict the job on Slave node
	Integrate the with GitHub repo
	Add the Build Steps “Execute Shell”
	sudo su -c "chmod +x setup_studentapp.sh"
	sudo su devops -c "./setup_studentapp.sh" 
Test the APP:-
	http://52.51.140.10/student/
	http://52.51.140.10:8080/student/
