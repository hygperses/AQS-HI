paper:基于历史信息的高效近似查询系统

## Introduction
Approximate query processing techniques play a pivotal role in enhancing the efficiency of aggregate database queries. In this paper, we propose an approximate query system for massive high-dimensional data that leverages historical query workloads. By incorporating historical query information and conducting hit detection within the historical query space, we effectively improve query efficiency, addressing issues like query region skewness. For global queries, paper employ spatial data partitioning techniques to divide the entire dataset into subregions and organize them into a tree-like shard index structure. This integration of sampling and data summarization methods enhances query accuracy. Experimental results demonstrate that when the volume of historical query records reaches an order of magnitude, query response times are reduced to only 40% of traditional methods. Furthermore, compared to traditional methods, our system achieves an average relative error reduction of 63%. The effectiveness of the system increases with the number of shards, with an average relative error of only 10% when the number of shards reaches 64.

## Dependencies 
- GEOS: brew install geos
- BOOST C++ library : brew install boost

- ## Build and Run test
- Compile the project using CMake. It will build a new direcotory named as ``` build```
  ```./build.sh ```
- Run unit tests 
  ``` ./build/test_aqs ```
  
