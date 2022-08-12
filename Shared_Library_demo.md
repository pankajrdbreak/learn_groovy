## Shared Library in Groovy
Shared Libraries are something which can be defined in external source control repositories and loaded into existing Pipelines
We can call this functions in our jenkins pipeline

### Setup:
Add Global Pipeline Libraries in System configuration with some name "shared-library"
Default version is master
Project Repository is where your /vars/HelloWorld.groovy available
.groovy files should be under /vars directory 


### Example:
We have a shared library HelloWorld.groovy in which we are echoing "Hello World"
Now in our jenkins pipeline we can import already created shared library 
And inside the pipeline stages we can call this HelloWorld.groovy

Below is the scripted pipeline script
```console
@Library("shared-library") _
pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                HelloWorld()
            }
        }
    }
}
```

