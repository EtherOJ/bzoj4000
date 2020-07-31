
# Description

<div class="content"><div>
<div>如果一个字符串可以被拆分为 AABBAABB 的形式，其中 AA 和 BB 是任意非空字符串，则我们称该字符串的这种拆</div>
<div>分是优秀的。例如，对于字符串 aabaabaa，如果令 A=aabA=aab，B=aB=a，我们就找到了这个字符串拆分成 AABBA</div>
<div>ABB 的一种方式。一个字符串可能没有优秀的拆分，也可能存在不止一种优秀的拆分。比如我们令 A=aA=a，B=baa</div>
<div>B=baa，也可以用 AABBAABB 表示出上述字符串；但是，字符串 abaabaa 就没有优秀的拆分。现在给出一个长度为</div>
<div> nn 的字符串 SS，我们需要求出，在它所有子串的所有拆分方式中，优秀拆分的总个数。这里的子串是指字符串</div>
<div>中连续的一段。以下事项需要注意：出现在不同位置的相同子串，我们认为是不同的子串，它们的优秀拆分均会被</div>
<div>记入答案。在一个拆分中，允许出现 A=BA=B。例如 cccc 存在拆分 A=B=cA=B=c。字符串本身也是它的一个子串。</div>
<div></div>
</div>
<div></div></div>

# Input

<div class="content"><div>每个输入文件包含多组数据。输入文件的第一行只有一个整数 TT，表示数据的组数。保证 1≤T≤101≤T≤10。接</div>
<div>下来 TT 行，每行包含一个仅由英文小写字母构成的字符串 SS，意义如题所述。</div></div>

# Output

<div class="content"><p>输出 TT 行，每行包含一个整数，表示字符串 SS 所有子串的所有拆分中，总共有多少个是优秀的拆分。</p></div>

# Sample Input

<div class="content"><span class="sampledata">4<br/>
aabbbb<br/>
cccccc<br/>
aabaabaabaa<br/>
bbaabaababaaba</span></div>

# Sample Output

<div class="content"><span class="sampledata">3<br/>
5<br/>
4<br/>
7<br/>
我们用 S[i,j]S[i,j] 表示字符串 SS 第 ii 个字符到第 jj 个字符的子串（从 11 开始计数）。第一组数据中，<br/>
共有 33 个子串存在优秀的拆分：S[1,4]=aabbS[1,4]=aabb，优秀的拆分为 A=aA=a，B=bB=b；S[3,6]=bbbbS[3,6]<br/>
=bbbb，优秀的拆分为 A=bA=b，B=bB=b；S[1,6]=aabbbbS[1,6]=aabbbb，优秀的拆分为 A=aA=a，B=bbB=bb。而剩<br/>
下的子串不存在优秀的拆分，所以第一组数据的答案是 33。第二组数据中，有两类，总共 44 个子串存在优秀的<br/>
拆分：对于子串 S[1,4]=S[2,5]=S[3,6]=ccccS[1,4]=S[2,5]=S[3,6]=cccc，它们优秀的拆分相同，均为 A=cA=c，<br/>
B=cB=c，但由于这些子串位置不同，因此要计算 33 次；对于子串 S[1,6]=ccccccS[1,6]=cccccc，它优秀的拆分<br/>
有 22 种：A=cA=c，B=ccB=cc 和 A=ccA=cc，B=cB=c，它们是相同子串的不同拆分，也都要计入答案。所以第二组<br/>
数据的答案是 3+2=53+2=5。第三组数据中，S[1,8]S[1,8] 和 S[4,11]S[4,11] 各有 22 种优秀的拆分，其中 S[1<br/>
,8]S[1,8] 是问题描述中的例子，所以答案是 2+2=42+2=4。第四组数据中，S[1,4]S[1,4]，S[6,11]S[6,11]，S[7<br/>
,12]S[7,12]，S[2,11]S[2,11]，S[1,8]S[1,8] 各有 11 种优秀的拆分，S[3,14]S[3,14] 有 22 种优秀的拆分，<br/>
所以答案是 5+2=75+2=7。</span></div>

# Hint

<div class="content"><p></p></div>

# Source

<div class="content"><p><a href="problemset.php?search="></a></p></div>

