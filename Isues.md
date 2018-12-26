### q:Error: Could not link: /usr/local/share/doc/homebrew
### a:[转载](http://c.n-di.com/2017/07/17/1827.html)
  mac 执行brew update 报错 Error: Could not link: /usr/local/etc/bash_completion.d/brew
更新brew，报错；

Error: Could not link:
/usr/local/etc/bash_completion.d/brew

Please delete these paths and run `brew update`.
Error: Could not link:
/usr/local/share/zsh/site-functions/_brew

Please delete these paths and run `brew update`.
Error: Could not link:
/usr/local/share/man/man1/brew.1

Please delete these paths and run `brew update`.
Error: Could not link:
/usr/local/share/doc/homebrew

Please delete these paths and run `brew update`.
#### 解决办法

rm -rf /usr/local/etc/bash_completion.d/brew
rm -rf /usr/local/share/zsh/site-functions/_brew
rm -rf /usr/local/share/man/man1/brew.1
rm -rf /usr/local/share/doc/homebrew
brew update
