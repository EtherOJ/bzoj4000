
# Description

<div class="content"><div>“地理哈希”是一个将二维平面坐标编码为整数的过程，这将为数据库中地理数据的存储和查询带来方便。在这个</div>
<div>问题中，一个地图是一个建立在标准二维笛卡尔坐标系上的2^n行2^n列的矩形网格，越往右x坐标越大，越往上y坐</div>
<div>标越大。一个地图格子是一个单位正方形，满足其左下角的点的坐标为(x,y)，其中0&lt;=x,y&lt;2^n。在2^n行2^n列的</div>
<div>地图上一共有2^(2n)个格子。对于一个格子c，它的地理哈希值h(c)是一个2n位的非负二进制整数。从最高位开始</div>
<div>考虑整个地图，然后重复下面两个步骤n次，即可得到c的地理哈希值h(c)：</div>
<div></div>
<div>1.把地图分成左右两个面积相等的区域，如果格子c在左半边，那么这一位是0，否则是1。</div>
<div>然后将考虑范围缩小到c所在的那半边地图。</div>
<div></div>
<div>2.把地图分成上下两个面积相等的区域，如果格子c在下半边，那么这一位是0，否则是1。</div>
<div>然后将考虑范围缩小到c所在的那半边地图。</div>
<div></div>
<div>一个“地理哈希区间”[a,b]表示所有哈希值在[a,b]之间的格子。通常应用中，我们会用一些地理哈希区间去近似</div>
<div>表示地图。给定一个格子集合C，以及一个正整数t，那么C的最优t近似是指使用不超过t个地理哈希区间，覆盖住</div>
<div>所有C中的格子（覆盖其它格子是允许的），同时满足覆盖住的区域的面积最小。给定一个地图以及一个格子集合C</div>
<div>，C用一个边平行于坐标轴的简单多边形来表示。然后给定q个询问t_1,t_2,...,t_q，对于每个询问t_k，你需要求</div>
<div>出C的最优t_k近似覆盖住的区域的面积。</div>
<div></div></div>

# Input

<div class="content"><div>第一行包含一个正整数n(1&lt;=n&lt;=30)，表示地图的尺寸的以2为底的对数。</div>
<div>第二行包含一个正整数m(4&lt;=m&lt;=200)，表示多边形顶点的个数。</div>
<div>接下来m行，每行两个整数x_i,y_i(0&lt;=x_i,y_i&lt;=2^n)，按逆时针依次表示多边形每个顶点的坐标。</div>
<div>输入数据保证多边形不自交，边平行于坐标轴，且不存在相邻两条边是平行的。</div>
<div>接下来一行包含一个正整数q(1&lt;=q&lt;=100000)，表示询问的个数。</div>
<div>接下来q行，每行一个正整数t_1,t_2,...,t_q(1&lt;=t_i&lt;=10^9)，依次表示每个询问。</div>
<div></div></div>

# Output

<div class="content"><div>输出q行，每行一个正整数，依次回答每个询问。</div>
<div></div></div>

# Sample Input

<div class="content"><span class="sampledata">3 8<br/>
1 1<br/>
5 1<br/>
5 4<br/>
3 4<br/>
3 8<br/>
0 8<br/>
0 5<br/>
1 5<br/>
4 2 3 5 7</span></div>

# Sample Output

<div class="content"><span class="sampledata">32<br/>
30<br/>
26<br/>
24</span></div>

# Hint

<div class="content"><p></p><p> <img src="/source/bzoj/4792/img/aHR0cHM6Ly9seWRzeS5jb20vSnVkZ2VPbmxpbmUvdXBsb2FkLzIwMTcwNC9waWMoMikuanBn.jpg" width="425" height="421" alt=""/></p><br/>
<p>区间[3,29]、[33,33]和[36,37]组成最优3近似，其覆盖住的总面积为30。</p><p></p></div>

# Source

<div class="content"><p><a href="problemset.php?search="></a></p></div>

