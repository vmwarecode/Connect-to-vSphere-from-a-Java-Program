This sample code shows how to make a connection to ESX or vCenter, and get back some simple information from it. All the code needed is included in this one Java file.

How to Run

In order to run this sample code you must provide three arguments:
[1] The server name or IP address
[2] The user name to log in as
[3] The password to use

You will need to get the vim25.jar library from the VMware vSphere JDK.  It is in the VMware-vSphere-SDK-5.5.0\vsphere-ws\java\JAXWS\lib directory.

You can run this sample code with a command similar to the following :
java -cp "vim25.jar;TestConnection.jar" com.vmware.sample.TestConnection <ip-or-domain-name> <user> <password>
for example:
java -cp "lib\vim25.jar:lib\TestConnection.jar" com.vmware.sample.TestConnection 127.0.0.1 root rootPassword

The 127.0.0.1 address is the local host, so will work if you are running the script from the same 
machine as vCenter is installed on.  If not, put in the vCenter machine's IP or domain name.
If you password contains strange characters that your shell uses (such as ! # ; | and so on), you 
should put quotes around it.

Output

You will see the output similar to the following when you run the sample:
VMware vCenter Server 5.5.0 build-1312298
Server type is VirtualCenter
API version is 5.5.0
