# Competitive Programming Template
by oko._.11
---
## 總分類索引

<!-- PAGE_INDEX_START -->
| 章節 | 分類名稱 | 包含模板內容 | 市賽重要度 | 雙欄版頁碼 | 單欄版頁碼 |
| :--- | :--- | :--- | :--- | :---: | :---: |
| **0** | **起手式與舊版 C++ 備案** | 0.1 個人模板、0.2 備用標頭檔、0.3 舊版 C++11/98 替換、0.4 組裝示範、0.5 PBDS | `[必背]` | **P. 02** | **P. 04** |
| **1** | **數學與數論** | 1.1 快速冪/龜速乘/逆元、1.2 exgcd、1.3 線性篩、1.4 組合數、1.5 矩陣快速冪、1.6 歐拉函數、1.7 大數 Bigint | `[必背]` | **P. 04** | **P. 07** |
| **2** | **基礎演算法與技巧** | 2.1 對答案二分搜、2.2 二維前綴和與差分、2.3 單調佇列與堆疊、2.4 逆序數對/區間合併/河內塔、2.5 離散化 | `[必背]` | **P. 07** | **P. 12** |
| **3** | **資料結構** | 3.1 DSU、3.2 BIT、3.3 RangeBIT、3.4 SparseTable、3.5 線段樹、3.6 懶標線段樹、3.7 FHQ-Treap、3.8 莫隊 | `[必背]` | **P. 09** | **P. 16** |
| **4** | **動態規劃 (DP)** | 4.1 背包全集、4.2 LIS、4.3 LCS 與編輯距離、4.4 區間 DP、4.5 樹直徑、4.6 狀壓 DP、4.7 數位 DP | `[必背]` | **P. 13** | **P. 23** |
| **5** | **圖論：最短路徑** | 5.1 網格迷宮 BFS 與 0-1 BFS、5.2 Dijkstra (含路徑還原)、5.3 SPFA (判負環)、5.4 Floyd-Warshall | `[必背]` | **P. 15** | **P. 26** |
| **6** | **圖論：MST／DAG／樹** | 6.1 Kruskal 與 Prim、6.2 拓樸排序、6.3 倍增 LCA、6.4 樹壓平 Euler Tour、6.5 重鏈剖分 HLD | `[必背]` | **P. 16** | **P. 29** |
| **7** | **圖論：連通分量／歐拉** | 7.1 Tarjan SCC (縮點)、7.2 Kosaraju、7.3 Lowlink (橋/割點/EBCC)、7.4 VBCC、7.5 歐拉路徑/迴路 | `[常考]` | **P. 19** | **P. 33** |
| **8** | **圖論：匹配／流／邏輯** | 8.1 二分圖判定、8.2 Kuhn 與 Hopcroft-Karp、8.3 最大流最小割 Dinic、8.4 費用流 MCMF、8.5 2-SAT | `[進階]` | **P. 21** | **P. 38** |
| **9** | **字串演算法** | 9.1 雙模 Rolling Hash、9.2 KMP、9.3 Z-function、9.4 Manacher 最長回文、9.5 Trie 與 0-1 Trie | `[常考]` | **P. 24** | **P. 42** |
| **10** | **計算幾何 2D** | 10.1 點向量、轉向 ccw、線段相交、多邊形面積、凸包 Convex Hull | `[常考]` | **P. 25** | **P. 45** |
| **11** | **C++ STL 函式速查字典** | 11.1 vector/string、11.2 queue/stack/pq、11.3 set/multiset/map、11.4 algorithm/數學/位元/格式 | `[必備查表]` | **P. 26** | **P. 46** |

### 詳細演算法頁碼速查索引

| 小節演算法 | 雙欄頁碼 | 單欄頁碼 | 小節演算法 | 雙欄頁碼 | 單欄頁碼 |
| :--- | :---: | :---: | :--- | :---: | :---: |
| 0.1 你的個人起手式模板（原封不動版） | **P. 02** | P. 04 | 4.7 數位 DP 萬用記憶化搜尋骨架 | **P. 14** | P. 26 |
| 0.2 備用標準標頭檔清單（當 `#include"bits/stdc++.h"` 無法編譯時替換第 1 行） | **P. 03** | P. 06 | 5.1 網格迷宮 `BFS`（搭配你的 `gridc`、`grid`、`dr`、`dc`）＆ `0-1 BFS` | **P. 15** | P. 26 |
| 0.3 舊版 C++（C++11／無 `auto`／舊版 Dev-C++）設定與語法替換指南 | **P. 04** | P. 06 | 5.2 `Dijkstra`（非負權單源最短路 ＋ 路徑還原） | **P. 15** | P. 27 |
| 0.4 完整組裝示範：怎麼把這份講義的模板放進你的程式碼？ | **P. 04** | P. 07 | 5.3 `SPFA`（含負權邊最短路 ＋ 判負環） | **P. 16** | P. 28 |
| 0.5 PBDS 進階紅黑樹 `ordered_set`（動態查排名與第 $k$ 小） | **P. 04** | P. 07 | 5.4 `Floyd-Warshall`（全點對最短路） | **P. 16** | P. 29 |
| 1.1 快速冪 `qpow`、龜速乘 `qmul`、模逆元、模除法 | **P. 04** | P. 08 | 6.1 `Kruskal` ＆ `Prim` 最小生成樹 (MST) | **P. 16** | P. 29 |
| 1.2 擴展歐幾里得 `exgcd` ＆ 任意模數逆元 | **P. 05** | P. 08 | 6.2 拓樸排序 `topo_sort`（DAG 排順序／判有向環／DAG DP） | **P. 17** | P. 30 |
| 1.3 線性篩質數 `Sieve` ＋ $O(\log x)$ 快速質因數分解 | **P. 05** | P. 09 | 6.3 最近共同祖先 `LCA`（倍增法：查祖先、查樹上兩點距離） | **P. 17** | P. 31 |
| 1.4 組合數預處理 `Comb`（$C^a_b, P^a_b \bmod p$） | **P. 05** | P. 09 | 6.4 樹壓平 `Euler Tour`（把整棵子樹轉成連續區間配 `BIT`／線段樹） | **P. 18** | P. 31 |
| 1.5 矩陣快速冪 `Mat` | **P. 06** | P. 10 | 6.5 重鏈剖分 `HLD`（樹上任意兩點路徑修改／查詢） | **P. 18** | P. 32 |
| 1.6 歐拉函數 $\varphi(n)$ | **P. 06** | P. 10 | 7.1 `TarjanSCC`（有向圖強連通分量 ＋ 縮點成 DAG） | **P. 19** | P. 33 |
| 1.7 大數運算 `Bigint`（純 C++11 相容、支援正負加減乘與除以整數） | **P. 06** | P. 11 | 7.2 `Kosaraju`（兩次 DFS 求 SCC 備用版） | **P. 19** | P. 34 |
| 2.1 對答案二分搜（永不無窮迴圈寫法） | **P. 07** | P. 12 | 7.3 無向圖 `Lowlink`：橋、割點、邊雙連通分量 (EBCC) | **P. 20** | P. 35 |
| 2.2 二維前綴和 `Prefix2D` ＆ 二維差分 `Diff2D` | **P. 07** | P. 13 | 7.4 點雙連通分量 `VBCC` | **P. 20** | P. 36 |
| 2.3 單調佇列（滑動視窗極值）＆ 單調堆疊（下一個更大元素） | **P. 08** | P. 14 | 7.5 歐拉路徑／歐拉迴路 `Euler`（無向圖＆有向圖一筆畫） | **P. 20** | P. 36 |
| 2.4 Merge Sort 求逆序數對 ＆ 區間合併 ＆ 河內塔 | **P. 08** | P. 15 | 8.1 二分圖判定（黑白塗色判奇環） | **P. 21** | P. 38 |
| 2.5 離散化（搭配你的 `mkunique` 與 `lb` 巨集只要 3 行！） | **P. 09** | P. 15 | 8.2 二分圖最大匹配：`Kuhn` ($O(VE)$) ＆ `HopcroftKarp` ($O(E\sqrt{V})$) | **P. 22** | P. 38 |
| 3.1 並查集 `DSU` (Disjoint Set Union) | **P. 09** | P. 16 | 8.3 最大流／最小割 `Dinic` | **P. 22** | P. 39 |
| 3.2 樹狀數組 `BIT` (Fenwick Tree) | **P. 09** | P. 16 | 8.4 最小費用最大流 `MCMF` | **P. 23** | P. 40 |
| 3.3 區間加值、區間求和 `RangeBIT` | **P. 10** | P. 17 | 8.5 `2-SAT`（二元布林條件滿足問題） | **P. 23** | P. 41 |
| 3.4 稀疏表 `SparseTable`（靜態區間最大／最小／GCD） | **P. 10** | P. 18 | 9.1 雙模數 `DoubleHash`（直接使用你的 `mod1` 與 `mod2`！） | **P. 24** | P. 42 |
| 3.5 一般線段樹 `SegTree`（單點修改＋區間總和／最大／最小） | **P. 10** | P. 18 | 9.2 `KMP` 字串匹配與最小週期 | **P. 24** | P. 43 |
| 3.6 懶標記線段樹 `LazySegTree`（區間加值＋區間設值＋區間極值與總和） | **P. 11** | P. 19 | 9.3 `Z-function`（擴展 KMP：求每個後綴與原字串的最長共同前綴） | **P. 24** | P. 43 |
| 3.7 無旋平衡樹 `FHQTreap`（區間翻轉／序列剪貼） | **P. 12** | P. 21 | 9.4 `Manacher` 最長回文子字串 | **P. 25** | P. 44 |
| 3.8 莫隊演算法 `Mo's Algorithm`（離線區間查詢） | **P. 12** | P. 22 | 9.5 字典樹 `Trie` ＆ `XorTrie`（最大 XOR 配對） | **P. 25** | P. 44 |
| 4.1 背包問題全集（0/1 背包、無限背包、有限背包） | **P. 13** | P. 23 | 10.1 點向量、轉向判定 `ccw`、線段相交、多邊形面積、凸包 `Convex Hull` | **P. 25** | P. 45 |
| 4.2 最長遞增子序列 `LIS`（直接搭配你的 `lb` / `ub` 巨集） | **P. 13** | P. 23 | 11.1 `vector` 與 `string` 與字元／字串轉型 | **P. 26** | P. 46 |
| 4.3 `LCS` 最長共同子序列 ＆ 編輯距離 (Edit Distance) | **P. 13** | P. 24 | 11.2 `queue`、`stack`、`deque`、`priority_queue`（堆） | **P. 26** | P. 47 |
| 4.4 區間 DP 標準骨架（相鄰石子合併最小代價） | **P. 14** | P. 24 | 11.3 `set`、`multiset`、`map`（紅黑樹容器與不用 `auto` 的迭代器寫法） | **P. 26** | P. 47 |
| 4.5 樹形 DP ＆ 樹直徑（樹上最遠兩點距離） | **P. 14** | P. 25 | 11.4 `<algorithm>`、`<numeric>`、`<cmath>`、位元與輸出格式全表 | **P. 27** | P. 48 |
| 4.6 狀態壓縮 DP（Bitmask TSP 最短路徑 ＆ 子集枚舉） | **P. 14** | P. 25 | | | |
<!-- PAGE_INDEX_END -->

---

## 三大實戰速查表

### A. 由題目數據範圍 $N$ 反推演算法複雜度（C++ 每秒約可跑 $10^8$ 次運算）

| 題目給的 $N$ 上限 | 安全時間複雜度 | 常見對應演算法 |
| :--- | :--- | :--- |
| $N \le 10$ | $O(N!)$ | `next_permutation` 全排列、DFS 暴力窮舉 |
| $N \le 20$ | $O(2^N)$ 或 $O(N^2 2^N)$ | 位元枚舉（Bitmask）、4.6 狀態壓縮 DP |
| $N \le 40$ | $O(2^{N/2})$ | 折半枚舉（拆成左右兩半各 $2^{20}$，排序後用 `lb` 二分搜湊答案） |
| $N \le 400 \sim 500$ | $O(N^3)$ | 5.4 `Floyd-Warshall`、4.4 區間 DP、矩陣乘法 |
| $N \le 5000$ | $O(N^2)$ | 2D DP、4.1 背包問題 $O(NW)$、樹上背包 |
| $N \le 2 \times 10^5$（你的 `N`） | $O(N \log N)$ 或 $O(N \log^2 N)$ | `sort`、二分搜、`BIT`、線段樹、`Dijkstra`、`Kruskal`、`LCA` |
| $N \le 10^6 \sim 5 \times 10^6$ | $O(N)$ | 前綴差分、單調佇列、線性篩、`KMP`／`Z`／`Manacher` |
| $N \le 10^{18}$ | $O(\log N)$ 或 $O(\sqrt{N})$ | 1.1 快速冪、1.5 矩陣快速冪、4.7 數位 DP、數學公式 |

### B. 資料結構快速選擇表

| 你想做的操作 | 選哪個模板？ | 時間複雜度 | 備註 |
| :--- | :--- | :--- | :--- |
| 合併兩群人、問兩點是否連通、問群大小 | 3.1 `DSU` | $O(\alpha(N))$ | 只支援加邊合併，不支援刪邊 |
| 單點加值 ＋ 查區間總和 | 3.2 `BIT` | $O(\log N)$ | 程式碼最短（15 行），優先用它別寫線段樹 |
| 區間加值 ＋ 查區間總和（不問最大最小） | 3.3 `RangeBIT` | $O(\log N)$ | 兩個 `BIT` 搞定，免寫懶標線段樹 |
| 陣列完全不修改，大量查區間最大／最小／GCD | 3.4 `SparseTable` | 建 $O(N\log N)$，查 $O(1)$ | 不能修改元素，不可查區間和 |
| 單點修改 ＋ 查區間最大／最小／總和 | 3.5 `SegTree` | $O(\log N)$ | 改 `merge_node` 即可換功能 |
| 區間加值／區間統一設值 ＋ 查區間極值或總和 | 3.6 `LazySegTree` | $O(\log N)$ | 同時支援 `range_add` 與 `range_set` |
| 動態插入刪除數字 ＋ 查第 $k$ 小／有幾個 $< x$ | 0.5 `ordered_set` | $O(\log N)$ | GNU PBDS 紅黑樹 |
| 區間整段翻轉 `[l, r]` | 3.7 `FHQ-Treap` | $O(\log N)$ | 無旋 Treap |

### C. 圖論快速選擇表

| 題目場景 | 選哪個模板？ | 時間複雜度 | 關鍵限制／提醒 |
| :--- | :--- | :--- | :--- |
| 網格迷宮上下左右每步距離 `1` | 5.1 網格 `BFS` | $O(NM)$ | 直接搭配你模板的 `dr[]`, `dc[]`, `grid` |
| 邊權只有 `0` 或 `1` 的最短路 | 5.1 `bfs01` | $O(V+E)$ | 用 `deque`，權重 `0` 放頭、`1` 放尾 |
| 單一起點最短路（**邊權皆 $\ge 0$**） | 5.2 `dijkstra` | $O((V+E)\log V)$ | **絕對不可有負權邊**；若總距離 $>10^{17}$ 記得把 `inf` 改 `4e18` |
| 單一起點最短路（**有負權邊**）或**判負環** | 5.3 `spfa` | 最壞 $O(VE)$ | 正權圖請用 `dijkstra`，勿用 `spfa` |
| 任意兩點最短路（點數 $V \le 400$） | 5.4 `Floyd-Warshall` | $O(V^3)$ | 中繼點 `k` 迴圈必須在最外層 |
| 最小總成本連通所有點（最小生成樹） | 6.1 `kruskal` | $O(E \log E)$ | 搭配 3.1 `DSU` 最快寫完 |
| 工作先後順序、排合法順序、判有向環 | 6.2 `topo_sort` | $O(V+E)$ | 若要求字典序最小，`queue` 改用你的 `rp_q` |
| 樹上查最近共同祖先、樹上兩點距離 | 6.3 `LCA` | 建 $O(V\log V)$，查 $O(\log V)$ | 樹上距離 $= \text{dep}[u]+\text{dep}[v]-2\text{dep}[\text{lca}]$ |
| 有向圖把「互相可達的點」縮成一顆點 | 7.1 `TarjanSCC` | $O(V+E)$ | 縮點後必為 DAG，常接 DP |
| 無向圖找「斷掉就不連通的橋／割點」 | 7.3 `Lowlink` | $O(V+E)$ | 內建支援重邊 |
| 一筆畫問題（每條邊恰走一次） | 7.5 `Euler` | $O(V+E)$ | 無向圖奇數度點只能有 `0` 或 `2` 個 |
| 左邊配右邊最多幾對（無權二分圖匹配） | 8.2 `Kuhn` / `HopcroftKarp` | $O(VE)$ / $O(E\sqrt{V})$ | 小圖用 `Kuhn`；大圖用 `HopcroftKarp` |
| 最大流量／最小代價切斷起終點（最小割） | 8.3 `Dinic` | $O(V^2 E)$ | 最大流數值 $=$ 最小割數值 |
| 布林開關限制（A 或 B 至少一成立） | 8.5 `TwoSat` | $O(V+E)$ | 需先貼 7.1 `TarjanSCC` |

---

## 0. 個人起手式與舊版 C++ 備案

### 0.1 你的個人起手式模板

```cpp
#include"bits/stdc++.h"
using namespace std;

#pragma GCC optimize("Ofast,fast-math,unroll-loops")
#pragma GCC target("sse,sse2,sse3,ssse3,sse4,popcnt,abm,mmx,avx,avx2,tune=native")

#define pb push_back
#define int long long
#define ll long long
#define ull unsigned long long
#define vec vector<ll>
#define p_q priority_queue<ll>
#define rp_q priority_queue<ll, vec, greater<ll>>
#define grid(n, m, name) vector<vector<ll>> name(n, vector<ll>(m))
#define gridc(n, m, name) vector<vector<char>> name(n, vector<char>(m))
#define pii pair<ll,ll>
#define fi first
#define se second
#define be(x) x.begin(),x.end()
#define rbe(x) x.rbegin(),x.rend()
#define mkunique(x) sort(be(x));(x).erase(unique(be(x)),(x).end());
#define lb(x, v) lower_bound(be((x)), (v)) - (x).begin()
#define ub(x, v) upper_bound(be((x)), (v)) - (x).begin()
#define Yes cout << "Yes\n"
#define No cout << "No\n"
#define YES cout << "YES\n"
#define NO cout << "NO\n"
#define oko_11 cin.tie(0)->sync_with_stdio(0)
#define cerr if(1) cerr
 
const int N = 2e5 + 5;
const ll inf = 1e17 + 5;
const int mod1 = 1e9 + 7;
const int mod2 = 998244353;
const int dr[] = {1, -1, 0, 0};
const int dc[] = {0, 0, 1, -1};
const int dr8[] = {1, 1, 1, 0, -1, -1, -1, 0};
const int dc8[] = {1, 0, -1, -1, -1, 0, 1, 1};

int gcd(int n, int m){
    return m ? gcd(m, n % m) : n;
}

int lcm(int a, int b) {
    return (a / gcd(a, b)) * b;
}

void voids(){

    cout << "\n";
}

int ints(int n){
    return 0;
}

signed main(){
    oko_11;
    int T = 1;
    //cin >> T;
    for(int i = 0; i < T; i++){
        //cout << "Case #" << i + 1 << " ";
        //int n;
        //cin >> n;
        voids();
        // ints(n);
    }
    return 0;
}
```

