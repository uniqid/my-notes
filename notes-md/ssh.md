#生成ssh公钥密钥对
ssh-keygen -b 2048 -t rsa

#设置别名
mv .ssh/id_dsa .ssh/alias_name

#.ssh/config 追加一下内容
HOST alias_name
    HOSTNAME remote_host
    PORT 22
    USER username
    IdentityFile ~/.ssh/scout


#拷贝公钥到远程服务器并设置
scp .ssh/id_dsa.pub username@remote_host:
ssh username@remote_host
cat id_dsa.pub >> authorized_keys
