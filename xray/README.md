# SINGBOX

> [!IMPORTANT]
> Атообновляемые списки для Xray ядра в формате .dat

<br> <!-- Пустая строка -->
 
> [**adaway**](https://4pda.to/forum/index.php?showtopic=275091&st=8000#Spoil-89665467-4)  (Список для блокировки рекламы от Schakal):
- [adaway.dat](https://github.com/AlgorithmArchitector/rulesets/blob/main/xray/adaway/adaway.dat)

<br> <!-- Пустая строка -->

> [**antifilter**](http://antifilter.download) (Списки заблокированных в РФ сайтов):

- [antifilter_allyouneed_ip.dat](https://github.com/AlgorithmArchitector/rulesets/blob/main/xray/antifilter/antifilter_allyouneed_ip.dat)
- [antifilter_community_ip.dat](https://github.com/AlgorithmArchitector/rulesets/blob/main/xray/antifilter/antifilter_community_ip.dat)
- [antifilter_community_domain.dat](https://github.com/AlgorithmArchitector/rulesets/blob/main/xray/antifilter/antifilter_community_domain.dat)

<br> <!-- Пустая строка -->

> [**torrents**](https://github.com/SM443/Pi-hole-Torrent-Blocklist) (Списки для блокировки известных торрент-трекеров и веб-сайтов):

- [torrents.dat](https://github.com/AlgorithmArchitector/rulesets/blob/main/xray/torrents/torrents.dat)


<br> <!-- Пустая строка -->

**Пример использования `.dat` списков:**

> **geosites:**
```
{
            "outboundTag": "BLOCK",
            "domain": [
                "ext:adaway.dat:adaway.lst",
                "ext:torrents.dat:torrent_trackers.lst",
                "ext:torrents.dat:torrent_websites.lst",
                "ext:antifilter_community_domain.dat:antifilter_community_domain.lst"
            ],
            "type": "field"
        }
```

> **geoip:**
```
{
            "outboundTag": "BLOCK",
            "ip": [
                "ext:antifilter_allyouneed_ip.dat:antifilter_allyouneed_ip",
                "ext:antifilter_community_ip.dat:antifilter_community_ip"
            ],
            "type": "field"
        }
```

