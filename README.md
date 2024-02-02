# K-Means-clustering-in-Verilog
Understand the overall working of the System, suggest ways to improve performance by pipelining etc.
See the top module is kluster_machine
Datapath file is k_datapath
The control path file is k_controller
Other datapath blocks/modules are also distributed within the folder. (adder, accumulator, sue, comparator, srt divider)

The Input is the Iris flower dataset (150 flowers with 4 features (dimensions) clustered into 3 clusters)
https://www.kaggle.com/datasets/arshid/iris-flower-dataset

The Verilog file k_datapath reads the data files (d1,d2,d3,d4 (4-dimensional array read separately) c1,c2,c3 (3 cluster centroids read separately) and put into memory using function $readmemh
