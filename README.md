# Introduction

## Description 
  SuperBuffer is a project designed for speeding up Aleo applications.      
  Aleo is a platform for web applications that need security and privacy guarantees.
Yet, users often have to endure huge time costs for each request execution. In addition, Aleo relies on heavy computation resources required for zero-knowledge proofs, which is the main challenge for users with weak computation power.       
  In order to address aforementioned problems, we design SuperBuffer, a middleware to cache these requests and substitute for executing these computations.
 ## Main Advantages
  The main advantages of this design for Aleo ecosystem can be summarized as follows:      
a. Users can proceed to the next move without waiting for the response to be put on the chain.      
b. Users can delegate heavy computation (i.e. zero-knowledge proof) to a device with powerful computation resources (e.g. sequencer, nodes with GPU/FPGA).     
c. The computation overhead of verifying the request proof is cheap.    
d. Users can query the state of their own requests at any time.     
e. SuperBuffer inherits the privacy-preserving feature of Aleo.
 ## Interactive Diagram
![image](https://github.com/superbuffers/introduction/blob/main/diagram/fundament.png)
