# Useful-traits-and-commands

### SSH tunelling - access jupyter notebook running on a remote server

1.	Log into Lambda Labs via Terminal
    
    a.	Command:  >> ssh username@unomaha.edu@<IP address>

2.	Navigate to Debug program folder

3.	Activate jupyter notebook
      a.	Command: >>  jupyter notebook
  
4.	copy link generated in terminal
    a.	Example: http://localhost:8888/?token=687b245463e88a654a2480218e0162ad7caf358879f76891
    b.	Note the 4 digit port number (bold in last bullet point)

5.	Open new terminal window and enter the follow command to complete port forwarding
     a.	Use the recorded 4 digit port number
     b.	 >> ssh -N -L localhost:8888:localhost:8888 username@unomaha.edu@<IP address>

6.	Open copied link from step 4 in web browser
  
  
 #########################################################################################
    
 ### generate intellicense in jupyter notebooks running locally
    
  Run the following command before beginning to code
    
    >> %config IPCompleter.greedy=True

