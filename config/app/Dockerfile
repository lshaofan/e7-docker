#
FROM liushaofan77/e7:v1
#FROM hyperf/hyperf:7.4-alpine-v3.14-swoole

WORKDIR /www/wwwroot/server/

# 生产阶段使用以下配置
#CMD sh -c "composer install -o && php /www/wwwroot/server/bin/hyperf.php && php /www/wwwroot/server/bin/hyperf.php start"
# 开发阶段使用以下配置，支持热更新
#CMD sh -c "composer install -o && php /www/wwwroot/server/bin/hyperf.php && php /www/wwwroot/server/bin/hyperf.php server:watch"
#开发环境下没有更新composer的包，可以使用以下配置
ENTRYPOINT ["php", "/www/wwwroot/server/bin/hyperf.php", "server:watch"]