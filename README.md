# README for Apache Fortress Demo End-to-End Security Example

## Last updated: March 15, 2015

## Prerequisites for target machine:
### 1. Debian or Redhat Liunx machine with OpenSSL installed.

### 2. Java 7 (or greater) sdk

### 3. Git

### 4. Apache Maven 3

### 5. Firefox Web Browser

### 6. Follow the [Apache Fortress Ten Minute Guide](http://symas.com/javadocs/apache-fortress-core/org/apache/directory/fortress/core/doc-files/ten-minute-guide.html)
#### Complete these steps under 'Navigation Links':
#### a. [Setup Apache Directory Server](http://symas.com/javadocs/apache-fortress-core/org/apache/directory/fortress/core/doc-files/apache-directory-server.html)
#### b. [Setup Apache Directory Studio](http://symas.com/javadocs/apache-fortress-core/org/apache/directory/fortress/core/doc-files/apache-directory-studio.html)
#### c. [Build Apache Fortress Core](http://symas.com/javadocs/apache-fortress-core/org/apache/directory/fortress/core/doc-files/apache-fortress-core.html)
#### d. [Build Apache Fortress Realm](http://symas.com/javadocs/apache-fortress-core/org/apache/directory/fortress/core/doc-files/apache-fortress-realm.html)
#### e. [Setup Apache Tomcat Web Server](http://symas.com/javadocs/apache-fortress-core/org/apache/directory/fortress/core/doc-files/apache-tomcat.html)
#### f. [Build Apache Fortress Web](http://symas.com/javadocs/apache-fortress-core/org/apache/directory/fortress/core/doc-files/apache-fortress-web.html)

## Instructions for downloading app and generating the install doc:

### 1. [Download ZIP](github: https://github.com/shawnmckinney/apache-fortress-demo/archive/master.zip)

### 2. Extract the contents zip archive to your local machine.

### 3. cd apache-fortress-demo-master

### 4. Set java and maven home env variables.

### 5. Run this command from the root package:
````
mvn javadoc:javadoc
````

note: if using java 8, add this param to the pom.xml:
````
<plugin>
    ...
    <artifactId>maven-javadoc-plugin</artifactId>
    <configuration>
        <additionalparam>-Xdoclint:none</additionalparam>
        ...
    </configuration>
</plugin>
````

### 6. Point your web browser to the following location:
[Apache Fortress Overview](target/site/apidocs/overview-summary.html)

### 7. Follow the steps under 'Demo Installation Instructions':

#### a. [Heartbleed Bug](target/site/apidocs/doc-files/opensslheartbleed.html)
#### b. [Managing PKI Keys](target/site/apidocs/doc-files/keys.html)
#### c. [Set Hostname Entry](target/site/apidocs/doc-files/hosts.html)
#### d. [Apache Directory SSL](target/site/apidocs/doc-files/apache-directory-ssl.html)
#### e. [Apache Fortress Core SSL](target/site/apidocs/doc-files/apache-fortress-core-ssl.html)
#### f. [Install MySQL](target/site/apidocs/doc-files/mysql.html)
#### g. [Apache Tomcat SSL](target/site/apidocs/doc-files/apache-tomcat-ssl.html)
#### h. [Apache Fortress Demo](target/site/apidocs/doc-files/apache-fortress-demo.html)