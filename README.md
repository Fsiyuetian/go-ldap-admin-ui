<div align="center">
<h1>Go Ldap Admin</h1>

Fork from [go-ldap-admin-ui](https://github.com/opsre/go-ldap-admin-ui)
<br>
Fork time: 2024-12-02 16:00

<p> 🌉 基于Go+Vue实现的openLDAP后台管理项目 🌉</p>

</div><br>

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->



## 变更点

- 新增用户，用户名字段描述：用户名（大写工号）
- 修改用户界面，用户名和工号字段禁止修改
- 优化用户忘记密码界面，当点击"发送验证码"按钮时，提示"发送验证码成功."，并且"发送验证码"按钮置灰60s
- 修改login背景图
- 优化关于我的界面，显示Hello <中文名：nickname>


## 构建dist.zip

```bash
docker build -t ldap-admin-ui:v1 .
docker run -d --name ldapui --privileged ldap-admin-ui:v1 && docker cp ldapui:/app ./
mv app dist
zip -r dist.zip dist
```


<!-- readme: collaborators,contributors -end -->
