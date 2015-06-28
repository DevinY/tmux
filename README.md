Mac OS X編譯安裝tmux，可參考:
https://github.com/tmux/tmux


# 一些tmux的教學說明
這個設定檔是我從網路上拷來的在下方加入一些常用熱鍵的說明及基本的操作。

預設的<kbd>Ctrl</kbd>+<kbd>b</kbd>變更為<kbd>Ctrl</kbd>+<kbd>a</kbd>

用<kbd>h</kbd><kbd>j</kbd><kbd>k</kbd><kbd>l</kbd>在panel間移動，例如: <kbd>Ctrl</kbd>+<kbd>a</kbd>再壓<kbd>h</kbd>

用大寫的HJKL調整panel的大小.

<kbd>Ctrl</kbd>+<kbd>a</kbd>再壓<kbd>w</kbd>，開新視窗。

<hr>
##與設定檔無關的熱鍵備忘
<kbd>Ctrl</kbd>+<kbd>a</kbd>再壓<kbd>[</kbd>，進入拷貝模式(copy)，因為設定檔有啟動vim模式了，所以可用<kbd>/</kbd>搜尋
用<kbd>h</kbd><kbd>j</kbd><kbd>k</kbd><kbd>l</kbd>移動，連按<kbd>g</kbd><kbd>g</kbd>到最頂端等，懂Vim操作的人應該很熟悉，不過要選擇拷貝文字時，要先壓<kbd>v</kbd>，再壓<kbd>shift</kbd>+<kbd>v</kbd>即可選擇拷貝文字。

壓<kbd>/</kbd>搜尋時，可壓<kbd>Ctrl</kbd>+<kbd>u</kbd>清除搜尋的字串。

查看熱鍵說明:<kbd>Ctrl</kbd>+<kbd>a</kbd>再壓<kbd>?</kbd>即可

##Session相關的指令
開始一個新的session:

<pre><code>tmux new -s session名稱</code></pre>


list sessions:(列出 session):

<pre><code>tmux ls</code></pre>

attach:(也可以用at或是attach)

<pre><code>tmux a #</code></pre>

刪除session:
<pre><code>tmux kill-session -t #</code></pre>

