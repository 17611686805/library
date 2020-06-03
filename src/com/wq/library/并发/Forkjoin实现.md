# 并行计算
以程序和算法设计人员的角度看，并行计算又可分为数据并行和任务并行。数据并行把大的任务化解成若干个相同的子任务，任务并行是指每一个线程执行一个分配到的任务，而这些线程则被分配（通常是操作系统内核）到该并行计算体系的各个计算节点中去。
   
简单来说，并行计算是通过把大问题划分为小问题，运用计算机资源并行的处理子问题，当需要得到大问题的结果时，将小问题的结果按顺序合并起来得到最终结果。这种思想就是分治思想

# Fork-Join
![](https://mmbiz.qpic.cn/mmbiz_png/f93EtXu3ZkicfT0ibtZGeXGVXficxgRFaa8LyI2HHeqT2GhyW0y6x6liboVLXibIciaK1oUoOQ84tksBchtkkHXdFpFg/640?wx_fmt=png&wxfrom=5&wx_lazy=1&wx_co=1)
Fork join思想步骤：
- 定义拆分和合并子任务的规则
- 利用计算机资源，最大并行执行子任务
- 执行合并所有子任务，获得最终结果