#### 你的模板巨集與常數快速對照（整份講義都會直接用這些縮寫！）

- **型別與容器**：`int` 與 `ll` 都是 64 位元整數；`vec` 是 `vector<ll>`；`pii` 是 `pair<ll,ll>`（用 `.fi` 取第一個、`.se` 取第二個）；`pb` 是 `push_back`。
- **優先佇列（堆）**：`p_q` 是大根堆（每次 `.top()` 取最大值）；`rp_q` 是小根堆（每次 `.top()` 取最小值）。
- **二維陣列**：`grid(n + 1, m + 1, a);` 直接建出 `(n+1) x (m+1)` 初值為 `0` 的二維 `ll` 陣列 `a`；`gridc(n, m, g);` 建二維字元陣列 `g`。
- **排序／去重／二分搜**：
  - `sort(be(a));` 由小到大排；`sort(rbe(a));` 由大到小排。
  - `mkunique(a);` 自動排序並刪除重複元素（離散化神器！）。
  - `lb(a, v)`：在**已排序**的 `a` 中找第一個 `>= v` 的位置（`0-based` 下標，同時等於 `< v` 的元素個數）。
  - `ub(a, v)`：在**已排序**的 `a` 中找第一個 `> v` 的位置（`0-based` 下標，同時等於 `<= v` 的元素個數）。
- **網格方向陣列**：`dr[0..3]` 與 `dc[0..3]` 為上下左右 4 方向；`dr8[0..7]` 與 `dc8[0..7]` 為含斜角 8 方向。
- **三個實戰小細節**：
  1. 在你自己的 Apple Silicon Mac 編譯時，若第 5 行 `#pragma GCC target("sse,...")` 報錯，在 Mac 本機註解掉第 5 行即可（比賽現場的 Windows/Linux x86 電腦支援該行）。
  2. `inf = 1e17 + 5`：一般題目非常安全且 `inf + inf` 不溢位；若遇到極端最短路總和可能超過 $10^{17}$，把 `inf` 改成 `4e18` 即可。
  3. 下面部分模板會用到 `lg2(x)`（求 $\lfloor \log_2 x \rfloor$），只要在 `lcm` 下方加一行：`int lg2(int x) { return x <= 1 ? 0 : 63 - __builtin_clzll(x); }` 即可。

---

### 0.2 備用標準標頭檔清單（當 `#include"bits/stdc++.h"` 無法編譯時替換第 1 行）

如果比賽環境（或學校電腦、Mac 預設 Clang）出現 `'bits/stdc++.h' file not found`，把第 1 行換成下面這組標準標頭檔即可：

```cpp
// === 所有 C++ 版本 (含 C++98 / C++11) 皆支援的核心標頭檔 ===
#include <iostream>
#include <cstdio>
#include <cstdlib>
#include <cmath>
#include <cstring>
#include <climits>
#include <cctype>
#include <cassert>
#include <iomanip>
#include <sstream>
#include <string>
#include <vector>
#include <deque>
#include <queue>
#include <stack>
#include <set>
#include <map>
#include <bitset>
#include <algorithm>
#include <numeric>
#include <functional>
#include <utility>

// === C++11 以上支援的標頭檔 (若編譯器未開 -std=c++11 報錯，刪掉這兩行即可) ===
#include <unordered_set>
#include <unordered_map>
#include <tuple>
```

---

### 0.3 舊版 C++（C++11／無 `auto`／舊版 Dev-C++）設定與語法替換指南

#### 第一招：進考場先花 5 秒在 IDE 開啟 C++11 / C++14！
學校電腦如果是舊版 **Dev-C++**，預設沒開 C++11 會連你的模板第 11 行 `>>` 與第 25 行 `cin.tie(0)->` 都編不過！請立刻打開：
- **Dev-C++**：上方選單 `工具 (Tools)` -> `編譯器選項 (Compiler Options)` -> 勾選「編譯時加入以下命令」填入 `-std=c++11`（若支援可填 `-std=c++14`）。
- **Code::Blocks**：`Settings` -> `Compiler` -> `Compiler flags` -> 勾選 `Have g++ follow the C++11 ISO C++ language standard [-std=c++11]`。

#### 第二招：新舊 C++ 語法替換對照表（本講義所有模板皆已改寫為「零 `auto`」純 C++11 寫法！）

| 新版寫法（舊編譯器會報錯） | 相容舊版 C++11 / C++98 的安全寫法 |
| :--- | :--- |
| `auto [d, u] = pq.top();` *(C++17 專用)* | `pii top = pq.top(); int d = top.fi, u = top.se;` |
| `auto it = st.lower_bound(x);` *(需 `auto`)* | `set<int>::iterator it = st.lower_bound(x);` |
| `for (auto [k, v] : mp)` *(C++17 專用)* | `for (map<int,int>::iterator it = mp.begin(); it != mp.end(); ++it)` 用 `it->fi`, `it->se` |
| `for (int x : v)` *(C++11 範圍迴圈，C++98 不支援)* | `for (int i = 0; i < (int)v.size(); i++) { int x = v[i]; }` |
| `auto dfs = [&](auto &self, int u)` *(C++14 專用)* | 直接把 `void dfs(int u)` 寫成 `voids()` 上方的一般函式（最穩最快！） |
| `pq.push({d, v});` *(C++11 大括號轉 pair)* | `pq.push(make_pair(d, v));`（連 C++98 都能過！） |
| `vector<vector<ll>>` *(C++98 會把 `>>` 當位元右移)* | 若沒開 C++11，兩個 `>` 中間加一個空白：`vector<vector<ll> >` |
| `(__int128)a * b % m` *(32 位元舊編譯器無 `__int128`)* | `mod1`/`mod2` 直接 `a * b % m` 不會溢位；超大模數用 1.1 的 `qmul(a, b, m)` |
| `cin.tie(0)->sync_with_stdio(0)` *(C++98 若報錯)* | 改成 `ios_base::sync_with_stdio(0); cin.tie(0);` |

---

### 0.4 完整組裝示範：怎麼把這份講義的模板放進你的程式碼？

下面示範當題目問「有 $n$ 個人、$m$ 次交朋友，問最後分成幾群人」時，你的完整檔案長什麼樣子：

```cpp
// [步驟 1] 保留你的個人模板上半部 (省略重複顯示，從 #include 到 lcm 完全不動)

// [步驟 2] 把講義裡的 struct 或函式貼在 voids() 的「正上方」！
struct DSU {
    vec pa, sz_v;
    int comps;
    DSU(int n) : pa(n + 1), sz_v(n + 1, 1), comps(n) { iota(be(pa), 0); }
    int find(int x) { return pa[x] == x ? x : pa[x] = find(pa[x]); }
    bool unite(int a, int b) {
        a = find(a); b = find(b);
        if (a == b) return false;
        if (sz_v[a] < sz_v[b]) swap(a, b);
        pa[b] = a; sz_v[a] += sz_v[b]; comps--;
        return true;
    }
};

// [步驟 3] 在你的 voids() 裡面讀輸入、呼叫模板、印出答案！
void voids(){
    int n, m;
    cin >> n >> m;
    DSU dsu(n);                  // 建立 1 ~ n 的並查集
    for (int i = 0; i < m; i++) {
        int u, v;
        cin >> u >> v;
        dsu.unite(u, v);         // 把 u 與 v 合併成同一群
    }
    cout << dsu.comps << "\n";   // 印出最後有幾個連通塊 (注意：已自己印 "\n")
}
// [步驟 4] 下方的 ints(n) 與 signed main() 維持你原本的寫法即可 (多筆測資把 //cin >> T; 打開)
```

---

### 0.5 PBDS 進階紅黑樹 `ordered_set`（動態查排名與第 $k$ 小）

- **何時用**：需要 `set` 動態插入刪除，又要 $O(\log N)$ 查「嚴格小於 $x$ 有幾個」或「第 $k$ 小是誰」（僅限 GNU C++）。

```cpp
#include <ext/pb_ds/assoc_container.hpp>
#include <ext/pb_ds/tree_policy.hpp>
using namespace __gnu_pbds;

typedef tree<int, null_type, less<int>, rb_tree_tag, tree_order_statistics_node_update> ordered_set;
// 若允許重複元素，把 int 改成 pii，插入 make_pair(數值, 時間編號 i)！

void voids() {
    ordered_set st;
    st.insert(10); st.insert(20); st.insert(30);
    cout << st.order_of_key(20) << "\n";    // 嚴格小於 20 的元素數量 -> 印出 1
    cout << *st.find_by_order(0) << "\n";   // 第 k 小的值 (0-based，k=0 為最小) -> 印出 10
}
```

---

## 1. 數學與數論 (Math & Number Theory)

> 提醒：你的模板已經內建 `gcd(a, b)` 與 `lcm(a, b)`，以及 `mod1 = 1e9 + 7`、`mod2 = 998244353`，可直接呼叫！

### 1.1 快速冪 `qpow`、龜速乘 `qmul`、模逆元、模除法｜$O(\log b)$

- **何時用**：算 $a^b \bmod m$，或算分數 $\frac{a}{b} \bmod p$（`mod_inv` / `mod_div` 要求模數 `p` **必須是質數**，如 `mod1` 或 `mod2`）。

```cpp
// 龜速乘：只有當模數 m > 3e9 (導致 a * a 超過 9e18 溢位) 時才需要用！一般 mod1/mod2 不用貼
int qmul(int a, int b, int m) {
    int res = 0;
    a = (a % m + m) % m; b = (b % m + m) % m;
    while (b > 0) {
        if (b & 1) res = (res + a) % m;
        a = (a + a) % m;
        b >>= 1;
    }
    return res;
}

// 快速冪：計算 a 的 b 次方對 m 取模 (預設 m = mod1 = 1e9 + 7)
int qpow(int a, int b, int m = mod1) {
    int res = 1 % m;
    a = (a % m + m) % m;             // 防止 a 是負數或超過 m
    while (b > 0) {
        if (b & 1) res = res * a % m; // 若 m > 3e9 改成 qmul(res, a, m)
        a = a * a % m;                // 若 m > 3e9 改成 qmul(a, a, m)
        b >>= 1;
    }
    return res;
}

// 費馬小定理求模逆元 (p 必須為質數，且 a % p != 0)
int mod_inv(int a, int p = mod1) { return qpow(a, p - 2, p); }

// 模除法：計算 (a / b) % p
int mod_div(int a, int b, int p = mod1) {
    return ((a % p + p) % p) * mod_inv(b, p) % p;
}

// === 實戰呼叫範例 ===
void voids() {
    int a, b;
    cin >> a >> b;
    cout << qpow(a, b, mod1) << "\n";   // 印出 a^b % (10^9+7)
    cout << mod_div(a, b, mod2) << "\n";// 印出 (a / b) % 998244353
}
```

---

### 1.2 擴展歐幾里得 `exgcd` ＆ 任意模數逆元｜$O(\log \min(a,b))$

- **何時用**：解整數方程式 $ax + by = \gcd(a, b)$ 的一組整數解 $(x, y)$；或當模數 $m$ **不是質數**時求模逆元。

```cpp
// 傳入 a, b，透過參考變數 x, y 寫入一組解使得 a*x + b*y == gcd(a, b)，並回傳 gcd
int exgcd(int a, int b, int &x, int &y) {
    if (b == 0) { x = 1; y = 0; return a; }
    int g = exgcd(b, a % b, y, x);
    y -= (a / b) * x;
    return g;
}

// 求 a 在模 m 下的逆元 (m 不必是質數，只要 gcd(a, m) == 1 就有解；無解回傳 -1)
int inv_any(int a, int m) {
    int x, y;
    if (exgcd(a, m, x, y) != 1) return -1;
    return (x % m + m) % m;
}

// === 實戰呼叫範例 ===
void voids() {
    int a = 3, m = 10;
    int inv = inv_any(a, m); // 找 3 * inv % 10 == 1 -> 得到 7
    if (inv == -1) No;
    else cout << inv << "\n";
}
```

---

### 1.3 線性篩質數 `Sieve` ＋ $O(\log x)$ 快速質因數分解｜預處理 $O(n)$

- **何時用**：建 $1 \sim n$ 質數表（$n \le 10^7$），或對大量數字快速質因數分解。
- **補充**：若只對**單一個大數** $x \le 10^{12}$ 做質因數分解，不要建表，直接寫 `for (int i = 2; i * i <= x; i++) while (x % i == 0) { ... x /= i; } if (x > 1) ...` 即可！

```cpp
struct Sieve {
    int n;
    vec primes;             // 存放篩出來的所有質數 (2, 3, 5, 7, ...)
    vec spf;                // spf[x] = x 的最小質因數 (Smallest Prime Factor)
    vector<bool> is_prime;  // is_prime[x] = x 是否為質數

    Sieve(int n) : n(n), spf(n + 1, 0), is_prime(n + 1, true) {
        is_prime[0] = is_prime[1] = false;
        for (int i = 2; i <= n; i++) {
            if (is_prime[i]) { primes.pb(i); spf[i] = i; }
            for (int j = 0; j < (int)primes.size(); j++) {
                int p = primes[j];
                if (i * p > n) break;
                is_prime[i * p] = false;
                spf[i * p] = p;
                if (i % p == 0) break; // 保證每個合數只被最小質因數篩掉一次 -> O(n)
            }
        }
    }
    // 將 x (1 <= x <= n) 質因數分解，回傳 {(質因數, 次方), ...}
    vector<pii> factorize(int x) {
        vector<pii> res;
        while (x > 1) {
            int p = spf[x], cnt = 0;
            while (x % p == 0) { x /= p; cnt++; }
            res.pb(make_pair(p, cnt));
        }
        return res;
    }
};

// === 實戰呼叫範例 (注意：多筆測資時，請把 Sieve 建在 main 或全域避免重複建表！) ===
void voids() {
    Sieve sv(1000000);                  // 預處理 1 ~ 10^6
    if (sv.is_prime[97]) Yes;           // O(1) 判斷 97 是否為質數
    vector<pii> f = sv.factorize(72);   // 72 = 2^3 * 3^2 -> {(2, 3), (3, 2)}
    for (int i = 0; i < (int)f.size(); i++) {
        cout << f[i].fi << "^" << f[i].se << " ";
    }
    cout << "\n";
}
```

---

### 1.4 組合數預處理 `Comb`（$C^a_b, P^a_b \bmod p$）｜建表 $O(n)$，查詢 $O(1)$

- **何時用**：排列組合題，需先貼上 1.1 的 `qpow`（模數 `mod` 必須是質數，預設 `mod1`）。

```cpp
struct Comb {
    int n, mod;
    vec fact, invf; // fact[i] = i! % mod, invf[i] = (i!)^(-1) % mod
    Comb(int n, int mod = mod1) : n(n), mod(mod), fact(n + 1), invf(n + 1) {
        fact[0] = 1;
        for (int i = 1; i <= n; i++) fact[i] = fact[i - 1] * i % mod;
        invf[n] = qpow(fact[n], mod - 2, mod);
        for (int i = n - 1; i >= 0; i--) invf[i] = invf[i + 1] * (i + 1) % mod;
    }
    int C(int a, int b) { // 從 a 個選 b 個的方法數 C(a, b)
        if (b < 0 || b > a) return 0;
        return fact[a] * invf[b] % mod * invf[a - b] % mod;
    }
    int P(int a, int b) { // 從 a 個選 b 個排成一列的方法數 P(a, b)
        if (b < 0 || b > a) return 0;
        return fact[a] * invf[a - b] % mod;
    }
};

// === 實戰呼叫範例 ===
void voids() {
    Comb cb(N, mod1);               // 直接用你模板的 N = 2e5 + 5 建表！
    cout << cb.C(10, 3) << "\n";    // 印出 120
    // 小技巧：重複組合 H(n, k) (n 種物品可重複選 k 個) 等於 cb.C(n + k - 1, k)
}
```

---

### 1.5 矩陣快速冪 `Mat`｜$O(K^3 \log P)$

- **何時用**：
  1. $n$ 高達 $10^{18}$ 的線性遞迴（如費氏數列 $F_n = F_{n-1} + F_{n-2}$）。
  2. 有向圖給鄰接矩陣 `G`，問從點 `u` 走**恰好 $P$ 步**到點 `v` 有幾種走法（算 `mpow(G, P).a[u][v]`）。

```cpp
struct Mat {
    int n;
    vector<vec> a;
    // ident = true 時建立對角線為 1 的單位矩陣，否則全為 0
    Mat(int n, bool ident = false) : n(n), a(n, vec(n, 0)) {
        if (ident) for (int i = 0; i < n; i++) a[i][i] = 1;
    }
    Mat operator*(const Mat &o) const {
        Mat res(n);
        for (int i = 0; i < n; i++)
            for (int k = 0; k < n; k++) if (a[i][k])
                for (int j = 0; j < n; j++)
                    res.a[i][j] = (res.a[i][j] + a[i][k] * o.a[k][j]) % mod1;
        return res;
    }
};

Mat mpow(Mat base, int p) { // 計算矩陣 base 的 p 次方
    Mat res(base.n, true);
    while (p > 0) {
        if (p & 1) res = res * base;
        base = base * base;
        p >>= 1;
    }
    return res;
}

// === 實戰呼叫範例：求費氏數列第 n 項 F(n) (F(0)=0, F(1)=1, n <= 10^18) ===
void voids() {
    int n;
    cin >> n;
    Mat T(2); // 轉移矩陣 [1 1; 1 0]
    T.a[0][0] = 1; T.a[0][1] = 1;
    T.a[1][0] = 1; T.a[1][1] = 0;
    Mat R = mpow(T, n);
    cout << R.a[0][1] << "\n"; // F(n) % mod1
}
```

---

### 1.6 歐拉函數 $\varphi(n)$｜$O(\sqrt{n})$

- **何時用**：計算 $1 \sim n$ 中與 $n$ 互質的整數個數。

```cpp
int euler_phi(int n) {
    int res = n;
    for (int i = 2; i * i <= n; i++) {
        if (n % i == 0) {
            while (n % i == 0) n /= i;
            res -= res / i;
        }
    }
    if (n > 1) res -= res / n;
    return res;
}
```

---

### 1.7 大數運算 `Bigint`（純 C++11 相容、支援正負加減乘與除以整數）

- **何時用**：數字超過 `long long`（$> 9 \times 10^{18}$）且題目**沒有給模數**必須精確輸出所有位數時。

