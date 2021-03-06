#Open Cloud Integrity Technology


**The Open CIT external artifacts project provides :** A couple of external dependencies required to build Open CIT successfully.

# Prerequisites #

To build this project, you will need to download a couple of artifacts and place them in specific directories so we can help you install to your local maven repo.

After you clone the project, cd to the root directory of external artifacts

    cd opencit-external-artifacts
	git checkout release-cit-2.2

Now download each artifact and prepare them to build the opencit-external-artifacts project.


### Apache Tomcat ###

    wget https://archive.apache.org/dist/tomcat/tomcat-7/v7.0.34/bin/apache-tomcat-7.0.34.tar.gz
    mv apache-tomcat-7.0.34.tar.gz apache-tomcat/apache-tomcat-7.0.34.tar.gz


### Glassfish ###
    wget http://download.java.net/glassfish/4.0/release/glassfish-4.0.zip
    mv glassfish-4.0.zip glassfish/glassfish-4.0.zip


### JDK ###

Download the JDK from:

*http://www.oracle.com/technetwork/java/javase/downloads/java-archive-downloads-javase7-521261.html#jdk-7u51-oth-JPR*

Download the following file: *jdk-7u51-linux-x64.tar.gz*

Once you downloaded the file, place it in the jdk directory

    mv jdk-7u51-linux-x64.tar.gz jdk/jdk-1.7.0_51-linux-x64.tar.gz


### Monit ###

    wget https://mmonit.com/monit/dist/monit-5.5.tar.gz
    mv monit-5.5.tar.gz monit/monit-5.5-linux-src.tgz


### TPM Tools ###
    wget https://sourceforge.net/projects/trousers/files/tpm-tools/1.3.8/tpm-tools-1.3.8.tar.gz/download
    mv tpm-tools-1.3.8.tar.gz tpm-tools/tpm-tools-1.3.8.tar.gz


### vijava ###
    wget https://sourceforge.net/projects/vijava/files/vijava/VI%20Java%20API%205.5%20Beta/vijava55b20130927.zip
    unzip vijava55b20130927.zip
    mv vijava55b20130927.jar vijava/vijava-5.5.jar


Now cleanup

    rm -rf *.zip
    rm -rf *.jar
    rm -rf XenServer-SDK


# Build #

You are now ready to build, run

    ant


Please see the [Product Guide](https://github.com/opencit/opencit/wiki/Open-CIT-2.2-Product-Guide) for further details on how this project is used.