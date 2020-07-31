
# Description

<div class="content"><div>Having become bored with standard 2-dimensional artwork (and also frustrated at others copying her w</div>
<div>ork), the great bovine artist Picowso has decided to switch to a more minimalist, 1-dimensional styl</div>
<div>e.Although, her paintings can now be described by a 1-dimensional array of colors of length N(1≤N≤</div>
<div>100,000), her painting style remains unchanged: she starts with a blank canvas and layers upon it a </div>
<div>sequence of &#34;rectangles&#34; of paint, which in this 1-dimensional case are simply intervals. Sheuses ea</div>
<div>ch of the colors 1…Nexactly once, although just as before, some colors might end up being completel</div>
<div>y covered up by the end.To Picowso&#39;s great dismay, her competitor Moonet seems to have figured out h</div>
<div>ow to copy even these 1-dimensional paintings, using a similar strategy to the preceding problem: Mo</div>
<div>onet will paint a set ofdisjoint intervals, wait for them to dry, then paint another set of disjoint</div>
<div> intervals, and so on.Moonet can only paint at most one interval of each color over the entire proce</div>
<div>ss. Please compute thenumber of such rounds needed for Moonet to copy a given 1-dimensional Picowso </div>
<div>painting.</div>
<div>
<div>
<div>伟大的牛艺术家皮科沃已经厌倦了标准的二维艺术作品，也在伤心其他人复制她的作品，她决定转向更简约，一维</div>
<div>的风格。尽管如此,她的作品现在可以表示描述颜色的一维数组长度N(1≤N≤100000)，她的绘画风格没有改变:她</div>
<div>以一个空白的画布开始，一次涂色只能涂上连续几个单位的颜料，同样新的颜料可以完全覆盖旧的颜料，每次涂完</div>
<div>要等上1day才能完全干，只有旧颜料干了以后才能用新颜料覆盖。皮科沃十分沮丧的是，她的对手Moonet似乎已经</div>
<div>找到了如何复制这些一维的绘画，使用类似的策略。前面的问题：Moonet会画几组不相交区间，等待他们干，然后</div>
<div>画几组不相交区间，等等。Moonet同一种颜色只能使用一次。请计算该轮Moonet复制一个给定的一维picowso绘画</div>
<div>所需要的时间。</div>
<div></div>
</div>
</div>
<div></div>
<p></p></div>

# Input

<div class="content"><div>The first line of input contains N, and the next N lines contain an integer in the range 0…N</div>
<div>indicating the color of each cell in the 1-dimensional painting (0 for a blank cell).</div>
<div>
<div>第一行为N，画条长度</div>
<div>从第2行至N行每行一个数表示要涂颜色</div>
</div>
<div></div>
<p></p></div>

# Output

<div class="content"><div>Please output the minimum number of rounds needed to copy this painting, or -1 if this could not hav</div>
<div>e possibly been an authentic work of Picowso (i.e., if she could not have painted it using a layered</div>
<div> sequence of intervals, one of each color).</div>
<div>输出一个整数表示最少天数。数据若不合法则输出-1</div>
<div></div>
<div></div>
<p></p></div>

# Sample Input

<div class="content"><span class="sampledata">7<br/>
0<br/>
1<br/>
4<br/>
5<br/>
1<br/>
3<br/>
3</span></div>

# Sample Output

<div class="content"><span class="sampledata">2<br/>
In this example, the interval of color 1 must be painted in an earlier round than the intervals of c<br/>
olors 4 and 5, so at least two rounds are needed.</span></div>

# Hint

<div class="content"><p></p></div>

# Source

<div class="content"><p><a href="problemset.php?search=Gold">Gold</a></p></div>

