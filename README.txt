This package contains sample code written in Java to demonstrate various ways to use the Tableau Server REST API.

Required tools:
    1. Tableau Server 9.3
    2. Java SE Development Kit 7
        a. Instructions: http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html
    3. Apache Ant
        It is not neccessary to run the "Optional" steps in the Apache Ant guide.
        a. Instructions: http://ant.apache.org/manual/install.html

Optional tools:
    1. A Java IDE (e.g. Eclipse, IntelliJ)

Required Java libraries:
    1. Google Guava 16.0.1
        a. License : https://code.google.com/p/guava-libraries/
        b. Download: http://mvnrepository.com/artifact/com.google.guava/guava/16.0.1
    2. Apache log4j 1.2.17
        a. License : https://logging.apache.org/log4j/1.2/license.html
        b. Download: http://mvnrepository.com/artifact/log4j/log4j/1.2.17
    3. Jersey Client 1.18.3
        a. License : https://jersey.java.net/license.html
        b. Download: http://mvnrepository.com/artifact/com.sun.jersey/jersey-client/1.18.3
    4. Jersey Core 1.18.3
        a. License : https://jersey.java.net/license.html
        b. Download: http://mvnrepository.com/artifact/com.sun.jersey/jersey-core/1.18.3
    5. Jersey Multipart 1.18.3
        a. License : https://jersey.java.net/license.html
        b. Download: http://mvnrepository.com/artifact/com.sun.jersey.contribs/jersey-multipart/1.18.3
    6. Jersey Server 1.18.3
        a. License : https://jersey.java.net/license.html
        b. Download: http://mvnrepository.com/artifact/com.sun.jersey/jersey-server/1.18.3

Getting started:
    1. Install the tools listed in the "Required tools" section.
    2. In the folder where this README file was extracted, create a folder and name it "lib".
    3. Download all libraries listed in the "Required Java libraries" section and put the .jar files for those libraries in the new "lib" folder.
    4. Download the REST API schema and save it in the "res" folder under the folder where this README file is. For more information about the schema, see the following documentation: http://onlinehelp.tableau.com/v9.3/api/rest_api/en-us/help.htm#REST/rest_api_concepts_schema.htm
    5. In the "res" folder, open the "config.properties" file using a text editor.
    6. Modify the configurations as instructed in the file. A sample workbook is already provided with this sample, but you can use any packaged workbook that you want.

Running the sample:
    1. Make sure that Tableau Server is running.
    2. Open a command prompt (e.g. cmd in Windows).
    3. In the command prompt window, change directory to the sample code's parent folder.
    4. Enter "ant" in the command prompt to compile the sample code.
    5. Enter "ant run" in the command prompt to run the sample code after compilation.

Possible problems:
    1. When "ant" is run in a command prompt, it may respond with "'ant' is not recognized as an internal or external command..."
        a. Issue: You did not correctly assign value to the ANT_HOME and JAVA_HOME environment variables.
        a. Resolution: http://ant.apache.org/manual/install.html#windows
           Make sure that the ANT_HOME and JAVA_HOME variables are set as described in the installation guide for Apache Ant. Paths should not include quotes.