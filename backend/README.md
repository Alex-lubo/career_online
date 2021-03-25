# 系统介绍
本系统基于开源平台（https://github.com/mtianyan/OnlineMooc.git）开发。

采用Django3.1 + DjangoRestful Framework + Ant Design Pro V4 开发网站管理后台。

DjangoRestful Framework提供后端API功能。

使用TyAdmin(现代化的Xadmin替代品)生成管理后台前后端，并自动对接。TyAdmin的使用参考：
>https://github.com/mtianyan/tyadmin_api_cli 

前端采用Vue开发。基于开源项目[vue-mooc](https://github.com/mtianyan/vue-mooc)

## 系统运行
### 本地运行
#### django项目
依赖： mysql, python
首先安装依赖：
```
pip install -r requirements.txt
```
然后创建数据库
```
# 修改caeer_wky/settings/base.py下的DATABASES设置，设置mysql数据库连接设置
# 在mysql中创建与DATABASES字段中NAME属性匹配的数据库
# 导入career_wky.sql
# 然后运行系统
python manage.py runserver
```
#### 后台管理项目
管理后台前后端使用TyAdmin生成，生成过程
```
python manage.py gen
```




