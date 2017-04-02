# Movie Search API

This project contains a simple servlet application.


## Movie Search API Request Format

A Movie Search API  request takes the following form:

Use the following steps to run the application locally:

    ```bash
    $http://localhost:9080/GetStartedJava/api/visitors
    ```


2. Download and install Liberty, then use it to run the built application from step 1:
    ```bash
    $ mvn liberty:run-server
    ```

    Once the server is running, the application will be available under [http://localhost:9080/JavaHelloWorldApp](http://localhost:9080/JavaHelloWorldApp).

Use the following command to run the built application in Bluemix:
    ```bash
    $ cf push <appname> -p target/JavaHelloWorldApp.war
    ```
## Developing and Deploying using Eclipse

IBM® Eclipse Tools for Bluemix® provides plug-ins that can be installed into an existing Eclipse environment to assist in integrating the developer's integrated development environment (IDE) with Bluemix.

1. Download and install  [IBM Eclipse Tools for Bluemix](https://developer.ibm.com/wasdev/downloads/#asset/tools-IBM_Eclipse_Tools_for_Bluemix).

2. Import this sample into Eclipse using `File` -> `Import` -> `Maven` -> `Existing Maven Projects` option.

3. Create a Liberty server definition:
  - In the `Servers` view right-click -> `New` -> `Server`
  - Select `IBM` -> `WebSphere Application Server Liberty`
  - Choose `Install from an archive or a repository`
  - Enter a destination path (/Users/username/liberty)
  - Choose `WAS Liberty with Java EE 7 Web Profile`
  - Continue the wizard with default options to Finish

4. Run your application locally on Liberty:
  - Right click on the `JavaHelloWorldApp` sample and select `Run As` -> `Run on Server` option
  - Find and select the localhost Liberty server and press `Finish`
  - In a few seconds, your application should be running at http://localhost:9080/JavaHelloWorldApp/

5. Create a Bluemix server definition:
  - In the `Servers` view, right-click -> `New` -> `Server`
  - Select `IBM` -> `IBM Bluemix` and follow the steps in the wizard.\
  - Enter your credentials and click `Next`
  - Select your `org` and `space` and click `Finish`

6. Run your application on Bluemix:
  - Right click on the `JavaHelloWorldApp` sample and select `Run As` -> `Run on Server` option
  - Find and select the `IBM Bluemix` and press `Finish`
  - A wizard will guide you with the deployment options. Be sure to choose a unique `Name` for your application
  - In a few minutes, your application should be running at the URL you chose.

## Liberty App Accelerator

For help generating other Liberty samples checkout the Liberty App Accelerator at [wasdev.net/accelerate](http://wasdev.net/accelerate)

[Liberty Maven Plug-in]: https://github.com/WASdev/ci.maven
