# FEUP-MFES
##Railway Signaling System VDM++ Project for MFES class
-------------------------------------------------------
##Project Overview

Specify in VDM++ a signaling system for a circular single track railway, for safely directing railway
traffic and preventing trains from colliding, with the following features:
* The track is doubled in stations, to allow trains to cross. Trains must always stop at stations.
At stations, trains circulate through the left.
* For signaling purposes, the railway is divided into blocks. The track between stations may be
divided into multiple (sequential) blocks. The two parallel tracks existent at each station constitute
distinct (parallel) blocks. No two trains can circulate in the same block.
* There are sensors for detecting trains entering each block.
* There is a semaphore before each block, with the following possible statuses: red - can’t enter
the block; yellow: can enter the block but be prepared to stop at next semaphore (can proceed
at reduced speed); green - can proceed normally (next semaphore cannot be red). The yellow
light is needed because, at full speed, trains may not be able to stop before a red light. For
the same reason, the last block before reaching a station will always present a yellow or red
light at the begin of the block.
* For leaving stations, drivers have to press a button to request permission to proceed. If it is
safe to proceed, the semaphore changes from red to yellow or green (depending on the status
ahead). Once the train starts entering the next block, the semaphore changes back to red.
* The system should be prepared to handle situation in which trains have abnormal stops. 