```cpp
struct Bigint {
    static const int BASE = 1000000000; // 每格存 9 位十進位數字 (10^9)
    vec d;                              // 低位存在前面 (d[0] 為個位~億位)
    int sign;                           // +1 為正或零，-1 為負

    Bigint(int v = 0) : sign(1) { *this = v; }
    Bigint(const string &s) : sign(1) { read(s); }

    Bigint& operator=(int v) {
        sign = 1; d.clear();
        if (v < 0) { sign = -1; v = -v; }
        for (; v > 0; v /= BASE) d.pb(v % BASE);
        return *this;
    }
    void trim() {
        while (!d.empty() && d.back() == 0) d.pop_back();
        if (d.empty()) sign = 1;
    }
    void read(const string &s) {
        sign = 1; d.clear();
        int pos = 0, len = (int)s.size();
        while (pos < len && (s[pos] == '-' || s[pos] == '+')) {
            if (s[pos] == '-') sign = -sign;
            pos++;
        }
        for (int i = len - 1; i >= pos; i -= 9) {
            int x = 0;
            for (int j = max(pos, i - 8); j <= i; j++) x = x * 10 + (s[j] - '0');
            d.pb(x);
        }
        trim();
    }
    string str() const { // 轉成字串供 cout 輸出
        if (d.empty()) return "0";
        stringstream ss;
        if (sign == -1) ss << '-';
        ss << d.back();
        for (int i = (int)d.size() - 2; i >= 0; i--)
            ss << setw(9) << setfill('0') << d[i];
        return ss.str();
    }
    static int cmp_abs(const Bigint &a, const Bigint &b) {
        if (a.d.size() != b.d.size()) return a.d.size() < b.d.size() ? -1 : 1;
        for (int i = (int)a.d.size() - 1; i >= 0; i--)
            if (a.d[i] != b.d[i]) return a.d[i] < b.d[i] ? -1 : 1;
        return 0;
    }
    bool operator<(const Bigint &o) const {
        if (sign != o.sign) return sign < o.sign;
        return sign == 1 ? cmp_abs(*this, o) < 0 : cmp_abs(*this, o) > 0;
    }
    bool operator==(const Bigint &o) const { return sign == o.sign && d == o.d; }
    Bigint operator-() const { Bigint r = *this; if (!r.d.empty()) r.sign = -r.sign; return r; }

    static Bigint add_abs(const Bigint &a, const Bigint &b) {
        Bigint r; r.d.assign(max(a.d.size(), b.d.size()) + 1, 0);
        for (int i = 0; i < (int)r.d.size() - 1; i++) {
            if (i < (int)a.d.size()) r.d[i] += a.d[i];
            if (i < (int)b.d.size()) r.d[i] += b.d[i];
            if (r.d[i] >= BASE) { r.d[i] -= BASE; r.d[i + 1]++; }
        }
        r.trim(); return r;
    }
    static Bigint sub_abs(const Bigint &a, const Bigint &b) {
        Bigint r = a;
        for (int i = 0; i < (int)b.d.size(); i++) r.d[i] -= b.d[i];
        for (int i = 0; i < (int)r.d.size(); i++)
            if (r.d[i] < 0) { r.d[i] += BASE; r.d[i + 1]--; }
        r.trim(); return r;
    }
    Bigint operator+(const Bigint &o) const {
        if (sign == o.sign) { Bigint r = add_abs(*this, o); r.sign = sign; r.trim(); return r; }
        if (cmp_abs(*this, o) >= 0) { Bigint r = sub_abs(*this, o); r.sign = sign; r.trim(); return r; }
        Bigint r = sub_abs(o, *this); r.sign = o.sign; r.trim(); return r;
    }
    Bigint operator-(const Bigint &o) const { return *this + (-o); }
    Bigint operator*(const Bigint &o) const {
        Bigint r; r.d.assign(d.size() + o.d.size(), 0); r.sign = sign * o.sign;
        for (int i = 0; i < (int)d.size(); i++) {
            int carry = 0;
            for (int j = 0; j < (int)o.d.size() || carry; j++) {
                ll cur = r.d[i + j] + d[i] * (j < (int)o.d.size() ? o.d[j] : 0LL) + carry;
                r.d[i + j] = cur % BASE;
                carry = cur / BASE;
            }
        }
        r.trim(); return r;
    }
    // 大數除以一般整數 v (|v| <= 8*10^9)，回傳 {商, 餘數}
    pair<Bigint, int> divmod(int v) const {
        Bigint r = *this;
        if (v < 0) { r.sign = -r.sign; v = -v; }
        ll rem = 0;
        for (int i = (int)r.d.size() - 1; i >= 0; i--) {
            ll cur = r.d[i] + rem * BASE;
            r.d[i] = cur / v;
            rem = cur % v;
        }
        r.trim();
        return make_pair(r, rem * sign);
    }
};

// === 實戰呼叫範例 ===
void voids() {
    string s1, s2;
    cin >> s1 >> s2;
    Bigint a(s1), b(s2);
    cout << (a + b).str() << "\n";        // 大數加法
    cout << (a - b).str() << "\n";        // 大數減法 (自動處理負號)
    cout << (a * b).str() << "\n";        // 大數乘法
    pair<Bigint, int> qr = a.divmod(7);   // 大數除以整數 7
    cout << qr.fi.str() << " " << qr.se << "\n"; // 印出 商 與 餘數
}
```

---

## 2. 基礎演算法與核心技巧 (Basic Techniques)

### 2.1 對答案二分搜（永不無窮迴圈寫法）｜$O(\log R \cdot T(\text{check}))$

- **何時用**：看到題目問 **「最小的最大值」**（例如：最大負擔最少是多少？）或 **「最大的最小值」**（例如：兩點最短距離最大可以是多少？），只要寫得出 `bool check(int mid)` 判斷某個答案 `mid` 做不做得到，就能二分搜答案！

```cpp
// 假設這題問：把陣列 a 分成最多 k 段，每段總和「上限 mid」最少要多少才夠分？
bool check(int mid, const vec &a, int k) {
    int parts = 1, cur_sum = 0;
    for (int i = 0; i < (int)a.size(); i++) {
        if (a[i] > mid) return false;       // 單一元素就超過 mid，絕對不可能
        if (cur_sum + a[i] > mid) {         // 裝不下就換下一段
            parts++;
            cur_sum = a[i];
        } else {
            cur_sum += a[i];
        }
    }
    return parts <= k;                      // 段數 <= k 代表 mid 足夠大 (可行)
}

void voids() {
    int n, k;
    cin >> n >> k;
    vec a(n);
    for (int i = 0; i < n; i++) cin >> a[i];

    // [情況 A] 找「最小」的可行答案 (false, false, ..., true, true)
    int lo = 0, hi = inf, ans = -1;
    while (lo <= hi) {
        int mid = lo + (hi - lo) / 2;
        if (check(mid, a, k)) {
            ans = mid;      // mid 可行！先記下答案，往左邊試試能不能更小
            hi = mid - 1;
        } else {
            lo = mid + 1;   // mid 太小不可行，往右邊找
        }
    }
    cout << ans << "\n";

    // [情況 B] 若題目是找「最大」的可行答案 (true, true, ..., false, false)：
    // 把 if 裡面改成：ans = mid; lo = mid + 1; 並把 else 改成：hi = mid - 1; 即可！

    // [情況 C] 浮點數二分搜：固定跑 100 次迴圈，精確度達 10^-18 且絕不 TLE！
    // double l = 0.0, r = 1e9;
    // for (int it = 0; it < 100; it++) {
    //     double m = (l + r) / 2.0;
    //     if (check_double(m)) r = m; else l = m;
    // }
}
```

---

### 2.2 二維前綴和 `Prefix2D` ＆ 二維差分 `Diff2D`｜`1-based`｜建表 $O(nm)$，單次 $O(1)$

- **何時用**：
  - `Prefix2D`：矩陣固定不變，詢問很多次「左上 `(r1, c1)` 到右下 `(r2, c2)` 的子矩陣總和」。
  - `Diff2D`：先對很多個子矩陣 `(r1, c1) ~ (r2, c2)` 整塊加值，**全部加完之後**才一次算出最終矩陣。
- **補充（一維前綴和與差分）**：一維前綴和 `s[i] = s[i-1] + a[i]`，區間和 `[l, r]` 為 `s[r] - s[l-1]`；一維差分在 `[l, r]` 加 `v` 為 `d[l] += v; d[r+1] -= v;`，最後對 `d` 做前綴和即還原。

```cpp
struct Prefix2D {
    vector<vec> s;
    // 傳入 1-based 二維陣列 a (大小至少 (n+1) x (m+1))
    Prefix2D(int n, int m, const vector<vec> &a) : s(n + 1, vec(m + 1, 0)) {
        for (int i = 1; i <= n; i++)
            for (int j = 1; j <= m; j++)
                s[i][j] = a[i][j] + s[i - 1][j] + s[i][j - 1] - s[i - 1][j - 1];
    }
    // O(1) 查詢左上 (r1, c1) 到右下 (r2, c2) 閉區間總和 (1-based)
    int query(int r1, int c1, int r2, int c2) {
        return s[r2][c2] - s[r1 - 1][c2] - s[r2][c1 - 1] + s[r1 - 1][c1 - 1];
    }
};

struct Diff2D {
    int n, m;
    vector<vec> d;
    Diff2D(int n, int m) : n(n), m(m), d(n + 2, vec(m + 2, 0)) {}
    // O(1) 將子矩陣 (r1, c1) ~ (r2, c2) 每個格子加上 val (1-based)
    void add(int r1, int c1, int r2, int c2, int val) {
        d[r1][c1] += val;
        d[r1][c2 + 1] -= val;
        d[r2 + 1][c1] -= val;
        d[r2 + 1][c2 + 1] += val;
    }
    // 所有 add 結束後呼叫 build()，回傳 1-based 最終矩陣 a[1..n][1..m]
    vector<vec> build() {
        grid(n + 1, m + 1, a); // 使用你模板的 grid 巨集！
        for (int i = 1; i <= n; i++)
            for (int j = 1; j <= m; j++)
                a[i][j] = d[i][j] + a[i - 1][j] + a[i][j - 1] - a[i - 1][j - 1];
        return a;
    }
};

// === 實戰呼叫範例 ===
void voids() {
    int n, m, q;
    cin >> n >> m >> q;
    grid(n + 1, m + 1, a); // 建立 (n+1) x (m+1) 的 1-based 矩陣
    for (int i = 1; i <= n; i++)
        for (int j = 1; j <= m; j++) cin >> a[i][j];

    Prefix2D pref(n, m, a);
    while (q--) {
        int r1, c1, r2, c2;
        cin >> r1 >> c1 >> r2 >> c2;
        cout << pref.query(r1, c1, r2, c2) << "\n";
    }
}
```

---

### 2.3 單調佇列（滑動視窗極值）＆ 單調堆疊（下一個更大元素）｜`0-based`｜$O(n)$

- **何時用**：
  - `sliding_max`：長度固定為 $k$ 的視窗從左滑到右，求每個視窗的最大值（求最小值只要把 `<=` 改成 `>=`）。
  - `next_greater`：求每個元素右邊第一個嚴格比它大的位置（找不到為 `-1`）。

```cpp
// 回傳共 (n - k + 1) 個數字，代表每個長度 k 視窗的最大值
vec sliding_max(const vec &a, int k) {
    deque<int> dq; // 裡面存陣列下標 index，且對應的 a[index] 保持由大到小
    vec res;
    for (int i = 0; i < (int)a.size(); i++) {
        while (!dq.empty() && dq.front() <= i - k) dq.pop_front(); // 踢掉滑出視窗左界的舊元素
        while (!dq.empty() && a[dq.back()] <= a[i]) dq.pop_back(); // 若改求視窗最小值，把 <= 改成 >=
        dq.pb(i);
        if (i >= k - 1) res.pb(a[dq.front()]); // 隊首永遠是當前視窗的最大值
    }
    return res;
}

// 回傳陣列 ans，ans[i] 為位置 i 右邊第一個滿足 a[j] > a[i] 的下標 j (不存在則為 -1)
vec next_greater(const vec &a) {
    int n = (int)a.size();
    vec ans(n, -1), stk; // stk 當作單調堆疊，存還沒找到答案的 index
    for (int i = 0; i < n; i++) {
        while (!stk.empty() && a[stk.back()] < a[i]) { // 找 >= 改 <=；找更小改 >
            ans[stk.back()] = i;
            stk.pop_back();
        }
        stk.pb(i);
    }
    return ans;
}

// === 實戰呼叫範例 ===
void voids() {
    int n, k;
    cin >> n >> k;
    vec a(n);
    for (int i = 0; i < n; i++) cin >> a[i];
    vec mx = sliding_max(a, k);
    for (int i = 0; i < (int)mx.size(); i++) cout << mx[i] << " ";
    cout << "\n";
}
```

---

### 2.4 Merge Sort 求逆序數對 ＆ 區間合併 ＆ 河內塔

```cpp
// 1. 求逆序數對數量 O(n log n)：計算有幾組 (i < j) 滿足 a[i] > a[j]
// (等價於：只用「相鄰兩數交換」把陣列排成由小到大所需的最少交換次數！)
int merge_inv_dfs(vec &a, vec &tmp, int l, int r) {
    if (r - l <= 1) return 0;
    int mid = (l + r) / 2;
    int inv = merge_inv_dfs(a, tmp, l, mid) + merge_inv_dfs(a, tmp, mid, r);
    int i = l, j = mid, k = l;
    while (i < mid && j < r) {
        if (a[i] <= a[j]) tmp[k++] = a[i++];
        else { tmp[k++] = a[j++]; inv += (mid - i); } // 左半邊 i..mid-1 全部都比 a[j] 大！
    }
    while (i < mid) tmp[k++] = a[i++];
    while (j < r) tmp[k++] = a[j++];
    for (int p = l; p < r; p++) a[p] = tmp[p];
    return inv;
}
int count_inversions(vec a) {
    vec tmp(a.size());
    return merge_inv_dfs(a, tmp, 0, (int)a.size());
}

// 2. 區間合併 O(n log n)：傳入一堆閉區間 {左界, 右界}，把有重疊的合併起來
vector<pii> merge_intervals(vector<pii> segs) {
    if (segs.empty()) return vector<pii>();
    sort(be(segs));
    vector<pii> res;
    res.pb(segs[0]);
    for (int i = 1; i < (int)segs.size(); i++) {
        if (segs[i].fi <= res.back().se) // 若端點剛好相接不算重疊，把 <= 改成 <
            res.back().se = max(res.back().se, segs[i].se);
        else
            res.pb(segs[i]);
    }
    return res;
}

// 3. 河內塔 O(2^n)：將 n 個盤子從柱 A 移到柱 C (輔助柱 B)，總步數為 (1LL << n) - 1
void hanoi(int n, char A, char B, char C) {
    if (n == 0) return;
    hanoi(n - 1, A, C, B);
    cout << A << " " << C << "\n";
    hanoi(n - 1, B, A, C);
}
```

---

### 2.5 離散化（搭配你的 `mkunique` 與 `lb` 巨集只要 3 行！）｜$O(n \log n)$

- **何時用**：數字範圍很大（如 $-10^9 \sim 10^9$），但個數 $n \le 2 \times 10^5$，想塞進 `BIT` 或陣列統計時，把它們換成 `1 ~ m` 的排名！

```cpp
void voids() {
    int n;
    cin >> n;
    vec a(n);
    for (int i = 0; i < n; i++) cin >> a[i];

    vec vals = a;           // 複製一份用來排序去重
    mkunique(vals);         // 你的巨集：自動 sort + unique 去重！
    for (int i = 0; i < n; i++) {
        a[i] = lb(vals, a[i]) + 1; // 你的 lb 巨集回傳 0-based，+1 轉成 1 ~ vals.size()！
    }
    // 現在 a[i] 已經全部變成 1 ~ vals.size() 的正整數，可以直接丟進 BIT 了！
}
```

---

## 3. 資料結構 (Data Structures)

### 3.1 並查集 `DSU` (Disjoint Set Union)｜`0/1-based 皆可`｜$O(\alpha(n))$

- **何時用**：動態合併兩個集合、查詢兩點是否連通、查某點所在連通塊人數、Kruskal 最小生成樹。
- **擴展域並查集技巧（敵人的敵人是朋友／二分圖奇環判定）**：開兩倍大 `DSU dsu(2 * n);`，`1..n` 代表自己，`x + n` 代表與 `x` 不同陣營的人。若題目說 `u` 與 `v` 必須不同邊：先檢查 `if (dsu.same(u, v))` 代表矛盾！否則執行 `dsu.unite(u, v + n); dsu.unite(v, u + n);`。

```cpp
struct DSU {
    vec pa;     // pa[x]: x 的老大 (父節點)
    vec sz_v;   // sz_v[x]: 以 x 為根的集合大小
    int comps;  // 目前共有幾個連通塊 (當點為 1..n 時準確)

    DSU(int n) : pa(n + 1), sz_v(n + 1, 1), comps(n) {
        iota(be(pa), 0); // 初始化 pa[i] = i (每個人一開始自己一國)
    }
    int find(int x) { // 找老大 + 路徑壓縮
        return pa[x] == x ? x : pa[x] = find(pa[x]);
    }
    bool same(int a, int b) { // 判斷 a 和 b 是否在同一群
        return find(a) == find(b);
    }
    bool unite(int a, int b) { // 合併 a 和 b；原本不同群回傳 true，原本同群回傳 false
        a = find(a); b = find(b);
        if (a == b) return false;
        if (sz_v[a] < sz_v[b]) swap(a, b); // 小群併入大群
        pa[b] = a;
        sz_v[a] += sz_v[b];
        comps--;
        return true;
    }
    int size(int x) { return sz_v[find(x)]; } // 查詢 x 所在群組的大小
};

// === 實戰呼叫範例：CSES Road Construction (每加一條路，輸出連通塊數與最大連通塊大小) ===
void voids() {
    int n, m;
    cin >> n >> m;
    DSU dsu(n);
    int max_sz = 1;
    while (m--) {
        int u, v;
        cin >> u >> v;
        if (dsu.unite(u, v)) {
            max_sz = max(max_sz, dsu.size(u));
        }
        cout << dsu.comps << " " << max_sz << "\n";
    }
}
```

---

### 3.2 樹狀數組 `BIT` (Fenwick Tree)｜`[注意] 嚴格 1-based`｜$O(\log n)$

- **何時用**：**單點加值 ＋ 區間總和**，或當作權值桶子查第 $k$ 小。
- **必死地雷**：位置 `i` **絕對不能是 `0`**（傳 `i = 0` 會無限迴圈 TLE）！所有座標請從 `1` 開始編號！

```cpp
// 若需要 kth()，記得在模板上方加這行：
int lg2(int x) { return x <= 1 ? 0 : 63 - __builtin_clzll(x); }

struct BIT {
    int n;
    vec tr;
    BIT(int n) : n(n), tr(n + 1, 0) {}

    // 將第 i 個位置加上 val (注意：是「加上 val」，不是「改成 val」！1 <= i <= n)
    void add(int i, int val) {
        for (; i <= n; i += (i & -i)) tr[i] += val;
    }
    // 查詢前綴和 a[1] + a[2] + ... + a[i]
    int query(int i) {
        int res = 0;
        for (; i > 0; i -= (i & -i)) res += tr[i];
        return res;
    }
    // 查詢閉區間 [l, r] 的總和
    int query(int l, int r) {
        return l > r ? 0 : query(r) - query(l - 1);
    }
    // 當 BIT 內所有元素皆 >= 0 時，O(log n) 找最小的位置 pos 使得 query(pos) >= k (第 k 小)
    int kth(int k) {
        int pos = 0;
        for (int pw = 1LL << lg2(n); pw > 0; pw >>= 1) {
            if (pos + pw <= n && tr[pos + pw] < k) {
                pos += pw;
                k -= tr[pos];
            }
        }
        return pos + 1; // 若回傳 n + 1 代表總和不足 k
    }
};

// === 實戰呼叫範例：單點修改為新值 + 區間求和 ===
void voids() {
    int n, q;
    cin >> n >> q;
    vec a(n + 1);
    BIT bit(n);
    for (int i = 1; i <= n; i++) {
        cin >> a[i];
        bit.add(i, a[i]); // 建表：把初始值加進去
    }
    while (q--) {
        int type;
        cin >> type;
        if (type == 1) {
            int pos, new_val;
            cin >> pos >> new_val;          // 題目要求把 a[pos]「改成」new_val
            bit.add(pos, new_val - a[pos]); // 加上差值！
            a[pos] = new_val;               // 記得同步更新原陣列 a[pos]
        } else {
            int l, r;
            cin >> l >> r;
            cout << bit.query(l, r) << "\n";
        }
    }
}
```

