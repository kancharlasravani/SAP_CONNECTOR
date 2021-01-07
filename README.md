## SAP Third party integration using NCO 3.0
This project is useful for anyone who wants to [integrate SAP with third party applications using NCO 3.0](https://www.veonconsulting.com/integrating-sap-using-nco/). However, it must be understood that this is limitated to (a) SAP ECC and S/4 HANA environments only (b) for real time exchange of information with the instance. 

The code demonstrate how NCO 3.0 library can be used for connecting with SAP ECC or S/4 HANA using the required parameters (listed below) and then subsequently be used for making a call to read information from SAP. The NCO File can be downloaded from SAP Service Market place. This library is not provided in the code repository. 

### SAP NCO 3.0 Project - Installation / Pre-requisite
Before your start with this project, you need to have the following aspects set up. 

* You have the latest version of .NET framework installed on your machine 
* You must also have an IDE for running and debugging a .NET code
* You must have downloaded the NCO 3.0 library from the SAP Service market place
* Access to working SAP ECC or S/4 instance is required

### SAP NCO 3.0 Project - How to use  (Objective)  
The objective of this repository is to have your .NET code connect and authenticate with SAP environment. Subsequently it helps you to read information from SAP on a real time basis by quering database.  

### SAP Integration using NCO 3.0 - Authenticating with SAP 
While authenticating with SAP using NCO 3.0, the following parameters need to be specified.

* SAP_USERNAME - This is the SAP user name with which the call will be made. Ensure that it has proper authority. 
* SAP_APPSERVERHOST - This is the SAP Application server with which the connection will be made
* SAP_PASSWORD - The password corresponding to SAP_USERNAME
* SAP_SYSNUM - SAP System number with which the connection will be made
* SAP_CLIENT - SAP Client number 
* SAP_LANGUAGE - The language for communication. Kindly ensure that respective language has been installed by your BASIS team before specifying the value. 
* SAP_POOLSIZE - The pool size for the RFC call. 

### Making a call to SAP for reading company codes
Further this example shows how a .NET code can be subsequently used for calling a BAPI to read company codes within SAP. In the actual business situation, it is important that you know which BAPI you need to call. It is also mandatory to understand how to use the following parameters in the BAPI.

* Import - These are the parameters which you need to pass to SAP. Correct value must be passed to the respective field. 
* Export - These are the parameters which are populated by SAP in the response. 
* Changing - These can be passed by the program and can be changed by SAP before returing the response
* Tables  - These can hold multiple values in rows. They are essentially changing parameters in tabular format. 

#### Conclusion and further support
Thanks for taking the time to go through our repository. We hope that this was useful. You can reach out to us by sending in your questions or feedback via our Website. 
