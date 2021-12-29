# Cloud189Checkin 

天翼云盘每日签到1次，抽奖2次，支持多账号

forked from peng4740/Cloud189Checkin-Actions: 
> [Cloud189Checkin-Actions](https://github.com/peng4740/Cloud189Checkin-Actions)

## 问题修复

1. 替换了失效的天翼云链接
2. 修正了随机等待不生效的问题
3. 优化了脚本代码和注释日志等

# Github Actions 使用说明

## 一、Fork此仓库

![](http://tu.yaohuo.me/imgs/2020/06/f059fe73afb4ef5f.png)

## 二、设置账号密码

- 点击**Settings**->**Secrets**->**New repository secret**
- 添加名为**USER**、**PWD**的变量，值分别为天翼云**账号**、**密码**
- 支持多账号，每个账号密码换行，个数必须一致

![](http://tu.yaohuo.me/imgs/2020/06/748bf9c0ca6143cd.png)
![](http://tu.yaohuo.me/imgs/2020/06/af2013b1ef5d8430.png)
![](http://tu.yaohuo.me/imgs/2020/06/09c22adcec7b5d81.png)

## 三、启用Action

点击**Actions**->**I understand my workflows, go ahead and enable them**->**Cloud189Checkin**->**Enable workflow**

![](http://tu.yaohuo.me/imgs/2020/06/34ca160c972b9927.png)
![](https://img30.360buyimg.com/pop/jfs/t1/137697/35/24762/20419/61cbff27Efd9e518d/9b072cf86c6961b4.png)

## 四、运行并查看结果

- 修改任意文件后提交一次，或在每日10点、22点自动运行（可在[.github/workflows/run.yml]修改）
- 运行后点击**Actions**>**Cloud189Checkin**>**运行记录**->**build**查看日志

![](https://img30.360buyimg.com/pop/jfs/t1/108313/33/20285/22039/61cc0745Ef1953d3e/3871dccc4848aed5.png)
![](https://img30.360buyimg.com/pop/jfs/t1/139516/3/24951/19019/61cc0745E43aa6c2b/d040f842f69110a3.png)
![](https://img30.360buyimg.com/pop/jfs/t1/220941/38/9351/24245/61cc069fE5f0cc7c8/0c20670e18a1473c.png)

## 可能遇到的问题

1. 用户名或密码错误：确认用户名密码是否填写正确，手机号和别名不要填写多余的邮箱后缀，查看账号安全是否已经关闭设备锁
2. 验证码错误：可能账号多次登录失败，图片验证码暂未识别，需手动登录或等待账号异常状态解除

## 关于账号安全

本版本仅会打印用户名前3位作为日志记录，不会泄露完整用户名和密码信息。 