---

### 3.3 區間加值、區間求和 `RangeBIT`｜`[注意] 嚴格 1-based`｜$O(\log n)$

- **何時用**：需要「把區間 `[l, r]` 每個數都 `+ val`」以及「查區間 `[l, r]` 總和」（需先貼上方的 `BIT`）。

```cpp
struct RangeBIT {
    int n;
    BIT b1, b2;
    RangeBIT(int n) : n(n), b1(n + 1), b2(n + 1) {}

    // 將閉區間 [l, r] 內每個位置都加上 val (1 <= l <= r <= n)
    void add(int l, int r, int val) {
        b1.add(l, val);           b1.add(r + 1, -val);
        b2.add(l, val * (l - 1)); b2.add(r + 1, -val * r);
    }
    int prefix(int i) { return b1.query(i) * i - b2.query(i); }
    int query(int l, int r) { return prefix(r) - prefix(l - 1); } // 查詢 [l, r] 總和
};

// === 實戰呼叫範例 ===
void voids() {
    int n, q;
    cin >> n >> q;
    RangeBIT rbit(n);
    for (int i = 1; i <= n; i++) { int x; cin >> x; rbit.add(i, i, x); }
    while (q--) {
        int op; cin >> op;
        if (op == 1) { int l, r, v; cin >> l >> r >> v; rbit.add(l, r, v); }
        else         { int l, r;    cin >> l >> r;      cout << rbit.query(l, r) << "\n"; }
    }
}
```

---

### 3.4 稀疏表 `SparseTable`（靜態區間最大／最小／GCD）｜`1-based`｜建 $O(n\log n)$，查 $O(1)$

- **何時用**：陣列**完全不修改**，詢問數極大（例如 $q = 10^6$ 次查詢區間最大值、最小值或 `gcd`）。

```cpp
int lg2(int x) { return x <= 1 ? 0 : 63 - __builtin_clzll(x); }

struct SparseTable {
    int n;
    vector<vec> st;
    // 想查區間最小值改成 min(a, b)；想查區間最大公因數改成 gcd(a, b)！
    static int op(int a, int b) { return max(a, b); }

    SparseTable(int n, const vec &a) : n(n) { // 傳入 1-based 陣列 a[1..n]
        int lg = lg2(n) + 1;
        st.assign(lg, vec(n + 1));
        for (int i = 1; i <= n; i++) st[0][i] = a[i];
        for (int k = 1; k < lg; k++)
            for (int i = 1; i + (1LL << k) - 1 <= n; i++)
                st[k][i] = op(st[k - 1][i], st[k - 1][i + (1LL << (k - 1))]);
    }
    int query(int l, int r) { // O(1) 查詢閉區間 [l, r]
        int k = lg2(r - l + 1);
        return op(st[k][l], st[k][r - (1LL << k) + 1]);
    }
};

// === 實戰呼叫範例 ===
void voids() {
    int n, q;
    cin >> n >> q;
    vec a(n + 1);
    for (int i = 1; i <= n; i++) cin >> a[i];
    SparseTable rmq(n, a);
    while (q--) {
        int l, r; cin >> l >> r;
        cout << rmq.query(l, r) << "\n";
    }
}
```

---

### 3.5 一般線段樹 `SegTree`（單點修改＋區間總和／最大／最小）｜`1-based`｜$O(\log n)$

- **何時用**：陣列會單點修改，並需要查區間最大、最小、總和（一個結構同時算好這三種，需要哪個就印 `.sum`、`.mx` 或 `.mn`！）。

```cpp
struct SegTree {
    struct Node {
        int sum, mx, mn;
        Node(int s = 0, int x = -inf, int n_v = inf) : sum(s), mx(x), mn(n_v) {}
    };
    // 合併左右子樹資訊：若題目要查區間 GCD，改這裡即可
    static Node merge_node(const Node &a, const Node &b) {
        return Node(a.sum + b.sum, max(a.mx, b.mx), min(a.mn, b.mn));
    }
    int n;
    vector<Node> tr;
    SegTree(int n) : n(n), tr(4 * n + 5) {}
    SegTree(int n, const vec &a) : n(n), tr(4 * n + 5) { build(1, 1, n, a); }

    void build(int id, int l, int r, const vec &a) {
        if (l == r) { tr[id] = Node(a[l], a[l], a[l]); return; }
        int mid = (l + r) / 2;
        build(id * 2, l, mid, a);
        build(id * 2 + 1, mid + 1, r, a);
        tr[id] = merge_node(tr[id * 2], tr[id * 2 + 1]);
    }
    // 將位置 pos 的值「設為」val (若題目是「加上 val」，把 = Node(val...) 改成 tr[id].sum += val 等)
    void update(int id, int l, int r, int pos, int val) {
        if (l == r) { tr[id] = Node(val, val, val); return; }
        int mid = (l + r) / 2;
        if (pos <= mid) update(id * 2, l, mid, pos, val);
        else update(id * 2 + 1, mid + 1, r, pos, val);
        tr[id] = merge_node(tr[id * 2], tr[id * 2 + 1]);
    }
    Node query(int id, int l, int r, int ql, int qr) {
        if (ql <= l && r <= qr) return tr[id];
        int mid = (l + r) / 2;
        if (qr <= mid) return query(id * 2, l, mid, ql, qr);
        if (ql > mid) return query(id * 2 + 1, mid + 1, r, ql, qr);
        return merge_node(query(id * 2, l, mid, ql, qr), query(id * 2 + 1, mid + 1, r, ql, qr));
    }
    // 對外簡化介面：直接呼叫 seg.update(pos, val) 與 seg.query(l, r)
    void update(int pos, int val) { update(1, 1, n, pos, val); }
    Node query(int ql, int qr) { return query(1, 1, n, ql, qr); }
};

// === 實戰呼叫範例 ===
void voids() {
    int n, q;
    cin >> n >> q;
    vec a(n + 1); // 1-based: 讀入 a[1] ~ a[n]
    for (int i = 1; i <= n; i++) cin >> a[i];
    SegTree seg(n, a);

    while (q--) {
        int op, x, y;
        cin >> op >> x >> y;
        if (op == 1) {
            seg.update(x, y);                   // 把 a[x] 改成 y
        } else {
            SegTree::Node ans = seg.query(x, y);// 查詢閉區間 [x, y]
            cout << ans.mn << "\n";             // 印最小值 (也可印 ans.mx 或 ans.sum)
        }
    }
}
```

---

### 3.6 懶標記線段樹 `LazySegTree`（區間加值＋區間設值＋區間極值與總和）｜`1-based`｜$O(\log n)$

- **何時用**：遇到「把 `[l, r]` 整段加 `x`」或「把 `[l, r]` 整段改成 `x`」，還要查區間總和、最大值或最小值！

```cpp
struct LazySegTree {
    struct Node {
        int sum, mx, mn, add, set_val;
        bool has_set;
        Node() : sum(0), mx(-inf), mn(inf), add(0), set_val(0), has_set(false) {}
    };
    int n;
    vector<Node> tr;
    LazySegTree(int n, const vec &a) : n(n), tr(4 * n + 5) {
        build(1, 1, n, a); // a 為 1-based (a[1..n])
    }
    void pull(int id) {
        tr[id].sum = tr[id * 2].sum + tr[id * 2 + 1].sum;
        tr[id].mx = max(tr[id * 2].mx, tr[id * 2 + 1].mx);
        tr[id].mn = min(tr[id * 2].mn, tr[id * 2 + 1].mn);
    }
    void apply_set(int id, int l, int r, int val) { // 整段賦值懶標記
        tr[id].sum = (r - l + 1) * val;
        tr[id].mx = tr[id].mn = val;
        tr[id].set_val = val;
        tr[id].has_set = true;
        tr[id].add = 0; // 賦值會覆蓋掉之前的加值標記
    }
    void apply_add(int id, int l, int r, int val) { // 整段加值懶標記
        tr[id].sum += (r - l + 1) * val;
        tr[id].mx += val;
        tr[id].mn += val;
        if (tr[id].has_set) tr[id].set_val += val;
        else tr[id].add += val;
    }
    void push(int id, int l, int r) { // 把懶標記往下推給左右兒子
        int mid = (l + r) / 2;
        if (tr[id].has_set) {
            apply_set(id * 2, l, mid, tr[id].set_val);
            apply_set(id * 2 + 1, mid + 1, r, tr[id].set_val);
            tr[id].has_set = false;
        }
        if (tr[id].add != 0) {
            apply_add(id * 2, l, mid, tr[id].add);
            apply_add(id * 2 + 1, mid + 1, r, tr[id].add);
            tr[id].add = 0;
        }
    }
    void build(int id, int l, int r, const vec &a) {
        if (l == r) { tr[id].sum = tr[id].mx = tr[id].mn = a[l]; return; }
        int mid = (l + r) / 2;
        build(id * 2, l, mid, a);
        build(id * 2 + 1, mid + 1, r, a);
        pull(id);
    }
    void range_add(int id, int l, int r, int ql, int qr, int val) {
        if (ql <= l && r <= qr) { apply_add(id, l, r, val); return; }
        push(id, l, r);
        int mid = (l + r) / 2;
        if (ql <= mid) range_add(id * 2, l, mid, ql, qr, val);
        if (qr > mid) range_add(id * 2 + 1, mid + 1, r, ql, qr, val);
        pull(id);
    }
    void range_set(int id, int l, int r, int ql, int qr, int val) {
        if (ql <= l && r <= qr) { apply_set(id, l, r, val); return; }
        push(id, l, r);
        int mid = (l + r) / 2;
        if (ql <= mid) range_set(id * 2, l, mid, ql, qr, val);
        if (qr > mid) range_set(id * 2 + 1, mid + 1, r, ql, qr, val);
        pull(id);
    }
    Node query(int id, int l, int r, int ql, int qr) {
        if (ql <= l && r <= qr) return tr[id];
        push(id, l, r);
        int mid = (l + r) / 2;
        if (qr <= mid) return query(id * 2, l, mid, ql, qr);
        if (ql > mid) return query(id * 2 + 1, mid + 1, r, ql, qr);
        Node L = query(id * 2, l, mid, ql, qr);
        Node R = query(id * 2 + 1, mid + 1, r, ql, qr);
        Node res;
        res.sum = L.sum + R.sum;
        res.mx = max(L.mx, R.mx);
        res.mn = min(L.mn, R.mn);
        return res;
    }
    // 對外簡化介面 (全部 1-based 閉區間 [l, r])
    void range_add(int l, int r, int val) { range_add(1, 1, n, l, r, val); }
    void range_set(int l, int r, int val) { range_set(1, 1, n, l, r, val); }
    Node query(int l, int r) { return query(1, 1, n, l, r); }
};

// === 實戰呼叫範例：CSES Range Updates and Sums ===
void voids() {
    int n, q;
    cin >> n >> q;
    vec a(n + 1, 0); // 若初始陣列全為 0，直接傳 vec a(n + 1, 0) 即可！
    for (int i = 1; i <= n; i++) cin >> a[i];
    LazySegTree seg(n, a);

    while (q--) {
        int op, l, r;
        cin >> op >> l >> r;
        if (op == 1)      { int x; cin >> x; seg.range_add(l, r, x); } // [l, r] 全部 +x
        else if (op == 2) { int x; cin >> x; seg.range_set(l, r, x); } // [l, r] 全部設為 x
        else              { cout << seg.query(l, r).sum << "\n"; }     // 查 [l, r] 總和 (.mx/.mn 為極值)
    }
}
```

---

### 3.7 無旋平衡樹 `FHQTreap`（區間翻轉／序列剪貼）｜`1-based`｜$O(\log n)$

- **何時用**：題目要求「把序列第 `l` 到第 `r` 個元素整段反轉」或「把 `[l, r]` 剪下來貼到隊伍最後面」。

```cpp
struct FHQTreap {
    struct Node {
        int l, r, val, sum, sz, pri;
        bool rev;
        Node(int v = 0, int s = 0, int p = 0)
            : l(0), r(0), val(v), sum(v), sz(s), pri(p), rev(false) {}
    };
    vector<Node> tr;
    int root;
    unsigned int seed; // 內建快速亂數，不依賴 C++11 <random>
    FHQTreap() : root(0), seed(1337) { tr.pb(Node(0, 0, 0)); }

    int next_rand() {
        seed ^= seed << 13; seed ^= seed >> 17; seed ^= seed << 5;
        return (int)(seed & 0x7fffffff);
    }
    int new_node(int val) {
        tr.pb(Node(val, 1, next_rand()));
        return (int)tr.size() - 1;
    }
    void pull(int u) {
        if (!u) return;
        tr[u].sz = 1 + tr[tr[u].l].sz + tr[tr[u].r].sz;
        tr[u].sum = tr[u].val + tr[tr[u].l].sum + tr[tr[u].r].sum;
    }
    void apply_rev(int u) {
        if (u) { swap(tr[u].l, tr[u].r); tr[u].rev = !tr[u].rev; }
    }
    void push(int u) {
        if (u && tr[u].rev) {
            apply_rev(tr[u].l); apply_rev(tr[u].r);
            tr[u].rev = false;
        }
    }
    // 將樹 u 按位置切開：前 k 個節點分給 x，剩餘節點分給 y
    void split(int u, int k, int &x, int &y) {
        if (!u) { x = y = 0; return; }
        push(u);
        if (tr[tr[u].l].sz >= k) {
            y = u; split(tr[u].l, k, x, tr[u].l); pull(y);
        } else {
            x = u; split(tr[u].r, k - tr[tr[u].l].sz - 1, tr[u].r, y); pull(x);
        }
    }
    // 將樹 x 與樹 y 左右合併 (前提：x 的所有位置都在 y 左邊)
    int merge_tr(int x, int y) {
        if (!x || !y) return x | y;
        if (tr[x].pri > tr[y].pri) {
            push(x); tr[x].r = merge_tr(tr[x].r, y); pull(x); return x;
        } else {
            push(y); tr[y].l = merge_tr(x, tr[y].l); pull(y); return y;
        }
    }
    void push_back_val(int val) { root = merge_tr(root, new_node(val)); }

    // 將 1-based 閉區間 [l, r] 整段翻轉
    void reverse_range(int l, int r) {
        int a, b, c;
        split(root, r, a, c);
        split(a, l - 1, a, b);
        apply_rev(b);
        root = merge_tr(merge_tr(a, b), c);
    }
    // 查詢 1-based 閉區間 [l, r] 總和
    int query_sum(int l, int r) {
        int a, b, c;
        split(root, r, a, c);
        split(a, l - 1, a, b);
        int ans = tr[b].sum;
        root = merge_tr(merge_tr(a, b), c);
        return ans;
    }
};

// === 實戰呼叫範例 ===
void voids() {
    int n, q;
    cin >> n >> q;
    FHQTreap tp;
    for (int i = 1; i <= n; i++) { int x; cin >> x; tp.push_back_val(x); }
    while (q--) {
        int op, l, r; cin >> op >> l >> r;
        if (op == 1) tp.reverse_range(l, r);
        else         cout << tp.query_sum(l, r) << "\n";
    }
}
```

---

### 3.8 莫隊演算法 `Mo's Algorithm`（離線區間查詢）｜`1-based`｜$O((n + q)\sqrt{n})$

- **何時用**：**沒有修改操作**，可把全部詢問先讀進來排序，且當區間左右端點加減 1 格時能 $O(1)$ 更新答案（例如：問 `[l, r]` 內有幾種不同數字）。

```cpp
int mo_B; // 分塊大小
struct MoQuery {
    int l, r, id;
    bool operator<(const MoQuery &o) const {
        int ba = l / mo_B, bb = o.l / mo_B;
        if (ba != bb) return ba < bb;
        return (ba & 1) ? (r > o.r) : (r < o.r); // 奇偶塊優化
    }
};

void voids() {
    int n, q;
    cin >> n >> q;
    vec a(n + 1);
    for (int i = 1; i <= n; i++) cin >> a[i]; // 若 a[i] > 2e5 請先用 2.5 離散化！

    mo_B = max(1LL, (int)(n / sqrt(max(1LL, q))));
    vector<MoQuery> qs(q);
    for (int i = 0; i < q; i++) {
        cin >> qs[i].l >> qs[i].r;
        qs[i].id = i;
    }
    sort(be(qs));

    vec cnt(N, 0), ans(q);
    int curL = 1, curR = 0, distinct = 0;
    for (int i = 0; i < q; i++) {
        int L = qs[i].l, R = qs[i].r;
        while (curL > L) { curL--; if (++cnt[a[curL]] == 1) distinct++; }
        while (curR < R) { curR++; if (++cnt[a[curR]] == 1) distinct++; }
        while (curL < L) { if (--cnt[a[curL]] == 0) distinct--; curL++; }
        while (curR > R) { if (--cnt[a[curR]] == 0) distinct--; curR--; }
        ans[qs[i].id] = distinct;
    }
    for (int i = 0; i < q; i++) cout << ans[i] << "\n";
}
```

---

## 4. 動態規劃 (Dynamic Programming)

### 4.1 背包問題全集（0/1 背包、無限背包、有限背包）

- **迴圈方向口訣**：
  - **0/1 背包**（每種只有 1 個）：內層容量 `j` **由大到小 (`W -> w`)**。
  - **無限背包**（每種無限多個）：內層容量 `j` **由小到大 (`w -> W`)**。
  - **有限背包**（每種最多拿 `c` 個）：用 `1, 2, 4...` 二進位拆成多個物品，轉成 **0/1 背包**。
  - **超大重量變形**：若容量 $W \le 10^9$ 但總價值 $V_{\text{sum}} \le 10^5$，改開 `vec dp(V_sum + 1, inf); dp[0] = 0;`，算湊出價值 `j` 的**最小重量**，最後找 `dp[j] <= W` 的最大 `j`！

```cpp
// 1. 0/1 背包 O(n * W)：items 存 pii(重量 w, 價值 v)
int knapsack_01(int W, const vector<pii> &items) {
    vec dp(W + 1, 0);
    for (int i = 0; i < (int)items.size(); i++) {
        int w = items[i].fi, v = items[i].se;
        for (int j = W; j >= w; j--) // 由大到小！
            dp[j] = max(dp[j], dp[j - w] + v);
    }
    return dp[W];
}

// 2. 無限背包 O(n * W)：每種物品可拿無限次
int knapsack_inf(int W, const vector<pii> &items) {
    vec dp(W + 1, 0);
    for (int i = 0; i < (int)items.size(); i++) {
        int w = items[i].fi, v = items[i].se;
        for (int j = w; j <= W; j++) // 由小到大！
            dp[j] = max(dp[j], dp[j - w] + v);
    }
    return dp[W];
}

// 3. 有限 (多重) 背包 O(W * sum(log c))：每種物品重量 w、價值 v、最多拿 c 個
struct Item3 { int w, v, c; };
int knapsack_bounded(int W, const vector<Item3> &items) {
    vector<pii> split_items;
    for (int i = 0; i < (int)items.size(); i++) {
        int w = items[i].w, v = items[i].v, c = items[i].c;
        for (int k = 1; k <= c; k <<= 1) {
            split_items.pb(make_pair(w * k, v * k));
            c -= k;
        }
        if (c > 0) split_items.pb(make_pair(w * c, v * c));
    }
    return knapsack_01(W, split_items);
}

// === 實戰呼叫範例 ===
void voids() {
    int n, W;
    cin >> n >> W;
    vector<pii> items(n);
    for (int i = 0; i < n; i++) cin >> items[i].fi >> items[i].se; // 讀入 重量、價值
    cout << knapsack_01(W, items) << "\n";
}
```

