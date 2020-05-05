node {
    stage('SCM Checkout') {
        git 'https://github.com/clecioantao/my-app-javahometech-curso'
    }
    stage('Compile Package') {
        // Get mavan home path
        def mvnHome = tool name: 'M2_HOME', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
    }

}