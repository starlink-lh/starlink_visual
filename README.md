# starlink_visual
starlink_visual

#2022.6.30总结GitHub上传项目  
1.下载Git，找一个空白文件夹  
2.右键Git Bash Here  
3. git init  
4.将要加入项目的文件添加到该空白文件夹中  
5.git add .  
注：  
warning: LF will be replaced by CRLF in satvis-master/satvis-master/data/cesium-assets/README.md.
The file will have its original line endings in your working directory
如果文件夹中存在隐藏文件如 .git 文件则报错，可以将其删除则可正常运行  
报错：warning: LF will be replaced by CRLF in   
解决办法：git config core.autocrlf false  
6.git status 查看状态  
7.git commit -m "注释"  
8.git remote add 仓库地址  
注：Git出现 fatal: ‘origin‘ does not appear to be a git repository fatal: Could not read from remote  
解决办法：https://blog.csdn.net/weixin_47872288/article/details/124944945  
git remote -v，查看仓库信息是否正确  
git remote remove orign，删除远程仓库  
git remote add origin 仓库，重新添加远程仓库  
git push -u origin master，提交信息到master仓库  
9.git push -u origin master  
注：  
会出现错误：fatal: unable to access 'https://github.com/mzLiuGitHub/satvis_demo.git/': OpenSSL SSL_read: Connection was reset, errno 10054  
解决办法：git config --global http.sslVerify false  
会出现错误：fatal: unable to access 'https://github.com/mzLiuGitHub/satvis_demo.git/': Failed to connect to github.com port 443 after 21076 ms: Timed out  
解决办法：连不上github重新连接  
出现错误：error: RPC failed; curl 92 HTTP/2 stream 0 was not closed cleanly: CANCEL (err 8)  
send-pack: unexpected disconnect while reading sideband packet  
Writing objects: 100% (3032/3032), 47.35 MiB | 1.19 MiB/s, done.  
Total 3032 (delta 7), reused 0 (delta 0), pack-reused 0  
fatal: the remote end hung up unexpectedly  
解决办法：git config --global http.version HTTP/1.1  
10.SSH Key如何获取设置  
https://blog.csdn.net/qq_40770527/article/details/124129505  