---

### 4.2 最長遞增子序列 `LIS`（直接搭配你的 `lb` / `ub` 巨集）｜$O(n \log n)$

- **何時用**：求陣列中最長嚴格遞增（`strict = true`）或最長不遞減（`strict = false`）子序列的長度。

```cpp
int lis_length(const vec &a, bool strict = true) {
    vec dp;
    for (int i = 0; i < (int)a.size(); i++) {
        int x = a[i];
        // 嚴格遞增 (<) 用你的 lb；允許相等 (<=) 用你的 ub！
        int pos = strict ? (lb(dp, x)) : (ub(dp, x));
        if (pos == (int)dp.size()) dp.pb(x);
        else dp[pos] = x;
    }
    return (int)dp.size();
}

// === 實戰呼叫範例 ===
void voids() {
    int n; cin >> n;
    vec a(n);
    for (int i = 0; i < n; i++) cin >> a[i];
    cout << lis_length(a, true) << "\n"; // 印出嚴格遞增子序列最大長度
}
```

---

### 4.3 `LCS` 最長共同子序列 ＆ 編輯距離 (Edit Distance)｜$O(nm)$

```cpp
// 1. LCS 最長共同子序列長度 (滾動陣列省記憶體版)
int lcs_length(const string &s, const string &t) {
    int n = (int)s.size(), m = (int)t.size();
    vec dp(m + 1, 0);
    for (int i = 1; i <= n; i++) {
        int prev = 0; // 存左上角 dp[i-1][j-1]
        for (int j = 1; j <= m; j++) {
            int tmp = dp[j];
            if (s[i - 1] == t[j - 1]) dp[j] = prev + 1;
            else dp[j] = max(dp[j], dp[j - 1]);
            prev = tmp;
        }
    }
    return dp[m];
}

// 2. 編輯距離：最少幾次「插入、刪除、替換字元」把字串 s 變成字串 t
int edit_distance(const string &s, const string &t) {
    int n = (int)s.size(), m = (int)t.size();
    grid(n + 1, m + 1, dp);
    for (int i = 0; i <= n; i++) dp[i][0] = i;
    for (int j = 0; j <= m; j++) dp[0][j] = j;
    for (int i = 1; i <= n; i++) {
        for (int j = 1; j <= m; j++) {
            if (s[i - 1] == t[j - 1]) dp[i][j] = dp[i - 1][j - 1];
            else dp[i][j] = 1 + min(dp[i - 1][j - 1], min(dp[i - 1][j], dp[i][j - 1]));
        }
    }
    return dp[n][m];
}
```

---

### 4.4 區間 DP 標準骨架（相鄰石子合併最小代價）｜$O(n^3)$

- **重點**：最外層迴圈**一定要枚舉區間長度 `len` 從 `2` 到 `n`**！

```cpp
void voids() {
    int n;
    cin >> n;
    vec a(n + 1, 0), pref(n + 1, 0);
    for (int i = 1; i <= n; i++) {
        cin >> a[i];
        pref[i] = pref[i - 1] + a[i]; // 前綴和用來 O(1) 算合併成本
    }
    grid(n + 1, n + 1, dp);
    for (int i = 1; i <= n; i++)
        for (int j = 1; j <= n; j++) dp[i][j] = (i == j ? 0 : inf);

    for (int len = 2; len <= n; len++) {          // 1. 枚舉長度
        for (int l = 1; l + len - 1 <= n; l++) {  // 2. 枚舉左界 l
            int r = l + len - 1;                  // 算出右界 r
            int cost = pref[r] - pref[l - 1];
            for (int k = l; k < r; k++) {         // 3. 枚舉切分點 k
                dp[l][r] = min(dp[l][r], dp[l][k] + dp[k + 1][r] + cost);
            }
        }
    }
    cout << dp[1][n] << "\n";
}
```

---

### 4.5 樹形 DP ＆ 樹直徑（樹上最遠兩點距離）｜`1-based`｜$O(n)$

```cpp
// 回傳從 u 往下走的最長單鏈長度，並順便用 mx1 + mx2 更新全域答案 ans
int tree_diam_dfs(int u, int p, const vector<vector<pii>> &adj, int &ans) {
    int mx1 = 0, mx2 = 0; // 最長與次長往下路徑
    for (int i = 0; i < (int)adj[u].size(); i++) {
        int v = adj[u][i].fi, w = adj[u][i].se;
        if (v == p) continue;
        int d = tree_diam_dfs(v, u, adj, ans) + w;
        if (d > mx1) { mx2 = mx1; mx1 = d; }
        else if (d > mx2) mx2 = d;
    }
    ans = max(ans, mx1 + mx2);
    return mx1;
}

void voids() {
    int n;
    cin >> n;
    vector<vector<pii>> adj(n + 1);
    for (int i = 0; i < n - 1; i++) {
        int u, v, w = 1;
        cin >> u >> v; // 若題目有給邊權就多讀 >> w
        adj[u].pb(make_pair(v, w));
        adj[v].pb(make_pair(u, w));
    }
    int ans = 0;
    if (n >= 1) tree_diam_dfs(1, 0, adj, ans);
    cout << ans << "\n";
}
```

---

### 4.6 狀態壓縮 DP（Bitmask TSP 最短路徑 ＆ 子集枚舉）｜$O(n^2 2^n)$

- **何時用**：$n \le 20$，用二進位整數 `mask` 的第 $i$ 個 bit (`(mask >> i) & 1`) 記錄點 $i$ 走過了沒。

```cpp
void voids() {
    int n;
    cin >> n;
    grid(n, n, dist);
    for (int i = 0; i < n; i++)
        for (int j = 0; j < n; j++) cin >> dist[i][j];

    // dp[mask][u]: 已走過集合為 mask，且目前站在點 u (0-based: 0 ~ n-1) 的最小花費
    vector<vec> dp(1LL << n, vec(n, inf));
    dp[1][0] = 0; // 從點 0 出發 (mask = 1 << 0 = 1)

    for (int mask = 1; mask < (1LL << n); mask++) {
        for (int u = 0; u < n; u++) {
            if (!((mask >> u) & 1) || dp[mask][u] == inf) continue;
            for (int v = 0; v < n; v++) {
                if (!((mask >> v) & 1)) { // 點 v 還沒走過
                    int nxt = mask | (1LL << v);
                    dp[nxt][v] = min(dp[nxt][v], dp[mask][u] + dist[u][v]);
                }
            }
        }
    }
    int full = (1LL << n) - 1, ans = inf;
    for (int u = 0; u < n; u++) ans = min(ans, dp[full][u]); // 若要走回 0 則加 + dist[u][0]
    cout << ans << "\n";

    // [附錄技巧] O(3^n) 枚舉所有 mask 的所有非空子集 sub：
    // for (int sub = mask; sub > 0; sub = (sub - 1) & mask) { ... }
}
```

---

### 4.7 數位 DP 萬用記憶化搜尋骨架｜$O(\log_{10} R \times \text{狀態數})$

- **何時用**：問 $[L, R]$（$R \le 10^{18}$）之間有幾個數字滿足某個位數規則（例如：各位數字總和是 $K$ 的倍數、不含相鄰相同數字）。用 `count_upto(R) - count_upto(L - 1)` 得到答案！

```cpp
struct DigitDP {
    string s;
    int memo[20][200]; // [第幾位][狀態值 (如數位和)]，依題目調整第二維大小

    int dfs(int pos, int state, bool tight, bool lead_zero) {
        if (pos == (int)s.size()) {
            return (state == 10) ? 1 : 0; // [依題目改] 填完所有位數後，檢查狀態是否合法
        }
        if (!tight && !lead_zero && memo[pos][state] != -1) {
            return memo[pos][state];
        }
        int up = tight ? (s[pos] - '0') : 9; // 受限時最多填到原數字該位，否則可填 0~9
        int res = 0;
        for (int d = 0; d <= up; d++) {
            bool nxt_zero = lead_zero && (d == 0);
            int nxt_state = state + d; // [依題目改] 更新狀態
            res += dfs(pos + 1, nxt_state, tight && (d == up), nxt_zero);
        }
        if (!tight && !lead_zero) memo[pos][state] = res;
        return res;
    }
    int solve(int X) {
        if (X < 0) return 0;
        s = to_string(X);
        memset(memo, -1, sizeof(memo));
        return dfs(0, 0, true, true);
    }
};

void voids() {
    int L, R;
    cin >> L >> R;
    DigitDP solver;
    cout << solver.solve(R) - solver.solve(L - 1) << "\n";
}
```

---

## 5. 圖論：最短路徑 (Shortest Paths)

### 5.1 網格迷宮 `BFS`（搭配你的 `gridc`、`grid`、`dr`、`dc`）＆ `0-1 BFS`｜$O(V + E)$

- **何時用**：
  - **網格 BFS**：迷宮找起點 `'S'` 到終點 `'E'` 最少步數（每步距離 `1`）。
  - **`bfs01`**：邊權只有 `0` 或 `1` 的最短路（權重 `0` 塞 `deque` 前面，權重 `1` 塞後面）。

```cpp
// 1. 網格迷宮 BFS 實戰寫法 (直接使用你模板的 gridc, grid, dr[], dc[], inf！)
void voids() {
    int n, m;
    cin >> n >> m;
    gridc(n, m, mp);        // 你的巨集：建立 n x m 字元地圖
    grid(n, m, dist);       // 你的巨集：建立 n x m 距離陣列
    int sr = 0, sc = 0, er = 0, ec = 0;

    for (int r = 0; r < n; r++) {
        for (int c = 0; c < m; c++) {
            cin >> mp[r][c];
            dist[r][c] = inf;
            if (mp[r][c] == 'S') { sr = r; sc = c; }
            if (mp[r][c] == 'E') { er = r; ec = c; }
        }
    }
    queue<pii> q;
    dist[sr][sc] = 0;
    q.push(make_pair(sr, sc));

    while (!q.empty()) {
        pii cur = q.front(); q.pop();
        int r = cur.fi, c = cur.se;
        for (int d = 0; d < 4; d++) { // 若可走斜角 8 方向，把 4 改 8，dr/dc 改 dr8/dc8！
            int nr = r + dr[d], nc = c + dc[d];
            if (nr < 0 || nr >= n || nc < 0 || nc >= m) continue; // 超出邊界
            if (mp[nr][nc] == '#' || dist[nr][nc] != inf) continue; // 撞牆或已走過
            dist[nr][nc] = dist[r][c] + 1;
            q.push(make_pair(nr, nc));
        }
    }
    if (dist[er][ec] == inf) cout << -1 << "\n";
    else cout << dist[er][ec] << "\n";
}

// 2. 0-1 BFS (邊權只有 0 或 1 的一般圖最短路，1-based)
vec bfs01(int n, int s, const vector<vector<pii>> &adj) {
    vec dist(n + 1, inf);
    deque<int> dq;
    dist[s] = 0; dq.push_front(s);
    while (!dq.empty()) {
        int u = dq.front(); dq.pop_front();
        for (int i = 0; i < (int)adj[u].size(); i++) {
            int v = adj[u][i].fi, w = adj[u][i].se;
            if (dist[u] + w < dist[v]) {
                dist[v] = dist[u] + w;
                if (w == 0) dq.push_front(v); // 0 元免費邊排到最前面優先走
                else dq.pb(v);                // 1 元邊排在後面
            }
        }
    }
    return dist;
}
```

---

### 5.2 `Dijkstra`（非負權單源最短路 ＋ 路徑還原）｜`1-based`｜$O((V + E) \log V)$

- **何時用**：所有邊權都 $\ge 0$，求起點 `s` 到各點最短距離。
- **避坑提醒**：
  1. `if (d > dist[u]) continue;` **絕對不可漏寫**，否則會退化超時 TLE！
  2. 若題目最多 $2 \times 10^5$ 條邊、每條邊權 $10^9$，總距離最大 $2 \times 10^{14} < \text{inf}$ (`1e17+5`) 很安全；若邊權高達 $10^{13}$，請把模板開頭的 `inf` 改大成 `4e18`！

```cpp
// adj[u] 存 pii(鄰點 v, 邊權 w)；回傳 {dist 最短距離陣列, parent 前驅點陣列}
pair<vec, vec> dijkstra(int n, int s, const vector<vector<pii>> &adj) {
    vec dist(n + 1, inf), parent(n + 1, -1);
    priority_queue<pii, vector<pii>, greater<pii>> pq; // 存 {目前距離, 點編號} 的小根堆
    dist[s] = 0;
    pq.push(make_pair(0, s));

    while (!pq.empty()) {
        pii top = pq.top(); pq.pop();
        int d = top.fi, u = top.se;
        if (d > dist[u]) continue; // 過期的舊距離直接跳過！
        for (int i = 0; i < (int)adj[u].size(); i++) {
            int v = adj[u][i].fi, w = adj[u][i].se;
            if (dist[u] + w < dist[v]) {
                dist[v] = dist[u] + w;
                parent[v] = u;
                pq.push(make_pair(dist[v], v));
            }
        }
    }
    return make_pair(dist, parent);
}

// 還原從起點 s 走到終點 t 的完整經過點序列 (呼叫前務必確認 dist[t] != inf)
vec restore_path(int t, const vec &parent) {
    vec path;
    for (int cur = t; cur != -1; cur = parent[cur]) path.pb(cur);
    reverse(be(path));
    return path;
}

// === 實戰呼叫範例：求點 1 到點 n 的最短距離與經過路徑 ===
void voids() {
    int n, m;
    cin >> n >> m;
    vector<vector<pii>> adj(n + 1);
    for (int i = 0; i < m; i++) {
        int u, v, w;
        cin >> u >> v >> w;
        adj[u].pb(make_pair(v, w)); // 注意順序是 (鄰點 v, 邊權 w)！
        adj[v].pb(make_pair(u, w)); // 若是有向圖，刪掉這行反向邊
    }
    pair<vec, vec> res = dijkstra(n, 1, adj);
    vec dist = res.fi, par = res.se;

    if (dist[n] == inf) {
        cout << -1 << "\n"; // 走不到終點
    } else {
        cout << dist[n] << "\n";
        vec path = restore_path(n, par);
        for (int i = 0; i < (int)path.size(); i++) cout << path[i] << " ";
        cout << "\n";
    }
}
```

---

### 5.3 `SPFA`（含負權邊最短路 ＋ 判負環）｜`1-based`｜最壞 $O(VE)$

- **何時用**：圖中有**負權邊**，或題目問**有沒有負環**。
- **判「全圖任意位置」負環技巧**：若負環不一定從起點 `1` 走得到，可多開一個超級源點 `0`，從 `0` 連權重 `0` 的邊到 `1..n` 所有點，呼叫 `spfa(n + 1, 0, adj)`（注意點數傳 `n + 1` 或把 `cnt[v] >= n + 1` 作為門檻）。

```cpp
// 回傳 {是否有從 s 可達的負環, dist 陣列}
pair<bool, vec> spfa(int n, int s, const vector<vector<pii>> &adj) {
    vec dist(n + 1, inf), cnt(n + 1, 0);
    vector<bool> in_q(n + 1, false);
    queue<int> q;
    dist[s] = 0; q.push(s); in_q[s] = true;

    while (!q.empty()) {
        int u = q.front(); q.pop(); in_q[u] = false;
        for (int i = 0; i < (int)adj[u].size(); i++) {
            int v = adj[u][i].fi, w = adj[u][i].se;
            if (dist[u] + w < dist[v]) {
                dist[v] = dist[u] + w;
                cnt[v] = cnt[u] + 1;
                if (cnt[v] >= n) return make_pair(true, dist); // 最短路超過 n-1 條邊必有負環！
                if (!in_q[v]) { q.push(v); in_q[v] = true; }
            }
        }
    }
    return make_pair(false, dist);
}

// === 實戰呼叫範例 ===
void voids() {
    int n, m;
    cin >> n >> m;
    vector<vector<pii>> adj(n + 1);
    for (int i = 0; i < m; i++) {
        int u, v, w; cin >> u >> v >> w;
        adj[u].pb(make_pair(v, w));
    }
    pair<bool, vec> res = spfa(n, 1, adj);
    if (res.fi) cout << "NEGATIVE CYCLE\n";
    else        cout << (res.se[n] == inf ? -1 : res.se[n]) << "\n";
}
```

---

### 5.4 `Floyd-Warshall`（全點對最短路）｜`1-based`｜$O(V^3)$

- **何時用**：點數 $n \le 400 \sim 500$，要回答很多筆「任意點 `u` 到點 `v` 最短距離」。

```cpp
void voids() {
    int n, m, q;
    cin >> n >> m >> q;
    grid(n + 1, n + 1, dist);
    for (int i = 1; i <= n; i++)
        for (int j = 1; j <= n; j++)
            dist[i][j] = (i == j ? 0 : inf);

    for (int i = 0; i < m; i++) {
        int u, v, w; cin >> u >> v >> w;
        dist[u][v] = min(dist[u][v], w); // 用 min 防止題目給重邊！
        dist[v][u] = min(dist[v][u], w); // 有向圖刪掉這行
    }
    // 核心三層迴圈：中繼點 k 絕對要在最外層！
    for (int k = 1; k <= n; k++)
        for (int i = 1; i <= n; i++)
            for (int j = 1; j <= n; j++)
                if (dist[i][k] < inf && dist[k][j] < inf)
                    dist[i][j] = min(dist[i][j], dist[i][k] + dist[k][j]);

    while (q--) {
        int u, v; cin >> u >> v;
        cout << (dist[u][v] == inf ? -1 : dist[u][v]) << "\n";
    }
}
```

---

## 6. 圖論：最小生成樹、拓樸排序、樹上問題 (MST, DAG, Trees)

### 6.1 `Kruskal` ＆ `Prim` 最小生成樹 (MST)｜`1-based`

- **優先用 `Kruskal`**（需先貼 3.1 的 `DSU`），簡單直覺；只有當圖是完全圖（$E \approx V^2$）時才用 `Prim`。

```cpp
struct Edge {
    int u, v, w;
    bool operator<(const Edge &o) const { return w < o.w; } // 按邊權由小到大排
};

// Kruskal O(E log E)：回傳 {是否連通成一棵樹, 最小生成樹總權重}
pair<bool, int> kruskal(int n, vector<Edge> edges) {
    sort(be(edges));
    DSU dsu(n);
    int total = 0, cnt = 0;
    for (int i = 0; i < (int)edges.size(); i++) {
        if (dsu.unite(edges[i].u, edges[i].v)) { // 不構成環就選這條邊
            total += edges[i].w;
            cnt++;
        }
    }
    return make_pair(cnt == n - 1, total);
}

// Prim O(E log V)：從點 1 開始往外擴張，回傳 {是否連通, 最小生成樹總權重}
pair<bool, int> prim(int n, const vector<vector<pii>> &adj) {
    vector<bool> vis(n + 1, false);
    priority_queue<pii, vector<pii>, greater<pii>> pq;
    pq.push(make_pair(0, 1));
    int total = 0, cnt = 0;
    while (!pq.empty()) {
        pii top = pq.top(); pq.pop();
        int w = top.fi, u = top.se;
        if (vis[u]) continue;
        vis[u] = true;
        total += w; cnt++;
        for (int i = 0; i < (int)adj[u].size(); i++) {
            int v = adj[u][i].fi, nw = adj[u][i].se;
            if (!vis[v]) pq.push(make_pair(nw, v));
        }
    }
    return make_pair(cnt == n, total);
}

// === 實戰呼叫範例 ===
void voids() {
    int n, m;
    cin >> n >> m;
    vector<Edge> edges(m);
    for (int i = 0; i < m; i++) cin >> edges[i].u >> edges[i].v >> edges[i].w;

    pair<bool, int> res = kruskal(n, edges);
    if (!res.fi) cout << "IMPOSSIBLE\n"; // 圖不連通
    else         cout << res.se << "\n"; // 印出 MST 最小總成本
}
```

