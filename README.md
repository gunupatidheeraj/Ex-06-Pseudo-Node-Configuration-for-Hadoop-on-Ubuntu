# Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu

## AIM

To implement Pseudo Node configuration for Hadoop on ubuntu

## Pre-requisites

a) jdk

Single-Node Configuration

1.	Create a dedicated user account for hadoop


![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/dc836092-ce76-4bcd-a965-bdd83918d8be)

2.	Install java1.8 in folder /usr/local


  ![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/d49170bb-7c79-45b3-80e2-df4413abcf5e)

3.	Install Hadoop


![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/82947a99-cef2-4a55-bee3-bff53e5ff0c9)

4.	Set the hadoop environment variables: Include the following lines in the
$HOME/.bashrc file


![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/259fd779-e99d-4f87-bc7a-6f629968eac4)

 
5.	Set hadoop environment variables: Include the following lines /etc/profile file


![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/0cdf090f-03f4-416b-b8e9-98fbdd6cefce)


6.	Run the.bashrc & profile files from the $ prompt for updating the changes

![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/596ee2c7-0502-4fe6-b7c7-0338b77ce3e1)



$ bin/hadoop version	

7.	Configuration of the hadoop files: hadoop-env.sh, core-site.xml, mapred-site.xml, hdfs- site.xml and yarn-site.xml

path ::	/usr/local/hadoop-2.5.1/etc/hadoop

a)	hadoop-env.sh
Include the following lines in hadoop-env.sh file


![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/ac50077a-13d8-46ba-adf5-094abbc9179d)

b)	core-site.xml
Configure the directory for Hadoop to store its data files, the network ports it listens to, etc. Setup will use Hadoop’s Distributed File System (HDFS-single local machine)

![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/c84b6784-518f-490c-a3f2-b55726b1cac6)

 
Include the following lines in core-site.xml file between <configuration> and
</configuration> tags


![Uploading image.png…]()

c)	mapred-site.xml
 
![Uploading image.png…]()

Include the following lines in mapred-site.xml file


 ![Uploading image.png…]()


d)	hdfs-site.xml
Include the following lines in hdfs-site.xml file


![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/b76715b5-a7a6-4f9a-97a9-3ffa8308eb12)


e)	yarn-site.xml
Include the following lines in yarn-site.xml file


![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/a8fe8371-0e36-4e68-bc6d-58b56b568ed9)

8.	Format the Hadoop File system implemented on top of the local file system using


![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/d32cf21d-2387-4d13-bc21-9114508fa281)

9.	Start Hadoop using

![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/d52c3f9c-229c-466b-acca-29133dad6309)

Explore Hadoop using http://localhost:50070/ from the browser	
 
10.	The commonly used HDFS Commands are as follows:


![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/bdc0710e-e924-4ca8-9029-ed6abc503884)


11.	Create a directory ‘/input’ in HDFS

![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/c69d7a09-8d05-4bfb-8f68-8bc2b652677a)


12.	Copy the input files into the distributed file system


 ![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/9e39eeeb-7527-4f53-9e02-6b3effab2859)


13.	Run some of the examples provided

![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/e8849cb2-645a-4c10-b8a9-d0bee3931913)


14.	Examine the output files
Copy the output files from the distributed file system to the local file system and examine them:

![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/40c4ce51-81af-493e-91ca-643e26a22ba9)



or

 ![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/08006dad-317f-4952-85d6-894ac03a0a14)
View the output files on the distributed file system

![image](https://github.com/gunupatidheeraj/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/146909163/b8da249f-0dfe-4ceb-97bd-26476f5cb40f)

## Result:
Thus, the implementation of Pseudo Node configuration for Hadoop on ubuntu is successfully executed.
