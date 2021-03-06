# CommunityDetection
ComunityDetection 包含三个社区发现算法，
分别为基于k-clique的社区渗透算法、Girvan-Newman 算法和Clauset-Newman-Moore模块度最大化贪心算法。
-----------------------------------------------------------------------------------------------------------------------------
1、基于k-clique的社区渗透算法
该算法中k是外部输入的参数，k的取值会影响最终发现的社区结构，k取值越小，社区将会越大，社区结构稀疏。
该算法是基于完全子图，适用于完全子图较多的网络，而对于稀疏网络效率将会很低，而且无法分配完全子图外的节点。
-----------------------------------------------------------------------------------------------------------------------------
2、Girvan-Newman 算法
GN算法是经典的社区发现算法，属于分裂层次聚类算法。
GN算法基于全局网络特性，需要不断地计算网络中的边介数，通过模块度可以准确地划分网络，但只适用于中小型规模网络。
-----------------------------------------------------------------------------------------------------------------------------
3、Clauset-Newman-Moore模块度最大化贪心算法
CNM是一种贪心算法，可以使最终的社区划分结果有较大的模块度值。
CNM算法是以得到模块度较大的社区划分为目标的贪心算法，可以发现Q值较好的社区划分，但不是Q值最大的社区划分。
-----------------------------------------------------------------------------------------------------------------------------
【注】源码中的第一种布局画的图饱满，单次运行不随机，但是需要额外导入scipy库，源码默认第二种布局。
