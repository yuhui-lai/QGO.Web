# QGO.Web

### appsettings.json
放資料庫連線等參數，分為以下3種版本
- appsettings.Production.json 正式
- appsettings.Staging.json 測試
- appsettings.Development.json 開發

### pubxml部署文件
- Production正式.pubxml
- Staging測試.pubxml: 修改執行環境(web.config)，iis執行時會吃appsettings.Staging.json設定檔
```xml
<!--測試環境-->
<EnvironmentName>Staging</EnvironmentName>
```

#### 模板flynext
套件放置於wwwroot/flynext/