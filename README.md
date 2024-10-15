# Что это? 

Этот репозиторий содержит автоматически обновляемые правила маршрутизации [**V2Ray**](https://github.com/v2fly/v2ray-core), основанные на данных о заблокированных доменах и адресах в России.

Распространяемые здесь файлы `geoip.dat` и `geosite.dat` могут использоваться в [V2Ray](https://github.com/v2fly/v2ray-core), [v2rayN](https://github.com/2dust/v2rayN), [Xray-core](https://github.com/XTLS/Xray-core), [mihomo](https://github.com/MetaCubeX/mihomo/tree/Meta), [hysteria](https://github.com/apernet/hysteria), [Trojan-Go](https://github.com/p4gefau1t/trojan-go), [leaf](https://github.com/eycorsican/leaf) и так далее.

Репозиторий обновляется каждые 6 часов.

## Какие категории содержатся в файлах

### geoip.dat

`geoip.dat` генерируется в репозитории [@runetfreedom/russia-blocked-geoip](https://github.com/runetfreedom/russia-blocked-geoip)

Основные категории:

- `ru-blocked` содержит `ipresolve.lst` и `subnet.lst` сервиса antifilter.download
- `ru-blocked-community` содержит `community.lst` сервиса community.antifilter.download

Для вашего удобства в файлы включены несколько дополнительных категорий (на основе ASN):

- `geoip:cloudflare`
- `geoip:cloudfront`
- `geoip:facebook`
- `geoip:fastly`
- `geoip:google`
- `geoip:netflix`
- `geoip:telegram`
- `geoip:twitter`
- `geoip:ddos-guard`
- `geoip:yandex`

### geosite.dat

`geosite.dat` генерируется в репозитории [@runetfreedom/russia-blocked-geosite](https://github.com/runetfreedom/russia-blocked-geosite)

Доступные категории:

- Все категории из [@v2fly/domain-list-community](https://github.com/v2fly/domain-list-community/tree/master/data). Включая: `google`, `discord`, `youtube`, `twitter`, `meta`, `openai` и так далее.
- `geosite:ru-blocked` - заблокированные в России домены (`antifilter-download-community` + `re:filter`)
- `geosite:ru-blocked-all` - **все известные** заблокированные в России домены (из всех источников сразу). Список содержит не менее 700 тысяч доменов, употреблять с осторожностью.
- `geosite:ru-available-only-inside` - Домены, доступные только внутри России
- `geosite:antifilter-download` - все домены из `antifilter.download` (почти 700 тысяч, употреблять с осторожностью)
- `geosite:antifilter-download-community` - все домены из `community.antifilter.download`
- `geosite:refilter` - все домены из `re:filter`
- `geosite:category-ads-all` - все рекламные домены
- `geosite:win-spy` - домены, используемые windows для слежки и сбора аналитики
- `geosite:win-update` - домены, используемые windows для обновлений
- `geosite:win-extra` - прочие домены, используемые windows

# Cкачать 

По ссылкам ниже всегда доступна последняя версия файлов.

- **geoip.dat**
    - [https://raw.githubusercontent.com/runetfreedom/russia-v2ray-rules-dat/release/geoip.dat](https://raw.githubusercontent.com/runetfreedom/russia-v2ray-rules-dat/release/geoip.dat)
- **geosite.dat**
    - [https://raw.githubusercontent.com/runetfreedom/russia-v2ray-rules-dat/release/geosite.dat](https://raw.githubusercontent.com/runetfreedom/russia-v2ray-rules-dat/release/geosite.dat)


## Благодарности

- [antifilter.download](https://antifilter.download/) - за предоставление данных о заблокированных доменах и комьюнити для их обновления
- [re:filter](https://github.com/1andrevich/Re-filter-lists) - за предоставление отфильтрованных данных о заблокированных доменах
- [@Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat) - за идею и основу этого проекта