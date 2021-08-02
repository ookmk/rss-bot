# rss-bot
RSS 機器人。 使用 indes/flowerss-bot。

請將此 repo 模板化，將其設為私有，並將您的變量添加到 config.yml。

將 config_sample.yml 重命名為 config.yml，然後添加變量。 如果您不知道變量的含義，請不要管它們。

如果您想了解有關變量的更多詳細信息，請參閱 reaitten/flowerss-bot。

使用 ClearDB MySQL (for heroku) 來保存 RSS 配置。 在config.yml中的mysql下添加。

示例：變量 CLEARDB_DATABASE_URL

mysql://"mysql-user":<mysql-password>@"mysql-host"/}mysql-database"

mysql-port 的默認端口號是 3306。

# 部署
大多數人會選擇 Heroku，所以我想你一定是這些人中的一員。

## heroku
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/makubex2010/rss-bot)
  
## 來源
- [indes](https://github.com/indes) for [flowerss-bot](https://github.com/indes/flowerss-bot)
