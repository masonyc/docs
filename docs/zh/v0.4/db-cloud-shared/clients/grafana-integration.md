
GreptimeDB 服务可以配置为 [Grafana 数据源](https://grafana.com/docs/grafana/latest/datasources/add-a-data-source/)。

## Prometheus

单击 Add data source 按钮，然后选择 Prometheus 作为类型。

在 HTTP 中填写 Prometheus server URL

- GreptimeCloud 请填写 `https://<host>/v1/prometheus?db=<dbname>`
- 自托管 GreptimeDB 请填写自己的地址，例如：`http://localhost:4000/v1/prometheus?db=<dbname>`

在 Auth 部分中单击 basic auth，并在 Basic Auth Details 中填写 GreptimeDB 的用户名和密码：

- User: `<username>`
- Password: *Your GreptimeDB password*

然后单击 Save & Test 按钮以测试连接。

## MySQL

单击 Add data source 按钮，然后选择 MySQL 作为类型。在 MySQL Connection 中填写以下信息：

- Host: `<host>:4002`
- Database: `<dbname>`
- User: `<username>`
- Password: *Your GreptimeDB password*
- Session timezone: `UTC`

然后单击 Save & Test 按钮以测试连接。
