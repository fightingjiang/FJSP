	分别用改进的粒子群优化算法和改进的差分进化算法求解柔性作业车间调度问题

	问题规模以(工件J*工序P*机器M)表示，例如J20P10M10表示共有20个工件，每个工件有10个工序，总共有10个加工机器可供选择。
	data文件夹中的文件表示程序所用的数据，其中data_first文件的问题规模是J10P5M6，data_second文件的问题规模是J20P10M10，data_third文件的问题规模是J20P20M15。

	关于编码，本项目采用的是同类问题常用的编码方式，参考论文“基于改进遗传算法的柔性作业车间调度问题研究”，与该论文所述的编码方式不同的是，本项目的编码中第一段为工序编码，第二段为机器编码。

	DE文件夹中的三个文件分别采用三种不同的初始化方式，其中DE_first.py采用的是完全随机的初始化方式，DE_second.py采用的是基于轮盘赌策略的初始化方式，DE_third.py采用的是基于极限完工时间最小化的初始化方式。PSO文件夹与DE文件夹类似。
	关于极限最大完工时间最小化策略，参考论文“基于极限调度完工时间最小化的机器选择及FJSP求解”。
