# lambda-deployment-exapmle
This is an example of a script created for AWS CodeBuild. It is in yaml format because buildspec.yml is in yaml. 
But it uses clearly linux commands to prepare and build two functions. One is Python and the other Go language.
The functions previously created using terraform and buildscripts written by developers, this example just shows how to :
1. Include different build scripts for different Lambda functions in one main build script.
2. How to use a single repo to detect in which folder or file the latest changes happend. To be able to build only the function in the folder that was changed.
3. To build and deploy all functions if the buildspec.yml file was changed (becasue it maybe that this affects all functions). 
4. Demonstarte usage of variables since this buildspec is environment agnostic. It can be used to deploy on any dev, stg or prod env without changes. 