---

### 6.2 拓樸排序 `topo_sort`（DAG 排順序／判有向環／DAG DP）｜`1-based`｜$O(V + E)$

- **字典序最小變形**：只要把下面的 `queue<int> q;` 換成你的小根堆巨集 `rp_q q;`，並把 `q.front()` 改成 `q.top()`，印出來就自動是字典序最小的合法順序！

```cpp
// 傳入 1-based 有向圖 adj；若圖中有環回傳空陣列 vec()，無環回傳長度 n 的合法順序
vec topo_sort(int n, const vector<vec> &adj) {
    vec indeg(n + 1, 0), order;
    for (int u = 1; u <= n; u++)
        for (int i = 0; i < (int)adj[u].size(); i++)
            indeg[adj[u][i]]++; // 統計每個點的入度 (有幾門先修課)

    queue<int> q; // 若要求字典序最小，改成 rp_q q; (並把下方 q.front() 改 q.top())
    for (int i = 1; i <= n; i++) if (indeg[i] == 0) q.push(i);

    while (!q.empty()) {
        int u = q.front(); q.pop();
        order.pb(u);
        for (int i = 0; i < (int)adj[u].size(); i++) {
            int v = adj[u][i];
            if (--indeg[v] == 0) q.push(v); // 先修課都修完了，可以排入佇列
        }
    }
    if ((int)order.size() < n) return vec(); // 點沒拿完代表有環！
    return order;
}

// === 實戰呼叫範例：判環 + 在 DAG 上做 DP 求從各點出發或到達的方法數 ===
void voids() {
    int n, m;
    cin >> n >> m;
    vector<vec> adj(n + 1);
    for (int i = 0; i < m; i++) {
        int u, v; cin >> u >> v;
        adj[u].pb(v); // u 必須排在 v 前面
    }
    vec ord = topo_sort(n, adj);
    if (ord.empty()) {
        cout << "IMPOSSIBLE\n"; // 有環無解
        return;
    }
    // 印出拓樸順序 (若要做 DAG DP：依序 for (int i=0; i<n; i++) 由 u = ord[i] 推給鄰點 v！)
    for (int i = 0; i < n; i++) cout << ord[i] << " ";
    cout << "\n";
}
```

---

### 6.3 最近共同祖先 `LCA`（倍增法：查祖先、查樹上兩點距離）｜`1-based`｜建 $O(n\log n)$，查 $O(\log n)$

```cpp
int lg2(int x) { return x <= 1 ? 0 : 63 - __builtin_clzll(x); }

struct LCA {
    int n, lg;
    vec dep;            // dep[u]: 點 u 的深度 (樹根深度為 0)
    vector<vec> up;     // up[k][u]: 點 u 往上跳 2^k 步到達的祖先
    vector<vec> adj;

    LCA(int n) : n(n), lg(lg2(n) + 2), dep(n + 1, 0), up(lg, vec(n + 1, 0)), adj(n + 1) {}
    void add_edge(int u, int v) { adj[u].pb(v); adj[v].pb(u); }
    void build(int root = 1) { dfs(root, 0); } // 讀完邊後務必呼叫 build(樹根)！

    void dfs(int u, int p) {
        up[0][u] = p;
        for (int k = 1; k < lg; k++) up[k][u] = up[k - 1][up[k - 1][u]];
        for (int i = 0; i < (int)adj[u].size(); i++) {
            int v = adj[u][i];
            if (v != p) { dep[v] = dep[u] + 1; dfs(v, u); }
        }
    }
    int kth_anc(int u, int k) { // 點 u 往上跳 k 步的祖先 (超過樹根回傳 0)
        for (int i = 0; i < lg && u; i++)
            if ((k >> i) & 1) u = up[i][u];
        return u;
    }
    int lca(int u, int v) { // 點 u 與點 v 的最近共同祖先
        if (dep[u] < dep[v]) swap(u, v);
        u = kth_anc(u, dep[u] - dep[v]);
        if (u == v) return u;
        for (int k = lg - 1; k >= 0; k--)
            if (up[k][u] != up[k][v]) { u = up[k][u]; v = up[k][v]; }
        return up[0][u];
    }
    int dist(int u, int v) { // 樹上 u 到 v 的邊數距離
        return dep[u] + dep[v] - 2 * dep[lca(u, v)];
    }
};

// === 實戰呼叫範例 ===
void voids() {
    int n, q;
    cin >> n >> q;
    LCA tr(n);
    for (int i = 0; i < n - 1; i++) {
        int u, v; cin >> u >> v;
        tr.add_edge(u, v);
    }
    tr.build(1); // 記得呼叫 build！
    while (q--) {
        int u, v; cin >> u >> v;
        cout << tr.lca(u, v) << " " << tr.dist(u, v) << "\n";
    }
}
```

---

### 6.4 樹壓平 `Euler Tour`（把整棵子樹轉成連續區間配 `BIT`／線段樹）｜`1-based`｜$O(n)$

- **何時用**：題目要「修改某點權重（或整棵子樹加值）」並「查詢某點 `u` 的**整棵子樹**權重總和」。

```cpp
struct EulerTour {
    int n, timer;
    vec tin, tout; // 點 u 的整棵子樹對應連續閉區間 [tin[u], tout[u]]！
    vector<vec> adj;
    EulerTour(int n) : n(n), timer(0), tin(n + 1, 0), tout(n + 1, 0), adj(n + 1) {}
    void add_edge(int u, int v) { adj[u].pb(v); adj[v].pb(u); }
    void dfs(int u, int p) {
        tin[u] = ++timer;
        for (int i = 0; i < (int)adj[u].size(); i++)
            if (adj[u][i] != p) dfs(adj[u][i], u);
        tout[u] = timer;
    }
    void build(int root = 1) { dfs(root, 0); }
};

// === 實戰呼叫範例：CSES Subtree Queries (改點權 + 查子樹總和，需先貼 3.2 BIT) ===
void voids() {
    int n, q;
    cin >> n >> q;
    vec val(n + 1);
    for (int i = 1; i <= n; i++) cin >> val[i];

    EulerTour et(n);
    for (int i = 0; i < n - 1; i++) { int u, v; cin >> u >> v; et.add_edge(u, v); }
    et.build(1);

    BIT bit(n);
    for (int u = 1; u <= n; u++) bit.add(et.tin[u], val[u]); // 放在 tin[u] 的位置！

    while (q--) {
        int op; cin >> op;
        if (op == 1) {
            int u, x; cin >> u >> x;
            bit.add(et.tin[u], x - val[u]); // 把點 u 的值改成 x
            val[u] = x;
        } else {
            int u; cin >> u;
            cout << bit.query(et.tin[u], et.tout[u]) << "\n"; // 查 u 的整棵子樹總和！
        }
    }
}
```

---

### 6.5 重鏈剖分 `HLD`（樹上任意兩點路徑修改／查詢）｜`1-based`｜$O(\log^2 n)$

- **何時用**：樹上要「修改 `u` 到 `v` 最短路徑上的點」或「查詢 `u` 到 `v` 路徑上的最大值／總和」（需搭配 3.5 `SegTree` 或 3.6 `LazySegTree`）。

```cpp
struct HLD {
    int n, timer;
    vec sz_v, dep, pa, heavy, head, dfn;
    vector<vec> adj;
    HLD(int n) : n(n), timer(0), sz_v(n + 1, 0), dep(n + 1, 0), pa(n + 1, 0),
                 heavy(n + 1, 0), head(n + 1, 0), dfn(n + 1, 0), adj(n + 1) {}
    void add_edge(int u, int v) { adj[u].pb(v); adj[v].pb(u); }
    void build(int root = 1) { dfs1(root, 0); dfs2(root, root); }

    void dfs1(int u, int p) {
        pa[u] = p; sz_v[u] = 1;
        for (int i = 0; i < (int)adj[u].size(); i++) {
            int v = adj[u][i];
            if (v == p) continue;
            dep[v] = dep[u] + 1;
            dfs1(v, u);
            sz_v[u] += sz_v[v];
            if (sz_v[v] > sz_v[heavy[u]]) heavy[u] = v;
        }
    }
    void dfs2(int u, int h) {
        head[u] = h; dfn[u] = ++timer;
        if (heavy[u]) dfs2(heavy[u], h);
        for (int i = 0; i < (int)adj[u].size(); i++) {
            int v = adj[u][i];
            if (v != pa[u] && v != heavy[u]) dfs2(v, v);
        }
    }
    // 將樹上 u 到 v 的路徑拆成 O(log n) 個線段樹閉區間 {l, r} 回傳！完全不需寫複雜語法！
    vector<pii> get_path_segs(int u, int v) {
        vector<pii> segs;
        while (head[u] != head[v]) {
            if (dep[head[u]] < dep[head[v]]) swap(u, v);
            segs.pb(make_pair(dfn[head[u]], dfn[u]));
            u = pa[head[u]];
        }
        if (dep[u] > dep[v]) swap(u, v);
        segs.pb(make_pair(dfn[u], dfn[v]));
        return segs;
    }
};

// === 實戰呼叫範例：單點修改點權 + 查樹上 u 到 v 路徑最大值 (搭配 3.5 SegTree) ===
void voids() {
    int n, q;
    cin >> n >> q;
    vec val(n + 1);
    for (int i = 1; i <= n; i++) cin >> val[i];

    HLD hld(n);
    for (int i = 0; i < n - 1; i++) { int u, v; cin >> u >> v; hld.add_edge(u, v); }
    hld.build(1);

    vec init_a(n + 1);
    for (int u = 1; u <= n; u++) init_a[hld.dfn[u]] = val[u]; // 按 dfn 編號放進線段樹
    SegTree seg(n, init_a);

    while (q--) {
        int op, x, y; cin >> op >> x >> y;
        if (op == 1) {
            seg.update(hld.dfn[x], y); // 把點 x 的權重改成 y
        } else {
            vector<pii> segs = hld.get_path_segs(x, y);
            int ans = -inf;
            for (int i = 0; i < (int)segs.size(); i++)
                ans = max(ans, seg.query(segs[i].fi, segs[i].se).mx);
            cout << ans << "\n";
        }
    }
}
```

---

## 7. 圖論：強連通分量、割點與橋、歐拉路徑 (SCC, Lowlink, Euler)

### 7.1 `TarjanSCC`（有向圖強連通分量 ＋ 縮點成 DAG）｜`1-based`｜$O(V + E)$

- **何時用**：有向圖有環，想把能互相走到的一群點縮成一顆大點變成 DAG（例如 CSES Coin Collector：每個點有硬幣，走過都能撿，問最多撿多少）。
- **重要性質**：跑完 `build()` 後，共有 `scc_cnt` 個強連通塊（編號 `1 ~ scc_cnt`），且**編號從 `scc_cnt` 倒數到 `1` 天然就是縮點後 DAG 的拓樸順序**！

```cpp
struct TarjanSCC {
    int n, timer, scc_cnt;
    vector<vec> adj;
    vec dfn, low, scc_id, stk; // scc_id[u]: 點 u 屬於第幾個強連通分量 (1 ~ scc_cnt)
    vector<bool> in_stk;

    TarjanSCC(int n) : n(n), timer(0), scc_cnt(0), adj(n + 1),
                       dfn(n + 1, 0), low(n + 1, 0), scc_id(n + 1, 0), in_stk(n + 1, false) {}
    void add_edge(int u, int v) { adj[u].pb(v); }

    void dfs(int u) {
        dfn[u] = low[u] = ++timer;
        stk.pb(u); in_stk[u] = true;
        for (int i = 0; i < (int)adj[u].size(); i++) {
            int v = adj[u][i];
            if (!dfn[v]) { dfs(v); low[u] = min(low[u], low[v]); }
            else if (in_stk[v]) low[u] = min(low[u], dfn[v]);
        }
        if (low[u] == dfn[u]) {
            scc_cnt++;
            while (true) {
                int x = stk.back(); stk.pop_back();
                in_stk[x] = false;
                scc_id[x] = scc_cnt;
                if (x == u) break;
            }
        }
    }
    void build() {
        for (int i = 1; i <= n; i++) if (!dfn[i]) dfs(i);
    }
    // 建立縮點後的無重邊 DAG 鄰接表 dag[1..scc_cnt]
    vector<vec> build_dag() {
        vector<vec> dag(scc_cnt + 1);
        for (int u = 1; u <= n; u++)
            for (int i = 0; i < (int)adj[u].size(); i++) {
                int v = adj[u][i];
                if (scc_id[u] != scc_id[v]) dag[scc_id[u]].pb(scc_id[v]);
            }
        for (int i = 1; i <= scc_cnt; i++) {
            mkunique(dag[i]); // 使用你的巨集排序去重邊！
        }
        return dag;
    }
};

// === 實戰呼叫範例：縮點後在 DAG 上 DP 求最大點權總和路徑 ===
void voids() {
    int n, m;
    cin >> n >> m;
    vec coin(n + 1);
    for (int i = 1; i <= n; i++) cin >> coin[i];

    TarjanSCC scc(n);
    for (int i = 0; i < m; i++) { int u, v; cin >> u >> v; scc.add_edge(u, v); }
    scc.build();

    vec group_coin(scc.scc_cnt + 1, 0), dp(scc.scc_cnt + 1, 0);
    for (int u = 1; u <= n; u++) group_coin[scc.scc_id[u]] += coin[u];

    vector<vec> dag = scc.build_dag();
    int ans = 0;
    // Tarjan 編號從大到小 (scc_cnt -> 1) 就是拓樸排序順序！
    for (int u = scc.scc_cnt; u >= 1; u--) {
        dp[u] = max(dp[u], group_coin[u]);
        for (int i = 0; i < (int)dag[u].size(); i++) {
            int v = dag[u][i];
            dp[v] = max(dp[v], dp[u] + group_coin[v]);
        }
        ans = max(ans, dp[u]);
    }
    cout << ans << "\n";
}
```

---

### 7.2 `Kosaraju`（兩次 DFS 求 SCC 備用版）｜`1-based`｜$O(V + E)$

- **特色**：`scc_id` **由小到大 (`1 -> scc_cnt`) 正向就是拓樸順序**。

```cpp
struct Kosaraju {
    int n, scc_cnt;
    vector<vec> adj, radj;
    vec order, scc_id;
    vector<bool> vis;
    Kosaraju(int n) : n(n), scc_cnt(0), adj(n + 1), radj(n + 1),
                      scc_id(n + 1, 0), vis(n + 1, false) {}
    void add_edge(int u, int v) { adj[u].pb(v); radj[v].pb(u); }
    void dfs1(int u) {
        vis[u] = true;
        for (int i = 0; i < (int)adj[u].size(); i++)
            if (!vis[adj[u][i]]) dfs1(adj[u][i]);
        order.pb(u);
    }
    void dfs2(int u, int cid) {
        scc_id[u] = cid;
        for (int i = 0; i < (int)radj[u].size(); i++)
            if (!scc_id[radj[u][i]]) dfs2(radj[u][i], cid);
    }
    void build() {
        for (int i = 1; i <= n; i++) if (!vis[i]) dfs1(i);
        reverse(be(order));
        for (int i = 0; i < (int)order.size(); i++)
            if (!scc_id[order[i]]) dfs2(order[i], ++scc_cnt);
    }
};
```

---

### 7.3 無向圖 `Lowlink`：橋、割點、邊雙連通分量 (EBCC)｜`1-based`｜$O(V + E)$

- **何時用**：找無向圖中「斷掉就不連通的**橋** (`is_bridge`)」、「刪掉就不連通的**割點** (`is_cut`)」、或把橋拔掉後的連通塊 `ebcc_id`（支援重邊！）。

```cpp
struct Lowlink {
    int n, m, timer, ebcc_cnt;
    vector<vector<pii>> adj;    // 存 {鄰點 v, 邊編號 id}
    vector<pii> edges;          // edges[id] = 第 id 條邊的兩個端點 {u, v}
    vec dfn, low, ebcc_id;      // ebcc_id[u] = 點 u 所屬的邊雙連通塊編號 (1 ~ ebcc_cnt)
    vector<bool> is_bridge;     // is_bridge[id] = 第 id 條邊是否為橋 (0 ~ m-1)
    vector<bool> is_cut;        // is_cut[u] = 點 u 是否為割點 (1 ~ n)

    Lowlink(int n) : n(n), m(0), timer(0), ebcc_cnt(0), adj(n + 1),
                     dfn(n + 1, 0), low(n + 1, 0), ebcc_id(n + 1, 0), is_cut(n + 1, false) {}
    void add_edge(int u, int v) {
        adj[u].pb(make_pair(v, m));
        adj[v].pb(make_pair(u, m));
        edges.pb(make_pair(u, v));
        m++;
    }
    void dfs(int u, int in_edge) {
        dfn[u] = low[u] = ++timer;
        int child = 0;
        for (int i = 0; i < (int)adj[u].size(); i++) {
            int v = adj[u][i].fi, id = adj[u][i].se;
            if (id == in_edge) continue;
            if (!dfn[v]) {
                child++;
                dfs(v, id);
                low[u] = min(low[u], low[v]);
                if (low[v] > dfn[u]) is_bridge[id] = true;
                if (in_edge != -1 && low[v] >= dfn[u]) is_cut[u] = true;
            } else {
                low[u] = min(low[u], dfn[v]);
            }
        }
        if (in_edge == -1 && child >= 2) is_cut[u] = true;
    }
    void dfs_ebcc(int u, int cid) {
        ebcc_id[u] = cid;
        for (int i = 0; i < (int)adj[u].size(); i++) {
            int v = adj[u][i].fi, id = adj[u][i].se;
            if (!ebcc_id[v] && !is_bridge[id]) dfs_ebcc(v, cid);
        }
    }
    void build() {
        is_bridge.assign(m, false);
        for (int i = 1; i <= n; i++) if (!dfn[i]) dfs(i, -1);
        for (int i = 1; i <= n; i++) if (!ebcc_id[i]) dfs_ebcc(i, ++ebcc_cnt);
    }
};

// === 實戰呼叫範例：印出所有的橋與所有的割點 ===
void voids() {
    int n, m;
    cin >> n >> m;
    Lowlink g(n);
    for (int i = 0; i < m; i++) { int u, v; cin >> u >> v; g.add_edge(u, v); }
    g.build();

    // 印出所有橋的兩端點
    for (int id = 0; id < m; id++)
        if (g.is_bridge[id]) cout << g.edges[id].fi << " " << g.edges[id].se << "\n";

    // 印出所有割點
    for (int u = 1; u <= n; u++)
        if (g.is_cut[u]) cout << u << " ";
    cout << "\n";
}
```

---

