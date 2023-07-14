# Introduction

## Description 
  SuperBuffer is a project designed for speeding up Aleo applications.      
  Aleo is a platform for web applications that need security and privacy guarantees.
Yet, users often have to endure huge time costs for each request execution. In addition, Aleo relies on heavy computation resources required for zero-knowledge proofs, which is the main challenge for users with weak computation power.       
  In order to address aforementioned problems, we design SuperBuffer, a middleware to cache these requests and substitute for executing these heavy computations.
 ## Main Advantages
  The main advantages of this design for Aleo ecosystem can be summarized as follows:      
a. Users can proceed to the next move without waiting for the response to be put on the chain.      
b. Users can delegate heavy computation (i.e. zero-knowledge proof) to a device with powerful computation resources (e.g. sequencer, nodes with GPU/FPGA).     
c. The computation overhead of verifying the request proof is cheap.    
d. Users can query the state of their own requests at any time.     
e. SuperBuffer inherits the privacy-preserving feature of Aleo.
 ## Interactive Diagram
![image](https://github.com/superbuffers/introduction/blob/main/diagram/fundament.png)
 ## SuperBuffer Building
  We choose the [battleship game](https://en.wikipedia.org/wiki/Battleship_(game)) which is well-known to most people for SuperBuffer to speed up. We design and implement three parts to introduce our
high-level idea.
 ### Aleo Contract
  Battleship Aleo contract as one case is used to show us the diverse possibilities of Aleo economy by official team. We want to use this game to present the speeding up process of SuperBuffer.   
  Please go to  for the run guide and implementation.
 ### Back End
  Back end receives the requests from front end and broadcasts key messages to Aleo chain. This part is responsible for ordering, verification, proof generation, and broadcasting transactions.    
  Please go to [superbuffer-battleship](https://github.com/superbuffers/superbuffer-battleship) for the run guide and implementation.    
 ### Front End
  Front end mainly presents the battleship game for players. Front end needs to execute and show every steps in game. This component also needs to generate requests signed by players according to their actions and transmit these requests to back end.      
  Please go to [ui](https://github.com/superbuffers/ui) for the run guide and implementation.    
