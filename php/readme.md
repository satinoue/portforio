# Virtual Env

## Tools
- virtualbox
- vagrant

## Setup
*Reference*
https://dotinstall.com/lessons/basic_localdev_win_v2/

- vagrant環境作成
動画と異なり、centos8とするため、こちらのコマンド実施
```
$ vagrant box add generic/centos8   (注：時間かかる)
$ vagrant init generic/centos8
```

- vagrantファイル編集

Vagrantファイルを開いて、下記をコメントアウト外す 
```
config.vm.network "private_network", ip: "192.168.33.10"
```

- vagrant起動
```
$ vagrant up (注：時間かかる)
$ vagrant status
```

- vagrantを終了 (ただし、仮想マシンは終了されない)
```
$ exit
```
または
```
$ vagrant halt
```

