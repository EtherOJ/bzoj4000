
# Description

<div class="content"><div>YDC将给你n个字符串，并要求进行q次操作，每次操作形如一下四种：</div>
<div>0.在第x个字符串后面加上一个字符y。</div>
<div>1.询问在第k个操作过后的第y个字符串在当前的第x个字符串中的出现次数。</div>
<div>2.将第x个字符串改成第y个字符串。</div>
<div>3.读入一个字符串，询问它在n个串中每一个串中的出现次数</div>
<div>这里的出现次数是特殊定义的，比如说询问串s1中s2的出现次数，那么询问时会给出参数l,r，需要回答s1有多少子串形如a+s2（&#39;+&#39;号代表字符串连接），其中a是一个字符集中在第[l,r]中的字符。不同的询问所给出的l,r可能不同。</div>
<div>另外输入文件可能被加密。</div>
<div></div>
<p></p></div>

# Input

<div class="content"><div>第一行三个整数数，n,m,ty，分别表示字符串个数，字符集大小，以及是否数据是否被加密，如果数据被加密，则ty的值为1，否则为0。</div>
<div>如果数据被加密，令lastans为当前操作之前最后一个输出的数（如果此前没有输出则lastans=0）。那么当前操作中读入的所有数均被加密成了原数异或上lastans（即假设原数为x，你读入的数将是x^lastans）。</div>
<div>接下来n行，第i行将给出第i个字符串。字符串将按照如下格式给出：第一个数len表示字符串的长度，接下来len个整数，两两之间用空格隔开，表示每个位置上的字符是字符集中的第几个（从0开始标号）。</div>
<div>再读入一个数q，即操作数。</div>
<div>接着q行，每行为一个操作的信息。每行第一个数为操作的类型。</div>
<div>如果是操作0，那么接着两个整数x,y，含义如题所示。</div>
<div>如果是操作1，那么接着五个整数x,y,k,l,r，其中l,r表示出现次数中所要求的l,r。（当k=0时表示所有操作进行之前）</div>
<div>如果是操作2，那么接着两个整数x,y，含义如题所示。</div>
<div>如果是操作3，那么接着两个整数l,r和一个字符串s，字符串的格式和上述相同。</div>
<div></div>
<p></p></div>

# Output

<div class="content"><div>对于每一个操作1和3，你都需要输出他们的答案。你需要确保你的输出顺序与读入顺序一致。</div>
<div></div>
<p></p></div>

# Sample Input

<div class="content"><span class="sampledata">3 3 0<br/>
5 0 1 1 1 2<br/>
1 1<br/>
2 1 1<br/>
4<br/>
0 1 1<br/>
3 0 1 1 1<br/>
2 2 1<br/>
1 1 2 0 0 1</span></div>

# Sample Output

<div class="content"><span class="sampledata">3 0 1<br/>
3</span></div>

# Hint

<div class="content"><p></p><div>2&lt;=n&lt;=5,1&lt;=m&lt;=10^5,0&lt;=q&lt;=2*10^5.</div><br/>
<div>初始n个串的总长度不超过2*10^5+20.</div><br/>
<div>操作3中读入的串总长度不超过10^6.</div><br/>
<div>保证数据合法。</div><br/>
<div>保证任意时刻出现的n个串均是一个长度不超过4*10^5的字符串的子串。</div><br/>
<div>对于前30%的数据，保证q&lt;=1000,初始n个串的总长度不超过1000+20，操作3中读入的串总长度不超过10^4.</div><br/>
<div>对于前60%的数据，保证所有的l=0,r=m-1.</div><br/>
<div>对于前80%的数据，保证数据没有被加密。</div><br/>
<p></p><p></p></div>

# Source

<div class="content"><p><a href="problemset.php?search=2015年集训队互测">2015年集训队互测</a></p></div>

