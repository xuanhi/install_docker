# install_docker
ansible install docker

### 历史经历：

首先ansible-galaxy可以直接在当前目录创建roles目录结构，文件自动生成

初始化roles文件：

```bash
cd /etc/ansible/roles
ansible-galaxy init install_docker-ce
```

然后就行执行脚本。

### 使用方法

步骤一：在inventory 配置主机清单

步骤二：修改site.yml hosts:你配置的主机清单组

步骤三：

```bash
# 语法检查
ansible-playbook --syntax-check site.yaml  
```

```bash
# 预执行
ansible-playbook -C site.yaml
```

#### 如果都没问题就可以执行
```bash
ansible-playbook site.yaml
```
