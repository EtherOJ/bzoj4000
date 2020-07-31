
# Description

<div class="content"><div>农夫约翰决定他的家里需要更多的装饰。通过参观当地的瓷器商店，他决定购买一个精致的玻璃牛雕像，他知道它</div>
<div>将完全适合放在壁炉上方的壁炉架上。牛雕像的形状由一个N×M的字符网格（就像下图）描述（3≤N，M≤500），</div>
<div>其中小写字母描述了雕像的每个部分（表示不同的颜色），&#39;.&#39;字符则不是。</div>
<div></div>
<div>...............</div>
<div>...............</div>
<div>x..x...........</div>
<div>xxxx...........</div>
<div>xxxxaaaaaaa...</div>
<div>.xx.aaaaaaaaa..</div>
<div>....aaaaaaa.aa.</div>
<div>....ll...ll....</div>
<div>....vv...vv....</div>
<div>...............</div>
<div></div>
<div>不幸的是，在FJ正准备购买之前，一头公牛穿过商店，不仅打破了FJ的雕像，而且还打破了货架上的许多其他玻璃</div>
<div>制品！ FJ的雕像碎成了3片，很快地散落在总共有K块碎片的地面上（4≤K≤100）。每块碎片由一个字符网格描述</div>
<div>，就像描述原来的雕像那样。请帮助FJ确定多少个3块碎片的集合（落在地板上的K块碎片中的其中3块）可以胶合</div>
<div>在一起修补成他的破碎的雕像。地面上的碎片可能已经水平或垂直翻转，或者旋转成了90度的几倍。因此，给定原</div>
<div>始网格以及描述K块碎片的网格，您需要找到3片碎片可以连接在一起以形成原始图像的集合，允许这些碎片被平移</div>
<div>，翻转或旋转90度的倍数。然后当叠加时，3个碎片应该准确地形成原始图形，原始图形中的每个彩色正方形正好</div>
<div>表示其中一片。</div>
<div></div></div>

# Input

<div class="content"><div>第一行包含单个整数K,接下来有K+1个描述片段，第一个片段描述了原始的玻璃牛，剩下的K个片段描述了K块碎片。</div>
<div>对于每个描述片段，第一行包含两个整数R和C（1≤R，C≤100），接下来R行每行C个小写字母或者是&#39;.&#39;。</div>
<div>每个碎片都将被水平/垂直连接并且具有至少一个非空单元（即至少包含一个小写字母）。</div>
<div></div></div>

# Output

<div class="content"><div>
<div>输出三元组i，j，k的数目（i &lt;j &lt;k），使得碎片i，j，k可以被拼接为原始的玻璃牛。</div>
</div>
<p></p></div>

# Sample Input

<div class="content"><span class="sampledata">5<br/>
5 5<br/>
aaaaa<br/>
..a..<br/>
bbabb<br/>
..a..<br/>
aaaaa<br/>
3 5<br/>
..abb<br/>
..a..<br/>
aaaaa<br/>
5 2<br/>
a.<br/>
a.<br/>
aa<br/>
a.<br/>
a.<br/>
1 2<br/>
bb<br/>
1 5<br/>
bbabb<br/>
2 5<br/>
aaaaa<br/>
..a..</span></div>

# Sample Output

<div class="content"><span class="sampledata">3<br/>
//共有三个解决方案，分别使用碎片（1,2,3），（1,3,5），（2,4,5）。</span></div>

# Hint

<div class="content"><p></p></div>

# Source

<div class="content"><p><a href="problemset.php?search=Platinum 鸣谢g1n0st提供译文">Platinum 鸣谢g1n0st提供译文</a></p></div>

