# LynkCo

LynkCo每日自动签到

## 配置说明

### Surge

安装模块

```ini
https://github.com/uyoungco/ios_rule_script/master/script/lynkco/lynkco_signin.sgmodule
```

## 获取Cookie

LynkCo APP - 我的 - 右上角签到

## 多账户

目前无法在单台iPhone/iPad设备上实现多账户执行每日签到。

多账户更多的作用是在多设备的情况下，将Cookies和坐标同步至青龙面板，由青龙面板执行多账户作业。

## 脚本变量

根据下表配置magic.json文件的内容

| 名称                          | 类型 | 说明                                   |
| ----------------------------- | ---- | -------------------------------------- |
| dingdongmaicai_checkin_cookie | Json | 多账户叮咚买菜Cookies                  |
| dingdongmaicai_checkin_body   | Json | 多账户叮咚买菜Body                     |
| dingdongmaicai_sync_qinglong  | Bool | 是否将获取的Cookie和Body同步至青龙面板 |

部分属性示例

```json
{
 "dingdongmaicai_checkin_cookie": {
   "magic_session": true,
   "user_id1": "cookie_1",
   "user_id2": "cookie_2"
 },
 "dingdongmaicai_checkin_body": {
   "magic_session": true,
   "user_id1": "body_1",
   "user_id2": "body_2"
 }
}
```
