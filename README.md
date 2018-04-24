cifaz.xwiki
========================
  
安装
```
ansible-galaxy install cifaz.xwiki
```
  
### 运行, 安装前, 请先安装tomcat, 设置进行相应的设置
```
- hosts: local
  remote_user: root
  roles:
    - {role: "cifaz.xwiki", tag: "xwiki"}


    配置项
    xwiki_version: 10.2
    xwiki_download_dir: /app/down/xwiki
    
    # 是否自动安装tomcat
    xwiki_tomcat_install: false
    # war包存放地址
    xwiki_tomcat_base_dir: /app/server/tomcat/
    xwiki_tomcat_web_dir: webapps/
    xwiki_tomcat_war_name: xwiki.war
    xwiki_tomcat_run_name: xwiki/
    xwiki_admin_open: true
```
  
License
-------

MIT

Author Information
------------------

ccz <hanlin2531@163.com>