### 7.4 點雙連通分量 `VBCC`｜`1-based`｜$O(V + E)$

```cpp
struct VBCC {
    int n, timer;
    vector<vec> adj, comps; // comps[i] 存第 i 個點雙連通分量的所有點 (割點會出現在多個塊中)
    vec dfn, low, stk;
    VBCC(int n) : n(n), timer(0), adj(n + 1), dfn(n + 1, 0), low(n + 1, 0) {}
    void add_edge(int u, int v) { if (u != v) { adj[u].pb(v); adj[v].pb(u); } }
    void dfs(int u, int p) {
        dfn[u] = low[u] = ++timer;
        stk.pb(u);
        if (p == 0 && adj[u].empty()) { vec single(1, u); comps.pb(single); return; }
        for (int i = 0; i < (int)adj[u].size(); i++) {
            int v = adj[u][i];
            if (v == p) continue;
            if (!dfn[v]) {
                dfs(v, u);
                low[u] = min(low[u], low[v]);
                if (low[v] >= dfn[u]) {
                    vec comp; comp.pb(u);
                    while (true) {
                        int x = stk.back(); stk.pop_back();
                        comp.pb(x);
                        if (x == v) break;
                    }
                    comps.pb(comp);
                }
            } else low[u] = min(low[u], dfn[v]);
        }
    }
    void build() {
        for (int i = 1; i <= n; i++) if (!dfn[i]) { stk.clear(); dfs(i, 0); }
    }
};
```

---

### 7.5 歐拉路徑／歐拉迴路 `Euler`（無向圖＆有向圖一筆畫）｜`1-based`｜$O(V + E)$

- **何時用**：每條邊**恰好走過一次**。`get_path()` 自動檢查度數與連通性，無解回傳空 `vec()`！
  - 若題目指定必須從點 `1` 出發，傳入 `get_path(1)`；若還要求**最後走回起點 `1`（歐拉迴路）**，再多檢查 `path.front() == 1 && path.back() == 1`！

```cpp
// 1. 無向圖歐拉路徑 / 迴路
struct EulerUndirected {
    int n, m;
    vector<vector<pii>> adj;
    vector<bool> used;
    vec deg, idx, path;
    EulerUndirected(int n) : n(n), m(0), adj(n + 1), deg(n + 1, 0) {}
    void add_edge(int u, int v) {
        adj[u].pb(make_pair(v, m));
        adj[v].pb(make_pair(u, m));
        deg[u]++; deg[v]++; m++;
    }
    void dfs(int u) {
        while (idx[u] < (int)adj[u].size()) {
            pii e = adj[u][idx[u]++];
            if (used[e.se]) continue;
            used[e.se] = true;
            dfs(e.fi);
        }
        path.pb(u);
    }
    vec get_path(int start = -1) {
        int odd = 0, first_odd = -1, any_v = 1;
        for (int i = 1; i <= n; i++) {
            if (deg[i] > 0) any_v = i;
            if (deg[i] % 2 == 1) { odd++; if (first_odd == -1) first_odd = i; }
        }
        if (odd != 0 && odd != 2) return vec();
        if (start == -1) start = (odd == 2 ? first_odd : any_v);
        else if (odd == 2 && deg[start] % 2 == 0) return vec();
        used.assign(m, false);
        idx.assign(n + 1, 0);
        path.clear();
        dfs(start);
        if ((int)path.size() != m + 1) return vec(); // 有邊走不到 -> 無解
        reverse(be(path));
        return path;
    }
};

// 2. 有向圖歐拉路徑 / 迴路
struct EulerDirected {
    int n, m;
    vector<vec> adj;
    vec indeg, outdeg, idx, path;
    EulerDirected(int n) : n(n), m(0), adj(n + 1), indeg(n + 1, 0), outdeg(n + 1, 0) {}
    void add_edge(int u, int v) { adj[u].pb(v); outdeg[u]++; indeg[v]++; m++; }
    void dfs(int u) {
        while (idx[u] < (int)adj[u].size()) {
            int v = adj[u][idx[u]++];
            dfs(v);
        }
        path.pb(u);
    }
    vec get_path(int start = -1) {
        int s_node = -1, t_node = -1, any_v = 1;
        for (int i = 1; i <= n; i++) {
            if (outdeg[i] > 0) any_v = i;
            if (outdeg[i] - indeg[i] == 1) { if (s_node != -1) return vec(); s_node = i; }
            else if (indeg[i] - outdeg[i] == 1) { if (t_node != -1) return vec(); t_node = i; }
            else if (indeg[i] != outdeg[i]) return vec();
        }
        if ((s_node == -1) != (t_node == -1)) return vec();
        if (start == -1) start = (s_node != -1 ? s_node : any_v);
        else if (s_node != -1 && start != s_node) return vec();
        idx.assign(n + 1, 0);
        path.clear();
        dfs(start);
        if ((int)path.size() != m + 1) return vec();
        reverse(be(path));
        return path;
    }
};

// === 實戰呼叫範例：CSES Mail Delivery (從點 1 出發走完所有無向邊並回到點 1) ===
void voids() {
    int n, m;
    cin >> n >> m;
    EulerUndirected eu(n);
    for (int i = 0; i < m; i++) { int u, v; cin >> u >> v; eu.add_edge(u, v); }
    vec path = eu.get_path(1);
    if (path.empty() || path.back() != 1) cout << "IMPOSSIBLE\n";
    else {
        for (int i = 0; i < (int)path.size(); i++) cout << path[i] << " ";
        cout << "\n";
    }
}
```

---

## 8. 圖論：二分圖、最大匹配、網路流、2-SAT

### 8.1 二分圖判定（黑白塗色判奇環）｜`1-based`｜$O(V + E)$

```cpp
// 回傳 {是否為二分圖, col 陣列 (每個點塗成 1 或 2)}
pair<bool, vec> check_bipartite(int n, const vector<vec> &adj) {
    vec col(n + 1, 0);
    for (int i = 1; i <= n; i++) if (!col[i]) {
        queue<int> q;
        col[i] = 1; q.push(i);
        while (!q.empty()) {
            int u = q.front(); q.pop();
            for (int j = 0; j < (int)adj[u].size(); j++) {
                int v = adj[u][j];
                if (!col[v]) { col[v] = 3 - col[u]; q.push(v); }
                else if (col[v] == col[u]) return make_pair(false, col); // 撞色代表有奇數環！
            }
        }
    }
    return make_pair(true, col);
}

// === 實戰呼叫範例：CSES Building Teams (把人分成兩隊使朋友不同隊) ===
void voids() {
    int n, m; cin >> n >> m;
    vector<vec> adj(n + 1);
    for (int i = 0; i < m; i++) {
        int u, v; cin >> u >> v;
        adj[u].pb(v); adj[v].pb(u);
    }
    pair<bool, vec> res = check_bipartite(n, adj);
    if (!res.fi) cout << "IMPOSSIBLE\n";
    else {
        for (int i = 1; i <= n; i++) cout << res.se[i] << " ";
        cout << "\n";
    }
}
```

---

### 8.2 二分圖最大匹配：`Kuhn` ($O(VE)$) ＆ `HopcroftKarp` ($O(E\sqrt{V})$)

- **必背轉換定理**：
  - 二分圖**最小點覆蓋**（選最少點蓋住所有邊）$=$ **最大匹配數**
  - 二分圖**最大獨立集**（選最多互不相鄰的點）$=$ **總點數 $-$ 最大匹配數**
- **編號方式**：左邊點編號 `1..nL`、右邊點編號 `1..nR`（兩邊各自從 `1` 開始編號即可！）。

```cpp
// 1. Kuhn 演算法 O(V * E)：適合 nL, nR <= 2000，程式碼極短！
struct Kuhn {
    int nL, nR;
    vector<vec> adj;
    vec matchR, vis; // matchR[v] = 右邊第 v 個點配給左邊哪個點 (0 代表未配對)
    Kuhn(int nL, int nR) : nL(nL), nR(nR), adj(nL + 1), matchR(nR + 1, 0), vis(nR + 1, 0) {}
    void add_edge(int u, int v) { adj[u].pb(v); } // 左 u (1..nL) 連到 右 v (1..nR)

    bool dfs(int u, int tag) {
        for (int i = 0; i < (int)adj[u].size(); i++) {
            int v = adj[u][i];
            if (vis[v] == tag) continue;
            vis[v] = tag;
            if (!matchR[v] || dfs(matchR[v], tag)) {
                matchR[v] = u;
                return true;
            }
        }
        return false;
    }
    int max_matching() {
        int ans = 0;
        for (int i = 1; i <= nL; i++) if (dfs(i, i)) ans++;
        return ans;
    }
};

// 2. Hopcroft-Karp O(E * sqrt(V))：適合 nL, nR 高達 10^5 的大型二分圖
struct HopcroftKarp {
    int nL, nR;
    vector<vec> adj;
    vec matchL, matchR, dist;
    HopcroftKarp(int nL, int nR) : nL(nL), nR(nR), adj(nL + 1),
                                   matchL(nL + 1, 0), matchR(nR + 1, 0), dist(nL + 1, 0) {}
    void add_edge(int u, int v) { adj[u].pb(v); }
    bool bfs() {
        queue<int> q;
        bool found = false;
        for (int i = 1; i <= nL; i++) {
            if (!matchL[i]) { dist[i] = 0; q.push(i); }
            else dist[i] = -1;
        }
        while (!q.empty()) {
            int u = q.front(); q.pop();
            for (int i = 0; i < (int)adj[u].size(); i++) {
                int nxt = matchR[adj[u][i]];
                if (!nxt) found = true;
                else if (dist[nxt] == -1) { dist[nxt] = dist[u] + 1; q.push(nxt); }
            }
        }
        return found;
    }
    bool dfs(int u) {
        for (int i = 0; i < (int)adj[u].size(); i++) {
            int v = adj[u][i], nxt = matchR[v];
            if (!nxt || (dist[nxt] == dist[u] + 1 && dfs(nxt))) {
                matchL[u] = v; matchR[v] = u;
                return true;
            }
        }
        dist[u] = -1;
        return false;
    }
    int max_matching() {
        int ans = 0;
        while (bfs())
            for (int i = 1; i <= nL; i++)
                if (!matchL[i] && dfs(i)) ans++;
        return ans;
    }
};

// === 實戰呼叫範例：CSES School Dance (n 個男生配 m 個女生，印出最多幾對與配對名單) ===
void voids() {
    int nL, nR, k;
    cin >> nL >> nR >> k;
    Kuhn bm(nL, nR);
    for (int i = 0; i < k; i++) {
        int u, v; cin >> u >> v;
        bm.add_edge(u, v);
    }
    cout << bm.max_matching() << "\n";
    for (int v = 1; v <= nR; v++) {
        if (bm.matchR[v] != 0) cout << bm.matchR[v] << " " << v << "\n";
    }
}
```

---

### 8.3 最大流／最小割 `Dinic`｜`0/1-based 皆可`｜$O(V^2 E)$

- **何時用**：水管最大流量、任務分配、**最小割（用最小總邊權切斷起點 `s` 到終點 `t`）**。
- **找最小割集合**：跑完 `din.max_flow(s, t)` 後，所有滿足 `din.lev[u] != -1` 的點都在源點 `s` 這一邊，滿足 `din.lev[u] == -1` 的點都在匯點 `t` 那一邊！

```cpp
struct Dinic {
    struct Edge { int to, rev, cap; };
    int n;
    vector<vector<Edge>> adj;
    vec lev, ptr;
    Dinic(int n) : n(n), adj(n + 1), lev(n + 1), ptr(n + 1) {}

    // 加入 u -> v 容量為 cap 的有向邊 (若為無向水管，把第 4 個參數傳 true)
    void add_edge(int u, int v, int cap, bool undirected = false) {
        Edge a = {v, (int)adj[v].size(), cap};
        Edge b = {u, (int)adj[u].size(), undirected ? cap : 0};
        adj[u].pb(a); adj[v].pb(b);
    }
    bool bfs(int s, int t) {
        fill(be(lev), -1);
        queue<int> q;
        lev[s] = 0; q.push(s);
        while (!q.empty()) {
            int u = q.front(); q.pop();
            for (int i = 0; i < (int)adj[u].size(); i++) {
                Edge &e = adj[u][i];
                if (e.cap > 0 && lev[e.to] == -1) {
                    lev[e.to] = lev[u] + 1;
                    q.push(e.to);
                }
            }
        }
        return lev[t] != -1;
    }
    int dfs(int u, int t, int pushed) {
        if (pushed == 0 || u == t) return pushed;
        for (int &cid = ptr[u]; cid < (int)adj[u].size(); cid++) {
            Edge &e = adj[u][cid];
            if (e.cap > 0 && lev[e.to] == lev[u] + 1) {
                int tr = dfs(e.to, t, min(pushed, e.cap));
                if (tr > 0) {
                    e.cap -= tr;
                    adj[e.to][e.rev].cap += tr;
                    return tr;
                }
            }
        }
        return 0;
    }
    int max_flow(int s, int t) {
        int flow = 0;
        while (bfs(s, t)) {
            fill(be(ptr), 0);
            while (int pushed = dfs(s, t, inf)) flow += pushed;
        }
        return flow;
    }
};

// === 實戰呼叫範例：求點 1 到點 n 的最大流 ===
void voids() {
    int n, m;
    cin >> n >> m;
    Dinic din(n); // 若有自己多開超級源匯點 S=0, T=n+1，記得傳 Dinic din(n + 1)！
    for (int i = 0; i < m; i++) {
        int u, v, cap; cin >> u >> v >> cap;
        din.add_edge(u, v, cap);
    }
    cout << din.max_flow(1, n) << "\n";
}
```

---

### 8.4 最小費用最大流 `MCMF`｜`0/1-based 皆可`

- **何時用**：每條邊有容量 `cap` 且每流 1 單位要花費 `cost`，求流最多流量的前提下最小總花費（無負費用環）。

```cpp
struct MCMF {
    struct Edge { int to, rev, cap, cost; };
    int n;
    vector<vector<Edge>> adj;
    MCMF(int n) : n(n), adj(n + 1) {}
    void add_edge(int u, int v, int cap, int cost) {
        Edge a = {v, (int)adj[v].size(), cap, cost};
        Edge b = {u, (int)adj[u].size(), 0, -cost};
        adj[u].pb(a); adj[v].pb(b);
    }
    // 回傳 pii(最大流量, 最小總花費)；若只要求流剛好 K 單位，第三個參數傳 K！
    pii min_cost_flow(int s, int t, int maxf = inf) {
        int flow = 0, cost = 0;
        vec dist(n + 1), pv(n + 1), pe(n + 1);
        vector<bool> in_q(n + 1);
        while (flow < maxf) {
            fill(be(dist), inf); fill(be(in_q), false);
            queue<int> q;
            dist[s] = 0; q.push(s); in_q[s] = true;
            while (!q.empty()) {
                int u = q.front(); q.pop(); in_q[u] = false;
                for (int i = 0; i < (int)adj[u].size(); i++) {
                    Edge &e = adj[u][i];
                    if (e.cap > 0 && dist[u] + e.cost < dist[e.to]) {
                        dist[e.to] = dist[u] + e.cost;
                        pv[e.to] = u; pe[e.to] = i;
                        if (!in_q[e.to]) { q.push(e.to); in_q[e.to] = true; }
                    }
                }
            }
            if (dist[t] == inf) break;
            int push = maxf - flow;
            for (int v = t; v != s; v = pv[v]) push = min(push, adj[pv[v]][pe[v]].cap);
            for (int v = t; v != s; v = pv[v]) {
                Edge &e = adj[pv[v]][pe[v]];
                e.cap -= push;
                adj[v][e.rev].cap += push;
            }
            flow += push;
            cost += push * dist[t];
        }
        return make_pair(flow, cost);
    }
};

// === 實戰呼叫範例 ===
void voids() {
    int n, m, k; cin >> n >> m >> k;
    MCMF mcmf(n);
    for (int i = 0; i < m; i++) {
        int u, v, cap, cost; cin >> u >> v >> cap >> cost;
        mcmf.add_edge(u, v, cap, cost);
    }
    pii res = mcmf.min_cost_flow(1, n, k); // 嘗試送 k 單位包裹從 1 到 n
    if (res.fi < k) cout << -1 << "\n";    // 最大流不到 k，送不完
    else            cout << res.se << "\n";// 印出最小總費用
}
```

---

### 8.5 `2-SAT`（二元布林條件滿足問題）｜變數 `0-based (0 ~ n-1)`｜$O(V + E)$

- **何時用**：$n$ 道料理／開關，每個只能選 `+` (`true`) 或 `-` (`false`)，每個人的兩個願望至少要滿足一個（需先貼 7.1 `TarjanSCC`）。

```cpp
struct TwoSat {
    int n;
    TarjanSCC scc;
    vector<bool> ans; // ans[i]: 第 i 個變數最終選 true 還是 false (0 ~ n-1)
    TwoSat(int n) : n(n), scc(2 * n), ans(n, false) {}
    int node(int x, bool val) { return 2 * x + (val ? 1 : 0) + 1; }

    void add_implies(int x, bool vx, int y, bool vy) {
        scc.add_edge(node(x, vx), node(y, vy));
        scc.add_edge(node(y, !vy), node(x, !vx));
    }
    // 加入條件：(x == vx) 或 (y == vy) 至少一個成立！
    void add_or(int x, bool vx, int y, bool vy) { add_implies(x, !vx, y, vy); }
    // 強制指定：x 必須等於 vx
    void set_val(int x, bool vx) { add_or(x, vx, x, vx); }

    bool solve() {
        scc.build();
        for (int i = 0; i < n; i++) {
            int f = scc.scc_id[node(i, false)], t = scc.scc_id[node(i, true)];
            if (f == t) return false; // 同一變數的 true 與 false 互推 -> 矛盾無解！
            ans[i] = (t < f);
        }
        return true;
    }
};

// === 實戰呼叫範例：CSES Giant Pizza (m 種配料，n 個人每人提兩個喜好至少滿足一個) ===
void voids() {
    int n_people, m_toppings;
    cin >> n_people >> m_toppings;
    TwoSat sat(m_toppings);
    for (int i = 0; i < n_people; i++) {
        char c1, c2; int x1, x2;
        cin >> c1 >> x1 >> c2 >> x2; // 輸入如: + 1 - 2 (代表要加 1 號配料 或 不加 2 號配料)
        sat.add_or(x1 - 1, c1 == '+', x2 - 1, c2 == '+'); // 轉 0-based！
    }
    if (!sat.solve()) cout << "IMPOSSIBLE\n";
    else {
        for (int i = 0; i < m_toppings; i++) cout << (sat.ans[i] ? "+ " : "- ");
        cout << "\n";
    }
}
```

---

## 9. 字串演算法 (String Algorithms)

### 9.1 雙模數 `DoubleHash`（直接使用你的 `mod1` 與 `mod2`！）｜`0-based`｜建 $O(n)$，查 $O(1)$

- **何時用**：$O(1)$ 判斷任意兩個子字串 `s[l1..r1]` 與 `s[l2..r2]` 是否相等！

