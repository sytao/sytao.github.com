---
layout: post
title: "homebrew install mysql"
description: ""
category: ruby
tags: [ruby]
---
{% include JB/setup %}

第一个问题困扰了老子两天。NND...
##问题一：


`ERROR 2002 (HY000): Can't connect to local MySQL server through socket '/tmp/mysql.sock' (2)`


解决办法：[参考一](http://blog.csdn.net/jianglei421/article/details/7049433)

    ---
    # brew install mysql   
    #mysql_install_db --verbose --user=`whoami` --basedir="$(brew --prefix mysql)" --datadir=/usr/local/var/mysql --tmpdir=/tmp  
    # mkdir -p ~/Library/LaunchAgents (如果有此目录省去此步)  
    #cp "$(brew --prefix mysql)"/homebrew.mxcl.mysql.plist ~/Library/LaunchAgents  
    #launchctl load -w ~/Library/LaunchAgents/homebrew.mxcl.mysql.plist  
    #"$(brew --prefix mysql)"/bin/mysql_secure_installation 
    ---
