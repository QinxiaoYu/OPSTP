# OPSTP
This repository includes the data set used in the paper "A matheuristic approach to the orienteering problem with service time dependent profits".

## Instances

- [kroData/file_format.md](./kroData/file_format.md) is a description of the text file that defines the network used in each Kro instance.
  ```
    <Number of nodes>
    X Y Profit(p_i) MinServiceTime(r_i) ProfitCollectingCoefficient(beta_i) MustVisit
    3140.0 1401.0    0.0    0.0   0.50 1
    556.0 1056.0   92.0   79.0   0.38 0
    ...
    Tmax
  ```
  TIPS:
  1. The first node is the starting and ending node.
  2. ProfitCollectingCoefficient(beta_i) should divide by 200 when using.
  3. Distance between any two nodes is Euclidean distance	and rounded to the closest integer.
  4. The data generation scheme is from "Erdogan, G. , & Laporte, G. (2013). The orienteering problem with variable profits. Networks, 61 (2), 104-116 ."
  

## Results 

The detailed results for Kro instances listed in the mentioned paper are included in the [kroData/Results_BestRoutes.csv](./kroData/Results_BestRoutes.csv).

-Each row shows the detailed information of the best route obtained from TSNLP(the proposed matheuristic method in our paper).
-The detailed information includes the objective value, total service time, total travel time, the number of visited customers, the route sequence, and the service time for each visited customer.


## Contact Info
Feel free to contact me for more information about our paper via email: Qinxiao Yu (yuqinxiao@tju.edu.cn)

