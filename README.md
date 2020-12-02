###### Go to the master branch for code. 
###### How to run                                                                                                                                                          
First clone this repository:                                                                                                                                          
###### git clone https://github.com/Salsabil007/Constention-aware-CDS-in-Wireless-Net.git                                                                                   

Install ns2                                                                                                                                                          
###### cd ns-allinone-2.34                                                                                                                                                 

###### ./install                                                                                                                                                           

###### cd ns-2.34                                                                                                                                                           

make                                                                                                                                                                 

###### sudo make install                                                                                                                                                   

Running tcl file                                                                                                                                                      
###### cd ../../run                                                                                                                                                         

###### ns flooding.tcl     

#### Scenario Generation
To test the performance, We need to generate our scenario/topology in a .tcl file. We must create nodes, explicitly mention the links and position of them. Set up TCP/UDP/CBR connection and network traffic and packet size. The protocol are written in AODV file.
Run the file using command: ns file_name.tcl
An animation (.nam) and a trace (.tr) file will be generated. From the trace file we can get info regarding the delay and number of forwarding. 
I have generated a simple scenario of 9 nodes in scenario1.tcl file. Have a look if you want, I have added comments for better understanding.
Below is the nam file generated from scenario1.tcl:
![Scene_1](https://user-images.githubusercontent.com/19349857/100922299-58428480-34a3-11eb-87ef-58cb58a51725.png)
A trace file generated from flooding.tcl:
![Scene_2](https://user-images.githubusercontent.com/19349857/100922309-5aa4de80-34a3-11eb-94bc-7de4dd4a9cbe.png)
#### A good source to analyze the trace file as well as other dynamics of NS-2: https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.527.6286&rep=rep1&type=pdf  


