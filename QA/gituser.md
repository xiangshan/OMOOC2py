### git user
### 问题
-   在进行代码提交时提示没有权限提交代码
-   通过 git config －list检查配置状态时发现之前配置过git 全局用户


### git 的全局配置
    ```
    git config --global user.name "username"
    git config --global user.email "user@email.com"
    ```
### 删除git 全局用户
    ```
    git config --global --unset user.name "username"
    git config --global --unset user.email "user@email.com"
    ```
### git 当前项目配置用户
    ```
    git config user.name "user"
    git config user.email "user@email.com"
    ```
这样通过在单独项目中创建用户信息来保证多个用户单独操作。

* 同时在搜集关于多个用户的问题时发现涉及一种 “多个sshkey配置” 配置的方法
   - 并没有深入的进行尝试和测试
   - 在这里搜索相关信息花了很多时间，担心在配置sshkey会影响之前已经配置过的其它内容，而且之前配置了什么都没有纪录
   
* 在遇到这个问题时实际上拖延了很久，之后为了尽快同步gitbook 内容通过线上添加项目的方式把github中的项目添加到了gitbook中，并没有配置双推

