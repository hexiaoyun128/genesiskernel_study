# golang环境配置
配置使用的用户名为cloudy
## 下载golang Linux二进制文件

* `wget https://dl.google.com/go/go1.10.linux-amd64.tar.gz`
* `tar zxfv go1.10.linux-amd64.tar.gz  -C /usr/local/` 需要sudo

## 配置环境变量

* 执行`vim /etc/profile` (可能需要sudo)增加下面的内容
<pre><code>
export GOROOT=/usr/local/go
export GOBIN=$GOROOT/bin
export PATH=$PATH:$GOBIN
export GOPATH=/home/cloudy/gowork
</code></pre>

* 执行 ` source /etc/profile`
* 检查验证 `go version`

