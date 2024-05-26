pipeline {
    agent any

    stages {
        stage('Prep') {
            steps {
                    dir('C:\\Users\\Aruna\\Downloads\\ARUNAAITRENDSLAB')
                {
		   pwd()
                    
                }
            }
        }
        stage('Clone repository') 
        {               
            steps {
                    dir('C:\\Users\\Aruna\\Downloads\\ARUNAAITRENDSLAB')
                {
		   bat 'git pull origin b1'    
                }
            }
        } 
        stage('Build image') 
        {         
            steps
            {
                dir('C:\\Users\\Aruna\\Downloads\\ARUNAAITRENDSLAB')
                {
                    bat 'docker build -t aruna2930/labexamimage1:latest .'
                }
            }
        }   
        stage('Push image') 
        {         
            steps {       
                dir('C:\\Users\\Aruna\\Downloads\\ARUNAAITRENDSLAB')
                {
		    bat 'docker push aruna2930/labexamimage1:latest'
                }
            }
        }
        
    }
}
