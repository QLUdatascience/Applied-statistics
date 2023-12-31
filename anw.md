## 简答题

### 使用图的形式展示统计数据有什么优势？常用的统计图有哪些？ 

**可以准确的表达数据想要传递的信息，可以清晰的显示数据和表达统计目的，让人更容易看懂和理解数据。**

- 图形可以直观地表现数据的特征、规律和关系，比纯文本或数字更容易吸引人的注意力和兴趣。
- 图形可以更有效地传达信息，帮助人们快速理解和记忆数据的含义和价值。
- 图形可以更美观地呈现数据，增加数据的视觉冲击力和吸引力，提高数据的说服力和影响力。

常用的统计图：**`直方图`**，**`箱形图`**，**`散点图`**，**`雷达图`**



### 简述算数平均数、几何平均数、中位数的适用范围。 

算数平均数：***适用于数据分布较为对称且没有极端值的情况。***

几何平均数：***适用于数据之间存在乘法关系或者比例关系的情况。如对比率、指数等进行平均，计算平均发展速度；***

中位数：***适用于数据分布不对称或者存在极端值的情况。***



### 表示数据分散程度的有哪些？ 

**`全距和四分位距`**，**`方差和标准差`**，**`离散系数`**，**`标准分数`**。



### 什么是统计学？统计学的研究对象是什么？研究对象有哪些特点？

统计学是***收集，处理，分析，解释数据并从数据中得出结论的科学。***

统计学的研究对象是***来自各领域的数据，统计学没有任何固定的对象，是一门独特的学问，用于解决其他领域内的问题***

研究对象的特点：**`随机性`**，**`变异性`**，**`大量性`**，**`多样性`**，**`可度量性`**









## 计算题

1. #### 某班分甲乙两个学习小组，在统计学考试中，甲小组平均成绩 75，标准差为 11.5，乙小组成绩如下表所示，（第4章 数据的概括性度量）

