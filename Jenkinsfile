pipeline{
	 agent any
  		stages{
    			stage(checkout){
     			steps{
        		git 'https://github.com/nikitabisan/job1.git'
         		 }
     			 }
   		 stage(build){
    			 steps{
       			 sh 'mvn install'
      				 }
      				}
    		stage(deployment){
     			steps{
       		 sh 'cp target/job1.war /home/nikita/Documents/devops/apache-tomcat-9.0.93/webapps'
     				}
  				}
 			}
		}
