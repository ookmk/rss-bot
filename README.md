# rss-bot
使用 heroku 部屬的 RSS 機器人。 使用代碼來自於 indes/flowerss-bot。

請將此代碼下載，並上傳到你自己的帳號，將您的配置添加到 config.yml。

將 config_sample.yml 重命名為 config.yml，然後添加您的配置。 如果您不知道其他配置的作用，請不要動它們。

![image](https://user-images.githubusercontent.com/67411136/128676810-c80a8e98-33f5-49e5-9ca2-2d84add6f563.png)

請使用 ClearDB MySQL (for heroku) 來保存 RSS 配置。 在config.yml中的mysql下添加。

示例： CLEARDB_DATABASE_URL

mysql://"mysql-user":"mysql-password"@"mysql-host"/mysql-database"

mysql-port 的默認端口號是 3306。

mysql:
  host: mysql-host
  port: 3306
  user: mysql-user
  password: mysql-password
  database: mysql-database


## heroku
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/makubex2010/rss-bot)
  
## 來源
- [indes](https://github.com/indes) for [flowerss-bot](https://github.com/indes/flowerss-bot)