```cpp
struct DoubleHash {
    static const int B = 13131;
    vec h1, h2, p1, p2;
    DoubleHash(const string &s) { // 傳入 0-based 字串 s
        int n = (int)s.size();
        h1.assign(n + 1, 0); h2.assign(n + 1, 0);
        p1.assign(n + 1, 1); p2.assign(n + 1, 1);
        for (int i = 0; i < n; i++) {
            h1[i + 1] = (h1[i] * B + s[i]) % mod1;
            h2[i + 1] = (h2[i] * B + s[i]) % mod2;
            p1[i + 1] = p1[i] * B % mod1;
            p2[i + 1] = p2[i] * B % mod2;
        }
    }
    // O(1) 取出閉區間子字串 s[l..r] (0 <= l <= r < n) 的雙雜湊值，可直接用 == 比對！
    pii get(int l, int r) const {
        int v1 = (h1[r + 1] - h1[l] * p1[r - l + 1] % mod1 + mod1) % mod1;
        int v2 = (h2[r + 1] - h2[l] * p2[r - l + 1] % mod2 + mod2) % mod2;
        return make_pair(v1, v2);
    }
};

// === 實戰呼叫範例：判斷字串前 3 個字與後 3 個字是否完全相同 ===
void voids() {
    string s; cin >> s;
    int n = (int)s.size();
    DoubleHash hs(s);
    if (hs.get(0, 2) == hs.get(n - 3, n - 1)) Yes;
    else No;
}
```

---

### 9.2 `KMP` 字串匹配與最小週期｜`0-based`｜$O(n + m)$

```cpp
vec build_pi(const string &p) {
    int n = (int)p.size();
    vec pi(n, 0);
    for (int i = 1; i < n; i++) {
        int j = pi[i - 1];
        while (j > 0 && p[i] != p[j]) j = pi[j - 1];
        if (p[i] == p[j]) j++;
        pi[i] = j;
    }
    return pi;
}

// 找出 pat 在 text 中所有出現的「起始下標 (0-based)」
vec kmp_search(const string &text, const string &pat) {
    vec pi = build_pi(pat), res;
    int j = 0, n = (int)text.size(), m = (int)pat.size();
    for (int i = 0; i < n; i++) {
        while (j > 0 && text[i] != pat[j]) j = pi[j - 1];
        if (text[i] == pat[j]) j++;
        if (j == m) { res.pb(i - m + 1); j = pi[j - 1]; }
    }
    return res;
}

// === 實戰呼叫範例 ===
void voids() {
    string text, pat;
    cin >> text >> pat;
    vec pos = kmp_search(text, pat);
    cout << pos.size() << "\n"; // 印出總共出現幾次
    // [附錄技巧] 字串最小重複週期：vec pi = build_pi(s); int len = n - pi[n-1];
}
```

---

### 9.3 `Z-function`（擴展 KMP：求每個後綴與原字串的最長共同前綴）｜`0-based`｜$O(n)$

```cpp
// Z-function：z[i] 為子字串 s[i..n-1] 與原字串 s[0..n-1] 的最長共同前綴長度
vec z_function(const string &s) {
    int n = (int)s.size();
    vec z(n, 0);
    z[0] = n;
    for (int i = 1, l = 0, r = 0; i < n; i++) {
        if (i <= r) z[i] = min(r - i + 1, z[i - l]);
        while (i + z[i] < n && s[z[i]] == s[i + z[i]]) z[i]++;
        if (i + z[i] - 1 > r) { l = i; r = i + z[i] - 1; }
    }
    return z;
}

// ==================== void voids() 實戰範例 ====================
// 用 Z-function 做字串匹配：把 pattern + "#" + text 拼起來，看哪些位置的 z[i] == pattern.size()
void voids() {
    string t, p;
    cin >> t >> p;
    string s = p + "#" + t;
    vec z = z_function(s);
    int m = (int)p.size();
    int cnt = 0;
    for (int i = m + 1; i < (int)s.size(); i++) {
        if (z[i] == m) cnt++;
    }
    cout << cnt << "\n";
}
```

---

### 9.4 `Manacher` 最長回文子字串｜`0-based`｜$O(n)$

```cpp
// Manacher：O(n) 直接回傳字串 s 中最長的回文子字串！
string manacher(const string &s) {
    string t = "#";
    for (int i = 0; i < (int)s.size(); i++) { t += s[i]; t += '#'; }
    int n = (int)t.size(), c = 0, r = 0, best_len = 0, best_center = 0;
    vec p(n, 0); // p[i] 剛好等於原字串對應位置的最長回文長度
    for (int i = 0; i < n; i++) {
        if (i < r) p[i] = min(r - i, p[2 * c - i]);
        while (i - p[i] - 1 >= 0 && i + p[i] + 1 < n && t[i - p[i] - 1] == t[i + p[i] + 1])
            p[i]++;
        if (i + p[i] > r) { c = i; r = i + p[i]; }
        if (p[i] > best_len) { best_len = p[i]; best_center = i; }
    }
    return s.substr((best_center - best_len) / 2, best_len);
}

// ==================== void voids() 實戰範例 ====================
void voids() {
    string s;
    cin >> s;
    cout << manacher(s) << "\n"; // 直接印出最長回文子字串（若問長度加 .size()）
}
```

---

### 9.5 字典樹 `Trie` ＆ `XorTrie`（最大 XOR 配對）

```cpp
// 1. 小寫英文字母字典樹 Trie
struct Trie {
    struct Node {
        int nxt[26];
        int pass, end_cnt; // pass: 有幾個字經過此節點(前綴數)；end_cnt: 有幾個字在此結尾
        Node() : pass(0), end_cnt(0) { memset(nxt, 0, sizeof(nxt)); }
    };
    vector<Node> tr;
    Trie() { tr.pb(Node()); }
    void insert(const string &s) {
        int u = 0;
        for (int i = 0; i < (int)s.size(); i++) {
            int c = s[i] - 'a';
            if (!tr[u].nxt[c]) { tr[u].nxt[c] = (int)tr.size(); tr.pb(Node()); }
            u = tr[u].nxt[c];
            tr[u].pass++;
        }
        tr[u].end_cnt++;
    }
    int count_prefix(const string &p) { // 查詢有多少已插入單字以 p 為開頭前綴
        int u = 0;
        for (int i = 0; i < (int)p.size(); i++) {
            int c = p[i] - 'a';
            if (!tr[u].nxt[c]) return 0;
            u = tr[u].nxt[c];
        }
        return tr[u].pass;
    }
};

// 2. 0-1 Trie：動態新增/刪除整數，O(60) 查集合中誰跟 x 做 XOR 最大！
struct XorTrie {
    static const int B = 60;
    struct Node {
        int nxt[2], cnt;
        Node() : cnt(0) { nxt[0] = nxt[1] = 0; }
    };
    vector<Node> tr;
    XorTrie() { tr.pb(Node()); }
    void insert(int x, int delta = 1) { // delta = +1 插入數字 x；delta = -1 刪除一個 x
        int u = 0;
        for (int i = B; i >= 0; i--) {
            int b = (x >> i) & 1;
            if (!tr[u].nxt[b]) { tr[u].nxt[b] = (int)tr.size(); tr.pb(Node()); }
            u = tr[u].nxt[b];
            tr[u].cnt += delta;
        }
    }
    int max_xor(int x) { // 集合必須非空！回傳 max(x ^ y)
        int u = 0, res = 0;
        for (int i = B; i >= 0; i--) {
            int b = (x >> i) & 1, want = b ^ 1;
            if (tr[u].nxt[want] && tr[tr[u].nxt[want]].cnt > 0) {
                res |= (1LL << i);
                u = tr[u].nxt[want];
            } else u = tr[u].nxt[b];
        }
        return res;
    }
};

// === 實戰呼叫範例：給 n 個數字，找任選兩數 XOR 的最大值 ===
void voids() {
    int n; cin >> n;
    XorTrie xt;
    int ans = 0;
    for (int i = 0; i < n; i++) {
        int x; cin >> x;
        if (i > 0) ans = max(ans, xt.max_xor(x));
        xt.insert(x, 1);
    }
    cout << ans << "\n";
}
```

---

## 10. 計算幾何 2D (Computational Geometry)

### 10.1 點向量、轉向判定 `ccw`、線段相交、多邊形面積、凸包 `Convex Hull`

- **幾何黃金守則**：全部使用整數 `int` (`long long`) 運算，零浮點數誤差！多邊形面積的 **2 倍** 必為整數。

```cpp
struct Pt {
    int x, y;
    Pt(int x = 0, int y = 0) : x(x), y(y) {}
    Pt operator+(const Pt &o) const { return Pt(x + o.x, y + o.y); }
    Pt operator-(const Pt &o) const { return Pt(x - o.x, y - o.y); }
    bool operator<(const Pt &o) const { return x != o.x ? x < o.x : y < o.y; }
    bool operator==(const Pt &o) const { return x == o.x && y == o.y; }
};
int dot(Pt a, Pt b) { return a.x * b.x + a.y * b.y; }   // 內積
int cross(Pt a, Pt b) { return a.x * b.y - a.y * b.x; } // 外積

// 1. 轉向判定 ccw(a, b, c)：從 a 走到 b 再看 c
// 回傳 +1 代表逆時針左轉；-1 代表順時針右轉；0 代表三點共線
int ccw(Pt a, Pt b, Pt c) {
    int v = cross(b - a, c - a);
    return (v > 0) - (v < 0);
}

// 2. 線段相交判定：線段 ab 與線段 cd 是否有交點 (含端點相碰與共線重疊)
bool on_seg(Pt a, Pt b, Pt p) { // 點 p 是否落在線段 ab 上
    return ccw(a, b, p) == 0 && dot(a - p, b - p) <= 0;
}
bool seg_intersect(Pt a, Pt b, Pt c, Pt d) {
    int c1 = ccw(a, b, c), c2 = ccw(a, b, d);
    int c3 = ccw(c, d, a), c4 = ccw(c, d, b);
    if (c1 * c2 < 0 && c3 * c4 < 0) return true;
    return on_seg(a, b, c) || on_seg(a, b, d) || on_seg(c, d, a) || on_seg(c, d, b);
}

// 3. 多邊形面積的「2 倍」(依序傳入頂點；實際面積為 polygon_area2(p) / 2.0)
int polygon_area2(const vector<Pt> &p) {
    int area2 = 0, n = (int)p.size();
    for (int i = 0; i < n; i++) area2 += cross(p[i], p[(i + 1) % n]);
    return abs(area2);
}

// 4. 凸包 Convex Hull O(n log n)：回傳逆時針順序的外圍頂點
// (預設去除邊上共線點；若題目要求保留凸包邊界上的共線點，把 <= 0 改成 < 0！)
vector<Pt> convex_hull(vector<Pt> pts) {
    mkunique(pts); // 使用你的巨集排序並去除重複點！
    int n = (int)pts.size();
    if (n <= 1) return pts;
    vector<Pt> h;
    for (int phase = 0; phase < 2; phase++) {
        int start = (int)h.size();
        for (int i = 0; i < n; i++) {
            while ((int)h.size() >= start + 2 && ccw(h[(int)h.size() - 2], h.back(), pts[i]) <= 0)
                h.pop_back();
            h.pb(pts[i]);
        }
        h.pop_back();
        reverse(be(pts));
    }
    return h;
}

// === 實戰呼叫範例 ===
void voids() {
    int n; cin >> n;
    vector<Pt> pts(n);
    for (int i = 0; i < n; i++) cin >> pts[i].x >> pts[i].y;
    vector<Pt> hull = convex_hull(pts);
    cout << hull.size() << "\n";
    for (int i = 0; i < (int)hull.size(); i++) cout << hull[i].x << " " << hull[i].y << "\n";
}
```

---

## 11. C++ STL 容器與內建函式完整拼字速查字典

> 考場忘記函式怎麼拼、參數順序誰先誰後、或不能用 `auto` 時，直接翻到這一章照抄！

### 11.1 `vector` 與 `string` 與字元／字串轉型

| 功能說明 | 正確拼字與寫法（相容你的模板巨集） | 重要提醒 |
| :--- | :--- | :--- |
| 建立長度 `n` 初值為 `v` 的陣列 | `vec a(n, v);` | 二維用你的 `grid(n, m, a);` |
| 重新設定大小並填初值 `0` | `a.assign(n, 0);` | 多筆測資清空重設大小最好用！ |
| 加到尾端／刪掉尾端 | `a.pb(x);` / `a.pop_back();` | 空陣列不可 `pop_back()` |
| 取第一個／最後一個元素 | `a.front()` / `a.back()` | 等同 `a[0]` 與 `a[a.size()-1]` |
| 在第 `i` 個位置插入／刪除 | `a.insert(a.begin() + i, x);` / `a.erase(a.begin() + i);` | 複雜度 $O(n)$，勿在迴圈狂用 |
| 取子字串 | `s.substr(pos, len)` | **第 2 個參數是長度 `len`，不是右界！** 省略 `len` 則取到結尾 |
| 尋找子字串位置 | `int p = s.find("abc");` | 找不到時 `p == (int)string::npos`（轉 `int` 會是 `-1`） |
| 讀取整行含空白字串 | `cin >> ws; getline(cin, s);` | `cin >> ws` 會自動吃掉前一個數字留下的換行符號！ |
| 字串轉整數／整數轉字串 | `stoll(s)` / `to_string(x)` | 若極舊非 C++11 環境用 `atoll(s.c_str())` |
| 用空白切開整行數字／單字 | `stringstream ss(line); while (ss >> word) { ... }` | 需 `#include <sstream>` |
| 字元分類與大小寫轉換 | `isdigit(c)`, `isalpha(c)`, `isupper(c)`, `islower(c)`, `tolower(c)`, `toupper(c)` | `tolower` 回傳 `int`，印出時要轉 `(char)tolower(c)` |

---

### 11.2 `queue`、`stack`、`deque`、`priority_queue`（堆）

| 容器 | 宣告方式 | 新增元素 | 看最上面／最前面 | 彈出元素 |
| :--- | :--- | :--- | :--- | :--- |
| 一般佇列 (FIFO) | `queue<int> q;` | `q.push(x);` | `q.front()` | `q.pop();` |
| 堆疊 (LIFO) | `stack<int> st;` | `st.push(x);` | `st.top()` *(注意不是 front!)* | `st.pop();` |
| 雙端佇列 | `deque<int> dq;` | `dq.push_front(x);` / `dq.pb(x);` | `dq.front()` / `dq.back()` / `dq[i]` | `dq.pop_front();` / `dq.pop_back();` |
| 大根堆 (最大在頂) | `p_q pq;` *(你的巨集)* | `pq.push(x);` | `pq.top()` | `pq.pop();` |
| 小根堆 (最小在頂) | `rp_q pq;` *(你的巨集)* | `pq.push(x);` | `pq.top()` | `pq.pop();` |
| `pii` 小根堆 | `priority_queue<pii, vector<pii>, greater<pii> > pq;` | `pq.push(make_pair(d, u));` | `pq.top().fi` | `pq.pop();` |

---

### 11.3 `set`、`multiset`、`map`（紅黑樹容器與不用 `auto` 的迭代器寫法）

```cpp
// 1. set (自動由小到大排序、且自動去重)
set<int> st;
st.insert(10);                      // 新增 O(log n)
st.erase(10);                       // 刪除數值 10 O(log n)
if (st.count(10)) { ... }           // 檢查 10 是否存在 (回傳 0 或 1)
int mn = *st.begin();               // 最小值 (前提：!st.empty())
int mx = *st.rbegin();              // 最大值 (前提：!st.empty())

// [重要] set 二分搜必須用「st.lower_bound(x)」，不可寫 lb(st, x)！
set<int>::iterator it = st.lower_bound(x); // 找第一個 >= x 的 iterator (找不到為 st.end())
if (it != st.end()) cout << *it << "\n";
// 如何找「嚴格小於 x 的最大值」？
set<int>::iterator it2 = st.lower_bound(x);
if (it2 != st.begin()) { --it2; cout << *it2 << "\n"; } // 往左退一格就是 < x 的最大值！

// 2. multiset (允許重複數字的 set) — 刪單一元素必看地雷！
multiset<int> ms;
ms.insert(5); ms.insert(5);
// ms.erase(5);                     // [地雷！] 這行會把「所有的 5」全部刪光！
if (ms.find(5) != ms.end()) {
    ms.erase(ms.find(5));           // [正確！] 傳入 iterator 只會刪掉「其中一個 5」！
}

// 3. map (字典 key -> value，按 key 由小到大排)
map<string, int> mp;
mp["apple"] += 1;
if (mp.count("apple")) { ... }      // 檢查 key 是否存在 (別寫 if (mp["x"])，會多塞一個 0 進去！)
// 不用 auto 遍歷整個 map 的標準寫法：
for (map<string, int>::iterator mit = mp.begin(); mit != mp.end(); ++mit) {
    cout << mit->fi << " -> " << mit->se << "\n";
}
```

---

### 11.4 `<algorithm>`、`<numeric>`、`<cmath>`、位元與輸出格式全表

```cpp
// === 1. 排序與自訂比較函式 ===
sort(be(a));                        // 由小到大排序
sort(rbe(a));                       // 由大到小排序
// 自訂排序：例如 pii 先按 fi 由小到大，fi 相同時按 se 由大到小
bool cmp(const pii &a, const pii &b) {
    if (a.fi != b.fi) return a.fi < b.fi;
    return a.se > b.se;             // [鐵則] 比較函式在兩者相等時必須回傳 false (嚴格用 < 或 >，不可寫 <=)！
}
// 呼叫：sort(be(v), cmp);

// === 2. 常見序列操作 ===
reverse(be(a));                     // 陣列原地反轉
int mx = *max_element(be(a));       // 找整個陣列最大值 O(n)
int mn = *min_element(be(a));       // 找整個陣列最小值 O(n)
int sum = accumulate(be(a), 0LL);   // 陣列總和 (第二個參數務必寫 0LL 防 32-bit 溢位！)
iota(be(a), 1);                     // 把 a 依序填入 1, 2, 3, ..., n
fill(be(a), -1);                    // 把 vector 全部填成任意數字 (如 -1 或 inf)
memset(arr, 0, sizeof(arr));        // C 陣列清空：只能填 0 或 -1！(填其他數字會壞掉)
nth_element(a.begin(), a.begin() + k, a.end()); // O(n) 讓 a[k] 變成第 k 小 (0-based)

// === 3. 全排列枚舉 (N <= 10 暴搜神器) ===
sort(be(a));                        // [必寫！] 一定要先排成最小字典序，才會枚舉出所有排列！
do {
    // 處理當前排列 a
} while (next_permutation(be(a)));

// === 4. 數學、無條件進位、位元內建函式 ===
int ceil_div = (a + b - 1) / b;     // 正整數 a 除以 b 無條件進位 (別用 ceil(double) 會失準！)
double pi = acos(-1.0);             // 最精確的圓周率 PI
double dist = hypot(dx, dy);        // 計算 sqrt(dx*dx + dy*dy) 不易溢位
int ones = __builtin_popcountll(x); // x 的二進位有幾個 1 (記得結尾加 ll！)
int tz   = __builtin_ctzll(x);      // x 二進位末尾有幾個 0 (x 不可為 0)
int lg   = 63 - __builtin_clzll(x); // floor(log2(x)) (x >= 1)

// === 5. bitset (64 倍加速布林陣列 / 存在性背包) ===
bitset<10005> bs;
bs[0] = 1;
bs |= (bs << w);                    // 一行完成容量 10000 的湊數問題！bs.count() 可查有幾個 1

// === 6. 小數點精度與補零輸出格式 ===
cout << fixed << setprecision(10) << ans_double << "\n"; // 固定印出小數點後 10 位
cout << setw(4) << setfill('0') << 7 << "\n";            // 印出 "0007"
```

---
