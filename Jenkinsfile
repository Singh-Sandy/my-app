node {
        stage('Checkout') { 
            git 'https://github.com/Singh-Sandy/my-app.git'
        }
        stage('Compile_Package') { 
            def mvnHome = tool name: 'apache-maven-3.6.3', type: 'maven'
            bat /c "${mvnHome}/bin/mvn package"
        }
    }
