# Jenkins
___
* Install Azure Key Vault Plugin:
   * Navigate to Manage Jenkins > Manage Plugins.
   * Install the Azure Key Vault plugin.

* Configure Plugin:
   * Go to Manage Jenkins > Configure System.
   * Add Azure credentials and Key Vault configurations.

* Use in Pipelines:
```groovy
pipeline {
    agent any
    environment {
        SECRET_VALUE = credentials('MySecret')
    }
    stages {
        stage('Build') {
            steps {
                echo "Secret Value: ${env.SECRET_VALUE}"
            }
        }
    }
}
```