![image-20231225143059479](https://starain-1252568110.cos.ap-beijing.myqcloud.com/blog/image-20231225143059479.png)



**1）比较哪个小组的成绩偏高；**

各组取中间值，分别为 55, 65, 75, 85, 95

$$
\overline{x} = \frac{55\times 10+65\times 25 + 75\times 40 + 85\times 19 + 95\times 4}{10+25+40+19+4} \approx 73.16
$$

与甲组(75)比较，甲组更高，所以甲组成绩偏高



**2）使用离散系数比较两组样本数据的离散程度。**

$$
\begin{equation} \label{}
\begin{split}

s & = \sqrt{\frac{(55-73.16)^2\times10+(65-73.16)^2\times 25+(75-73.16)^2\times 40+(85-73.16)^2\times 19+(95-73.16)^2\times 4}{10+25+40+19+4}} \\
& = \ \sqrt{\frac{3112+ 1681+ 129.6+ 2645.6+1901}{98}} \\
& = \ 9.83

\end{split}
\end{equation}
$$

离散系数：

$$
CV_{甲} = \frac{s_{甲}}{\overline{x_{甲}}} = \frac{11.5}{75} \approx 15.33\%
$$

$$
CV_{乙} = \frac{s_{乙}}{\overline{x_{乙}}} = \frac{9.83}{73.16} \approx 13.44\%
$$









2. #### 某企业某种产品的有关数据如下，按照环比增长速度和定基增长速度定义， 补全下表（）中缺失的部分。（第13章 时间序列分析和预测）

![image-20231225143146803](https://starain-1252568110.cos.ap-beijing.myqcloud.com/blog/image-20231225143146803.png)

| 年份         | 1999 | 2000     | 2001      | 2002       | 2003       | 2004      |
| ------------ | ---- | -------- | --------- | ---------- | ---------- | --------- |
| 环比增长速度 | -    | 5.3%     | **3.99%** | 0.48%      | 4.3%       | **4.66%** |
| 定基增长速度 | -    | **5.3%** | 9.5%      | **10.02%** | **14.75%** | 20.1%     |









3. #### 为了解某因素对产品销量的影响，收集了过去 10 年的有关数据。根据计算 得到以下方差分析表，（第10章 方差分析  P196）

![image-20231225143205506](https://starain-1252568110.cos.ap-beijing.myqcloud.com/blog/image-20231225143205506.png)

**1）补全表（）中缺失的部分；**

|      | df   | SS     | MS     | F    |
| ---- | ---- | ------ | ------ | ---- |
| SSA  | 3    | 1456.6 | 485.53 | 3.41 |
| SSE  | 19   | 2708   | 142.53 |      |
| SST  | 22   | 4164.6 |        |      |

**2）计算 $R^2$，并对结果进行分析。**

$$
R^2 = \frac{SSA}{SST} = \frac{1456.6}{4164.6} \approx 34.96\%
$$






4. #### 研究上市公司对其股价波动的关注程度，一家研究机构对在主板、中小板和 创业板上市的 190 家公司进行了调查，得到如下信息：

![image-20231225143322184](https://starain-1252568110.cos.ap-beijing.myqcloud.com/blog/image-20231225143322184.png)

**检验上市公司的类型与对股价波动的关注程度是否独立(α=0.05)。**

| 上市公司的类型 | 关注 | 不关注 | 合计 |
| -------------- | ---- | ------ | ---- |
| 主板企业       | 50   | 70     | 120  |
| 中小板企业     | 30   | 15     | 45   |
| 创业板企业     | 20   | 5      | 25   |
| 合计           | 100  | 90     | 190  |



| 行   | 列   | $f_0$ | $f_e$  | $f_0 - f_e$ | $(f_0 - f_e)^2$ | $(f_0 - f_e)^2/f_e$ |
| ---- | ---- | ----- | ------ | ----------- | --------------- | ------------------- |
| 1    | 1    | 50    | 63.158 | -13.158     | 173.13296       | 2.74127             |
| 1    | 2    | 70    | 56.842 | 13.158      | 173.13296       | 3.04586             |
| 2    | 1    | 30    | 23.684 | 6.316       | 39.89186        | 1.68434             |
| 2    | 2    | 15    | 21.316 | -6.316      | 39.89186        | 1.87145             |
| 3    | 1    | 20    | 13.158 | 6.842       | 46.81296        | 3.55776             |
| 3    | 2    | 5     | 11.842 | -6.842      | 46.81296        | 3.95313             |



$H_0$: 上市公司的类型与对股价波动的关注程度是独立的
$H_1$: 上市公司的类型与对股价波动的关注程度不是独立的

$$
\chi^2 = \sum \frac{(f_0 - f_e)^2}{f_e} \approx 16.853 > \chi_{0.05}^2(2) = 5.9915
$$

故拒绝 $H_0$ 接受 $H_1$, 上市公司的类型与对股价波动的关注程度之间存在依赖关系







5. #### 为研究产品销售额与销售利润之间的关系，某公司对所属 6 家企业进行了调 查，设产品销售额为 x(万元)，销售利润为 y(万元)。调查资料经初步整理和计算， 结果如下：(第11章 一元线性回归)

$$
\sum x=225, \sum x^2=9823, \sum y = 13, \sum y^2 = 36.7, \sum xy = 593
$$

1）计算销售额与销售利润之间的相关系数；

$$
r = \frac{n\sum xy - \sum x \sum y}{\sqrt{n\sum x^2 - (\sum x)^2 }\times \sqrt{n\sum y^2 - (\sum y)^2}} = \frac{6\times 593 - 225\times 13}{\sqrt{6\times 9823 - 225^2 }\times \sqrt{6\times 36.7 - 13^2}} = \frac{633}{652.39988} = 0.97026
$$

2）给出销售利润对销售额的回归方程，并计算回归方程系数；
$$
\overline{x} = \frac{\sum x}{n} = \frac{225}{6} = 37.5, \\ 
\overline{y} = \frac{\sum y}{n} = \frac{13}{6} = 2.167
$$

$$
\hat{\beta_1} = \frac{6\times 593-225\times13}{6\times9823-225^2} = 0.07615
$$

$$
\hat{\beta_0} = \overline{y} - \hat{\beta_1} \overline{x} = 2.167- 0.07615 \times 37.5 = -0.68863
$$

$$
\hat{y} = 0.07615x-0.68863
$$





3）计算判定系数 $R^2$

$$
R^2 = r^2 = 0.94141
$$




6. #### 一家保险公司收集到由 36 个投保人组成的随机样本，得到每个投保人的年龄(单位：周岁)数据如下表。试建立投保人年龄的置信区间（α=0.1）。（第7章 参数估计）

![image-20231225143545705](https://starain-1252568110.cos.ap-beijing.myqcloud.com/blog/image-20231225143545705.png)

$$
\overline{x}= \frac{208+246+252+242+251+223}{36} = \frac{1422}{36} = 39.5
$$

$$
s = 7.66
$$

（假设符合正态分布）由于 样本数量为36大于 30 用 z 分布

置信区间为: 

$$
\overline{x} \pm z_{0.005}\times \frac{\sigma}{\sqrt{n}} = 39.5 \pm \frac{7.66}{6} = 39.5\pm1.277
$$








7. ####  某橡胶厂生产汽车轮胎，厂商宣称使用他们的橡胶生产的轮胎平均里程不 低于 $25\times10^3$ 公里。现在从近期生产的轮胎中随机抽取 100 个做试验，检验结果 如下表所示，检验该制造商的说法是否可信（α=0.05）。（第8章 假设检验）

![image-20231225143607497](https://starain-1252568110.cos.ap-beijing.myqcloud.com/blog/image-20231225143607497.png)

每组取中值 23.5, 24.5, 25.5, 26.5

$H_0$: 厂商的说法正确，即总体平均值 $\mu$ 等于 $25×10^3$ 公里。
$H_1$: 厂商说法不正确，即总体平均值 $\mu$ 小于 $25×10^3$ 公里。

$$
\overline{x} = \frac{23.5\times 10+24.5\times20 + 25.5\times 50 + 26.5\times 20}{100} = 25.3
$$

$$
s = \sqrt{\frac{32.4+12.8+2+28.8}{100-1}}= 0.87617
$$

$$
z = \frac{\overline{x}-\mu_0}{\sigma/\sqrt{n}} = \frac{25.3-25}{0.87617/10} \approx 3.42399 > z_{0.05} = 1.64
$$

故拒绝原假设





8. #### 某企业生产的袋装食品采用自动打包机包装，每袋标准重量为 100 克。 现从某天生产的一批产品中按重复抽样随机抽取 50 袋进行检查，得到如下 数据：（第7章 参数估计，P130 7.3）

![image-20231225143626056](https://starain-1252568110.cos.ap-beijing.myqcloud.com/blog/image-20231225143626056.png)

**已知食品每袋的重量服从正态分布，要求：**

**1）计算该样本的均值和标准差；** 

各组取中间值，分别为 97, 99, 101, 103, 105

$$
\overline{x} = 101.32
$$

$$
s = \sqrt{\frac{37.32+16.15+3.48+19.76+54.17}{50-1}} \approx 1.63433
$$





**2）确定该食品平均重量的 99%的置信区间。**
$$
\Delta = \frac{\sigma}{\sqrt{n}} = \frac{1.63433}{\sqrt{50}} \approx 0.23113
$$
 大样本(>30) 选择 z 分布，置信区间为：
$$
\overline{x} \pm \Delta \times z_{a/2} = 101.32 \pm 0.59631
$$

**3）如果规定食品重量低于 100 克属于不合格，确定该批食品合格率的 95% 的置信区间。**

低于100克有5个，

$p=1-\frac{5}{50} = 90\%$ 

$$
p \pm z_{\alpha/2}\sqrt{\frac{p(1-p)}{n}} = 0.9 \pm 1.96 \times \sqrt{\frac{0.9\times(1-0.9)}{50}} = 0.9 \pm 0.08316
$$






---

注：

$t_{0.005}(99) \approx 2.626, t_{0.01(99)}=2.364, Z_{0.025}=1.96, Z_{0.005}=2.58$

