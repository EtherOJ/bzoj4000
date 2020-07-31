
# Description

<div class="content"><div>今天Nick来到了一个大公司(CCF)，这个公司掌控了整个城市的运输系统，这个运输系统在各</div>
<div>种运输线的连接下形成了一个网状结构。</div>
<div>当然，任何系统都会有缺陷，这个系统的缺陷在于所有的运输线都会有一定的延时，一共有n</div>
<div>种运输线，相同种类的运输线延时是相同的。</div>
<div>由于每天会有很多的货物需要通过这个网络进行运输，所以管理员小J需要制订每天的运输计</div>
<div>划，当然，他就需要知道某个货物从生产地运送到某个运输站的最短延时。</div>
<div>为了简化问题，假设所有货物的生产地在0号运输站，所有的运输站形成了一个分层结构，第1</div>
<div>层有n个运输站，第2层有n-1个运输站……第n层有1个运输站，小J用(i，j)表示第i层的第</div>
<div>j个运输站，注意i&lt;=j&lt;n，因为第2层没有第1个运输站，第3层没有第1，2个运输站，以此类</div>
<div>推。这个网络的结构比较奇怪。0号运输站通过一条j类型的单向运输线与（1，j）相连；当i&gt;l时，</div>
<div>运输站(i-l，j-l)和运输站(i-1，j）通过两条j类型的单向运输线与运输站（i，j）相连。对于所</div>
<div>有i&gt;=l，货物只能够从第i-l层向第i层运输。</div>
<div>令天有m个货物需要运输，小T想要知道每个货物到达目的地的最短延时，他找到了Nick帮</div>
<div>忙，由于Nick没带电脑，所以这个光荣而艰巨的任务就交给你啦！</div>
<div></div>
<p></p></div>

# Input

<div class="content"><div>
<div>第1行2个正整数n，m，表示运输线的种类数和今天运输的货物个数。</div>
<div>第2行共n个非负整数，数与数之间用空格隔开，第i个数Pi表示第i种运输线的延时。</div>
<div>第3～m+2行，每行两个正整数xi，Yi，表示第i个货物需要运送到运输站(xi，Yi)。</div>
<div>注意：为了防止离线算法的出现，本题将对输入文件进行加密。假设第i-l组询问的答案为ans，</div>
<div>则第i组实际询问的xi&#39;，yi&#39;为给定的xi，yi对ans进行异或操作得到的结果，即，xi&#39;=xi xor ans</div>
<div>yi=yi xor ans，实际的询问为xi&#39;,yi&#39;。特别地，对于i=1，ans=0。</div>
<div>N,M&lt;=10^5,0&lt;=Pi&lt;=20000,1&lt;=xi&#39;&lt;=yi&#39;&lt;=N</div>
</div>
<div></div>
<div></div></div>

# Output

<div class="content"><div>共m行，每行一个非负整数，第i行表示第i个货物的最短延时</div>
<div></div>
<p></p></div>

# Sample Input

<div class="content"><span class="sampledata">6 4 <br/>
2 2 3 4 3 4 <br/>
4 5 <br/>
15 8 <br/>
10 13<br/>
11 10</span></div>

# Sample Output

<div class="content"><span class="sampledata">9<br/>
9<br/>
5<br/>
//对于第一组样例，第1组询问的答案为12，第二组询问由于15 xor 12=3<br/>
8 xor 12=4,所以实际的询问为(3,4),答案为9</span></div>

# Hint

<div class="content"><p></p></div>

# Source

<div class="content"><p><a href="problemset.php?search="></a></p></div>

