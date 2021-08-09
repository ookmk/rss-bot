# rss-bot
RSS 機器人。 使用的代碼來自於 indes/flowerss-bot。

請將此代碼下載，並上傳到你自己的帳號，將您的配置添加到 config.yml。

將 config_sample.yml 重命名為 config.yml，然後添加您的配置。 如果您不知道其他配置的作用，請不要動它們。

配置说明：

配置项	含义	是否必填
bot_token	Telegram Bot Token	必填
telegraph_token	Telegraph Token, 用于转存原文到 Telegraph	可忽略（不转存原文到 Telegraph ）
preview_text	纯文字预览字数（不借助Telegraph）	可忽略（默认0, 0为禁用）
user_agent	User Agent	可忽略
disable_web_page_preview	是否禁用 web 页面预览	可忽略（默认 false, true 为禁用）
update_interval	RSS 源扫描间隔（分钟）	可忽略（默认 10）
error_threshold	源最大出错次数	可忽略（默认 100）
socks5	用于无法正常 Telegram API 的环境	可忽略（能正常连接上 Telegram API 服务器）
mysql	MySQL 数据库配置	可忽略（使用 SQLite ）
sqlite	SQLite 配置	可忽略（已配置mysql时，该项失效）
telegram.endpoint	自定义telegram bot api url	可忽略（使用默认api url）
allowed_users	允许使用bot的用户telegram id，	可忽略，为空时所有用户都能使用bot

使用 ClearDB MySQL (for heroku) 來保存 RSS 配置。 在config.yml中的mysql下添加。

示例： CLEARDB_DATABASE_URL

mysql://"mysql-user":"mysql-password"@"mysql-host"/mysql-database"

mysql-port 的默認端口號是 3306。

# 部署
大多數人會選擇 Heroku，所以我想你一定是這些人中的一員。

## heroku
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/makubex2010/rss-bot)
  
## 來源
- [indes](https://github.com/indes) for [flowerss-bot](https://github.com/indes/flowerss-bot)
