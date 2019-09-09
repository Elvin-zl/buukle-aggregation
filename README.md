# buukle-aggregation
An aggregation for devloper , you can decide witch module you want to install together .

# start up

### First, make a dictionary named buukle-resource , then git clone all resource code from github , open your gitbash and use commands like below :

````
    git clone git@github.com:Elvin-zl/buukle-www.git
    git clone git@github.com:Elvin-zl/buukle-util.git
    git clone git@github.com:Elvin-zl/buukle-tc.git
    git clone git@github.com:Elvin-zl/buukle-security.git
    git clone git@github.com:Elvin-zl/buukle-srs.git
    git clone git@github.com:Elvin-zl/buukle-pc.git
    git clone git@github.com:Elvin-zl/buukle-main.git
    git clone git@github.com:Elvin-zl/buukle-drc.git
    git clone git@github.com:Elvin-zl/buukle-common.git
    git clone git@github.com:Elvin-zl/buukle-cms.git
    git clone git@github.com:Elvin-zl/buukle-cloud.git
    git clone git@github.com:Elvin-zl/buukle-aggregation.git
    git clone git@github.com:Elvin-zl/buukle-doc.git
    git clone git@github.com:Elvin-zl/buukle-assistance.git
    git clone git@github.com:Elvin-zl/buukle-wjs.git
        
````
### Second, configure your maven , cause buukle needs some dependencies from <http://maven.buukle.top:8080> , you must make sure your maven configure settings include this repository : http://maven.buukle.top:8080/repository/buukle-group/ . Here is an example : 
````
    <?xml version="1.0" encoding="UTF-8"?>
    <settings xmlns="http://maven.apache.org/SETTINGS/1.0.0"
              xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
              xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.0.0 http://maven.apache.org/xsd/settings-1.0.0.xsd">
     
        <localRepository>D:\repository.buukle</localRepository>
        <servers>       
            <server>   
                <id>buukle-server</id>   
                <username>elvin</username>
                <password>elvin</password> 
            </server>   
        </servers>
        <profiles>
            <profile>
            <id>artifactory</id>
            <repositories>
                <repository>
                    <snapshots>
                        <enabled>true</enabled>
                    </snapshots>
                    <id>buukle-server</id>
                    <name>buukle-snapshots</name>  
                    <url>http://maven.buukle.top:8080/repository/buukle-group/</url>
                </repository>
            </repositories>
        </profile>
        </profiles>
        <activeProfiles>
            <activeProfile>artifactory</activeProfile>
        </activeProfiles>
    </settings>
````
### Third，In your IDEA , open the dictionary named "buukle-resource" , open the buukle-aggregation/pom.xml,and add it as a maven project,let's enjoy our trip with buukle ! 
  