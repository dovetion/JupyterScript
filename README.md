# JupyterScript

@author: Dovetion

This is my jupyternotebook script repo

## files description

### beacon_timelist.ipynb

* [LoRa]
* function: calculate the next 100 beacon time list. Beacon time is defined in LoRaWAN protocal, which is the epoch from GPS time equals to 0 (MOD 128). And when the beacon time comes, it makes the system play an audio to notify people. It's useful when implementing and debugging Class B in LoRaWAN



### ficklaw.ipynb

* [Molecular Communication]
* when studing Molecular Communication, it is important to play around with fick's law. So this file is about study the fick's law, including the first and second fick's law. Using different concentration function to calculate the gradient function, the flux function, .etc.



### gateway time diff.ipynb

* [LoRa]
* When we trying to locate items under LoRa network, we use TDOA algorithm. So we have to depoly serveral gateways in the environment, and calculate the time different. This script using two gateway files to calculate the time difference of the same LoRa endnode packet, to evaluate the effectiveness of the TDOA. 
* according to our test, noraml GPS time would cause enormous time difference, it's unacceptable, so we stopped this project.



### gateway_toolate_time.ipynb

* [LoRa]
* When we testing the downlink of the LoRa network, the gateway always repoter "too late" error. It means that when the packet arrive to the gateway, it have passed the emit time window, which is impossible because the link status is great. So this is a debug script to analyse where the time goes and how many time did every process cosume.
* solved, because of the gateway-server downlink keey-alive protocal.





### gw_timeflow.ipynb

* [LoRa]
* There are 3 kinds of time used in the gateway, GPS time(tmms), UTC time(time), and CNT time(tmst). GPS time is from the GPS module, and the UTC time is converted from GPS time, the CNT time is from internal xtal. To implement Class B in LoRaWAN, we need high resolution time, because a pingslot is just 30ms. So the question is what's the error of each time to the real time? This script calculated that error, and the error distribution.





### GwTooLate.ipynb

* [LoRa]
* Another testing script for gateway "too late" error, it's solved by add one more line of code. Everytime when enqueued a packet, just need to break, get out of the while loop.





### lora_gw_time_diff.ipynb

* [LoRa]
* testing script for TDOA





### pktdrop.ipynb

* [LoRa]
* When we need to analyse the packet drop rate for the gateway in LoRa network (normally uplink). We need the gateway printf file. And this script can calculate the packet drop rate for certain endnode, and can give a list of dropped packets' fcnt number. 





### python vs matlab.ipynb

* [course]
* I hate matlab but Dr.Xu loves it, we argued about these two tools. He asked to calculate the speed of matlab and python of solving a matrix's reverse. So here is the answer. Matlab is more fast than the python, but it requires more calculation resources( memory, CPU time slot, .etc) and these to have no significant difference of calculation error.





### Q3-how does google rank webpages.ipynb

* [course]
* It's a preparation script for Dr.Xu's course





### Q8_egienvector_centrality

* [course]
* Dr.Xu's course, this script is to calculate the eigenvector centrality of a given graph to simulate the results of  "how to describe the importance of a node in a graph"





### tiantian.ipynb

* [draw]
* helping a friend to visualize his data.





### too late report

* [LoRa]
* this is a conclusion of the gateway "too late" problem, and it's solved.