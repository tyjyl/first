问题1：fatal: not a git repository -> 解法：先执行 git init 初始化。

问题2：! [rejected] main -> main (fetch first) -> 解法：说明远程有东西，执行 git pull --allow-unrelated-histories 合并历史。

问题3：fatal: Not possible to fast-forward -> 解法：用 git merge origin/main 解决分叉，再 push。