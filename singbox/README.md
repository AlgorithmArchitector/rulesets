# SINGBOX

> [!IMPORTANT]
> Атообновляемые списки для Sing-box с ядром выше 1.8.0

<br> <!-- Пустая строка -->
 
> [**adaway**](https://4pda.to/forum/index.php?showtopic=275091&st=8000#Spoil-89665467-4)  (Список для блокировки рекламы от Schakal):
- [ruleset-domain-adaway.srs](https://github.com/AlgorithmArchitector/rulesets/raw/main/singbox/adaway/ruleset-domain-adaway.srs)

<br> <!-- Пустая строка -->

> [**antifilter**](http://antifilter.download) (Списки заблокированных в РФ сайтов):

- [ruleset-domain-antifilter_community_domain.srs](https://github.com/AlgorithmArchitector/rulesets/raw/main/singbox/antifilter/ruleset-domain-antifilter_community_domain.srs)
- [ruleset-ip-antifilter_community_ip.srs](https://github.com/AlgorithmArchitector/rulesets/raw/main/singbox/antifilter/ruleset-ip-antifilter_community_ip.srs)
- [ruleset-ip-antifilter_allyouneed.srs](https://github.com/AlgorithmArchitector/rulesets/raw/main/singbox/antifilter/ruleset-ip-antifilter_allyouneed.srs)

<br> <!-- Пустая строка -->

> [**torrents**](https://github.com/SM443/Pi-hole-Torrent-Blocklist) (Списки для блокировки известных торрент-трекеров и веб-сайтов):

- [ruleset-domain-torrent_trackers.srs](https://github.com/AlgorithmArchitector/rulesets/raw/main/singbox/torrents/ruleset-domain-torrent_trackers.srs)
- [ruleset-domain-torrent_websites.srs](https://github.com/AlgorithmArchitector/rulesets/raw/main/singbox/torrents/ruleset-domain-torrent_websites.srs)

<br> <!-- Пустая строка -->

**Пример использования `.srs` списка:**

```
{
  "tag": "torrent_websites",
  "type": "remote",
  "format": "binary",
  "url": "https://github.com/AlgorithmArchitector/rulesets/raw/main/singbox/adaway/ruleset-domain-adaway.srs",
  "download_detour": "direct",
  "update_interval": "168h0m0s"
}
```
