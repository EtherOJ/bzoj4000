
# Description

<div class="content"><div>神犇Aleph在SDOI Round2前立了一个flag：如果进了省队，就现场直播喝崂山白花蛇草水。凭借着神犇Aleph的实</div>
<div>力，他轻松地进了山东省省队，现在便是他履行诺言的时候了。蒟蒻Bob特地为他准备了999,999,999,999,999,999</div>
<div>瓶崂山白花蛇草水，想要灌神犇Aleph。神犇Aleph求（跪着的）蒟蒻Bob不要灌他，由于神犇Aleph是神犇，蒟蒻Bo</div>
<div>b最终答应了他的请求，但蒟蒻Bob决定将计就计，也让神犇Aleph回答一些问题。具体说来，蒟蒻Bob会在一个宽敞</div>
<div>的广场上放置一些崂山白花蛇草水（可视为二维平面上的一些整点），然后询问神犇Aleph在矩形区域(x1, y1), (</div>
<div>x2, y2)(x1≤x2且y1≤y2，包括边界)中，崂山白花蛇草水瓶数第k多的是多少。为了避免麻烦，蒟蒻Bob不会在同</div>
<div>一个位置放置两次或两次以上的崂山白花蛇草水，但蒟蒻Bob想为难一下神犇Aleph，希望他能在每次询问时立刻回</div>
<div>答出答案。神犇Aleph不屑于做这种问题，所以把这个问题交给了你。</div>
<p></p></div>

# Input

<div class="content"><div>输入的第一行为两个正整数N, Q，表示横纵坐标的范围和蒟蒻Bob的操作次数（包括放置次数和询问次数）。</div>
<div>接下来Q行，每行代表蒟蒻Bob的一个操作，操作格式如下：</div>
<div>首先第一个数字type，表示操作种类。type=1表示放置，type=2表示询问。</div>
<div>若type=1，接下来会有三个正整数x, y, v，表示在坐标整点(x, y)放置v瓶崂山白花蛇草水。(1≤x, y≤N, 1≤v≤10^9)</div>
<div>若type=2，接下来会有五个正整数x1, y1, x2, y2, k，表示询问矩形区域(x1, y1), (x2, y2)中，崂山白花蛇草水瓶数第k多的是多少。</div>
<div>(1≤x1≤x2≤N，1≤y1≤y2≤N，1≤k≤Q)</div>
<div>为了体现程序的在线性，你需要将每次读入的数据（除了type值）都异或lastans，其中lastans表示上次询问的答</div>
<div>案。如果上次询问的答案为&#34;NAIVE!ORZzyz.&#34;（见样例输出），则将lastans置为0。初始时的lastans为0。</div>
<div>初始时平面上不存在崂山白花蛇草水。</div>
<div>
<div>本题共有12组测试数据。对于所有的数据，N≤500,000。</div>
<div>Q的范围见下表：</div>
<div>测试点1-2     Q=1,000</div>
<div>测试点3-7     Q=50,000</div>
<div>测试点8-12     Q=100,000</div>
</div>
<div></div>
<div></div>
<p></p></div>

# Output

<div class="content"><div>对于每个询问(type=2的操作)，回答崂山白花蛇草水瓶数第k多的是多少。若不存在第k多的瓶数，</div>
<div>请输出&#34;NAIVE!ORZzyz.&#34;（输出不含双引号）。</div>
<p></p></div>

# Sample Input

<div class="content"><span class="sampledata">10 7<br/>
1 1 1 1<br/>
1 2 2 3<br/>
1 4 1 2<br/>
1 3 4 4<br/>
2 1 1 4 1 3<br/>
2 2 2 3 5 4<br/>
2 2 1 4 4 2</span></div>

# Sample Output

<div class="content"><span class="sampledata">NAIVE!ORZzyz.<br/>
NAIVE!ORZzyz.<br/>
3</span></div>

# Hint

<div class="content"><p></p></div>

# Source

<div class="content"><p><a href="problemset.php?search=Idea By Aleph, Description &amp; Data cases By jinlifu1999.
">Idea By Aleph, Description &amp; Data cases By jinlifu1999.<br/>
</a></p></div>

