# [Odoo](https://www.odoo.com "Odoo's Homepage") Install Script


## 修改符合GCP安裝用途

##### 1.目前適用ubuntu 18.04 (test in 2019/04/10)

## 安裝流程

##### 1. 下載 script:
```
sudo wget https://raw.githubusercontent.com/skypc785308/InstallScript/11.0/odoo_install.sh
```
##### 2. 修改需要變更的參數
There are a few things you can configure, this is the most used list:<br/>
```OE_USER``` will be the username for the system user.<br/>
```OE_PORT``` is the port where Odoo should run on, for example 8069.<br/>
```OE_VERSION``` is the Odoo version to install, for example ```11.0``` for Odoo V11.<br/>
```OE_SUPERADMIN``` is the master password for this Odoo installation.<br/>

##### 3. 讓 script 有權限執行:
```
sudo chmod +x odoo_install.sh
```
##### 4. 執行 script:
```
sudo ./odoo_install.sh
```

##### 5. 完成，可以經由以下指令控制服務
```
# 開啟服務
sudo service odoo-server start
# 關閉服務
sudo service odoo-server stop
# 重啟服務
sudo service odoo-server restart
# 查看服務運行狀態
sudo service odoo-server status
```
