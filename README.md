mixed-port: 7890
allow-lan: false
mode: rule
log-level: info
ipv6: true
external-controller: '127.0.0.1:9090'
experimental:
    ignore-resolve-fail: true
dns:
    enable: true
    ipv6: false
    default-nameserver: [223.5.5.5, 119.29.29.29]
    enhanced-mode: redir-host
    fake-ip-range: 198.18.0.1/16
    use-hosts: true
    nameserver: ['https://doh.pub/dns-query', 'https://dns.alidns.com/dns-query']
    fallback: ['tls://1.0.0.1:853', 'https://cloudflare-dns.com/dns-query', 'https://dns.google/dns-query']
    fallback-filter: { geoip: true, ipcidr: [240.0.0.0/4, 0.0.0.0/32] }
proxies:
    - { name: '🇭🇰 [2.5] 香港 S01', type: ss, server: lgz.sub-nthu.com, port: 51003, cipher: aes-128-gcm, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true }
    - { name: '🇯🇵 [2.5] 东京 S01', type: ss, server: lgz.sub-nthu.com, port: 51002, cipher: aes-128-gcm, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true }
    - { name: '🇹🇼 [2.5] 台灣 S01', type: ss, server: lgz.sub-nthu.com, port: 51004, cipher: aes-128-gcm, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true }
    - { name: '🇸🇬 [2.5] 星洲 S01', type: ss, server: lgz.sub-nthu.com, port: 51001, cipher: aes-128-gcm, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true }
    - { name: '🇺🇸 [2.5] 美國 S01', type: ss, server: lgz.sub-nthu.com, port: 51000, cipher: aes-128-gcm, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true }
    - { name: '🇰🇷 [2.5] 韩国 S01', type: ss, server: lgz.sub-nthu.com, port: 51005, cipher: aes-128-gcm, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true }
    - { name: '🇺🇸 美國 A01', type: trojan, server: ygzyd.sub-nthu.com, port: 35000, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: us-1.sub-nthu.com }
    - { name: '🇺🇸 美國 B01', type: trojan, server: shlt.sub-nthu.com, port: 35000, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: us-1.sub-nthu.com }
    - { name: '🇺🇸 美國 D01', type: trojan, server: cn2hn.sub-nthu.com, port: 35000, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: us-1.sub-nthu.com }
    - { name: '🇯🇵 東京 A01', type: trojan, server: ygzyd.sub-nthu.com, port: 35001, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: jp-1.sub-nthu.com }
    - { name: '🇯🇵 東京 B01', type: trojan, server: shlt.sub-nthu.com, port: 35001, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: jp-1.sub-nthu.com }
    - { name: '🇯🇵 東京 D01', type: trojan, server: cn2hn.sub-nthu.com, port: 35001, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: jp-1.sub-nthu.com }
    - { name: '🇭🇰 香港 A01', type: trojan, server: ygzyd.sub-nthu.com, port: 35002, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: hk-1.sub-nthu.com }
    - { name: '🇭🇰 香港 B01', type: trojan, server: shlt.sub-nthu.com, port: 35002, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: hk-1.sub-nthu.com }
    - { name: '🇭🇰 香港 D01', type: trojan, server: cn2hn.sub-nthu.com, port: 35002, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: hk-1.sub-nthu.com }
    - { name: '🇭🇰 香港 A02', type: trojan, server: ygzyd.sub-nthu.com, port: 35006, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: hk-0.sub-nthu.com }
    - { name: '🇭🇰 香港 B02', type: trojan, server: shlt.sub-nthu.com, port: 35006, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: hk-0.sub-nthu.com }
    - { name: '🇭🇰 香港 D02', type: trojan, server: cn2hn.sub-nthu.com, port: 35006, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: hk-0.sub-nthu.com }
    - { name: '🇸🇬 新加坡 A01', type: trojan, server: ygzyd.sub-nthu.com, port: 35003, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: sg-1.sub-nthu.com }
    - { name: '🇸🇬 新加坡 B01', type: trojan, server: shlt.sub-nthu.com, port: 35003, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: sg-1.sub-nthu.com }
    - { name: '🇸🇬 新加坡 D01', type: trojan, server: cn2hn.sub-nthu.com, port: 35003, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: sg-1.sub-nthu.com }
    - { name: '🇹🇼 台灣 A01', type: trojan, server: ygzyd.sub-nthu.com, port: 35005, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: tw-1.sub-nthu.com }
    - { name: '🇹🇼 台灣 B01', type: trojan, server: shlt.sub-nthu.com, port: 35005, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: tw-1.sub-nthu.com }
    - { name: '🇹🇼 台灣 D01', type: trojan, server: cn2hn.sub-nthu.com, port: 35005, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: tw-1.sub-nthu.com }
    - { name: '🇰🇷 韩国 A01', type: trojan, server: ygzyd.sub-nthu.com, port: 35007, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: kr-1.sub-nthu.com }
    - { name: '🇰🇷 韩国 B01', type: trojan, server: shlt.sub-nthu.com, port: 35007, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: kr-1.sub-nthu.com }
    - { name: '🇰🇷 韩国 D01', type: trojan, server: cn2hn.sub-nthu.com, port: 35007, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: kr-1.sub-nthu.com }
proxy-groups:
    - { name: 🚀NTHU.CC, type: select, proxies: [🏆自動選擇, '🇭🇰 [2.5] 香港 S01', '🇯🇵 [2.5] 东京 S01', '🇹🇼 [2.5] 台灣 S01', '🇸🇬 [2.5] 星洲 S01', '🇺🇸 [2.5] 美國 S01', '🇰🇷 [2.5] 韩国 S01', '🇺🇸 美國 A01', '🇺🇸 美國 B01', '🇺🇸 美國 D01', '🇯🇵 東京 A01', '🇯🇵 東京 B01', '🇯🇵 東京 D01', '🇭🇰 香港 A01', '🇭🇰 香港 B01', '🇭🇰 香港 D01', '🇭🇰 香港 A02', '🇭🇰 香港 B02', '🇭🇰 香港 D02', '🇸🇬 新加坡 A01', '🇸🇬 新加坡 B01', '🇸🇬 新加坡 D01', '🇹🇼 台灣 A01', '🇹🇼 台灣 B01', '🇹🇼 台灣 D01', '🇰🇷 韩国 A01', '🇰🇷 韩国 B01', '🇰🇷 韩国 D01'] }
    - { name: 🏆自動選擇, type: load-balance, proxies: ['🇭🇰 [2.5] 香港 S01', '🇯🇵 [2.5] 东京 S01', '🇹🇼 [2.5] 台灣 S01', '🇸🇬 [2.5] 星洲 S01', '🇺🇸 [2.5] 美國 S01', '🇰🇷 [2.5] 韩国 S01', '🇺🇸 美國 A01', '🇺🇸 美國 B01', '🇺🇸 美國 D01', '🇯🇵 東京 A01', '🇯🇵 東京 B01', '🇯🇵 東京 D01', '🇭🇰 香港 A01', '🇭🇰 香港 B01', '🇭🇰 香港 D01', '🇭🇰 香港 A02', '🇭🇰 香港 B02', '🇭🇰 香港 D02', '🇸🇬 新加坡 A01', '🇸🇬 新加坡 B01', '🇸🇬 新加坡 D01', '🇹🇼 台灣 A01', '🇹🇼 台灣 B01', '🇹🇼 台灣 D01', '🇰🇷 韩国 A01', '🇰🇷 韩国 B01', '🇰🇷 韩国 D01'], url: 'http://www.msftconnecttest.com/connecttest.txt', interval: 300 }
    - { name: 🇲🇴港台專區, type: select, proxies: [DIRECT, 🚀NTHU.CC, '🇭🇰 [2.5] 香港 S01', '🇯🇵 [2.5] 东京 S01', '🇹🇼 [2.5] 台灣 S01', '🇸🇬 [2.5] 星洲 S01', '🇺🇸 [2.5] 美國 S01', '🇰🇷 [2.5] 韩国 S01', '🇺🇸 美國 A01', '🇺🇸 美國 B01', '🇺🇸 美國 D01', '🇯🇵 東京 A01', '🇯🇵 東京 B01', '🇯🇵 東京 D01', '🇭🇰 香港 A01', '🇭🇰 香港 B01', '🇭🇰 香港 D01', '🇭🇰 香港 A02', '🇭🇰 香港 B02', '🇭🇰 香港 D02', '🇸🇬 新加坡 A01', '🇸🇬 新加坡 B01', '🇸🇬 新加坡 D01', '🇹🇼 台灣 A01', '🇹🇼 台灣 B01', '🇹🇼 台灣 D01', '🇰🇷 韩国 A01', '🇰🇷 韩国 B01', '🇰🇷 韩国 D01'] }
    - { name: 📺串流媒體, type: select, proxies: [🚀NTHU.CC, '🇭🇰 [2.5] 香港 S01', '🇯🇵 [2.5] 东京 S01', '🇹🇼 [2.5] 台灣 S01', '🇸🇬 [2.5] 星洲 S01', '🇺🇸 [2.5] 美國 S01', '🇰🇷 [2.5] 韩国 S01', '🇺🇸 美國 A01', '🇺🇸 美國 B01', '🇺🇸 美國 D01', '🇯🇵 東京 A01', '🇯🇵 東京 B01', '🇯🇵 東京 D01', '🇭🇰 香港 A01', '🇭🇰 香港 B01', '🇭🇰 香港 D01', '🇭🇰 香港 A02', '🇭🇰 香港 B02', '🇭🇰 香港 D02', '🇸🇬 新加坡 A01', '🇸🇬 新加坡 B01', '🇸🇬 新加坡 D01', '🇹🇼 台灣 A01', '🇹🇼 台灣 B01', '🇹🇼 台灣 D01', '🇰🇷 韩国 A01', '🇰🇷 韩国 B01', '🇰🇷 韩国 D01'] }
rule-providers:
    StreamingSE: { type: http, behavior: classical, path: ./RuleSet/StreamingMedia/StreamingSE.yaml, url: 'https://nthu.cc/Clash/RuleSet/StreamingMedia/StreamingSE.yaml', interval: 86400 }
    Streaming: { type: http, behavior: classical, path: ./RuleSet/StreamingMedia/Streaming.yaml, url: 'https://nthu.cc/Clash/RuleSet/StreamingMedia/Streaming.yaml', interval: 86400 }
    Scholar: { type: http, behavior: classical, path: ./RuleSet/Extra/Scholar.yaml, url: 'https://nthu.cc/Clash/RuleSet/Extra/Scholar.yaml', interval: 86400 }
    PayPal: { type: http, behavior: classical, path: ./RuleSet/Extra/Paypal.yaml, url: 'https://nthu.cc/Clash/RuleSet/Extra/PayPal.yaml', interval: 86400 }
    Global: { type: http, behavior: classical, path: ./RuleSet/Global.yaml, url: 'https://nthu.cc/Clash/RuleSet/Global.yaml', interval: 86400 }
    China: { type: http, behavior: classical, path: ./RuleSet/China.yaml, url: 'https://nthu.cc/Clash/RuleSet/China.yaml', interval: 86400 }
    ChinaIP: { type: http, behavior: ipcidr, path: ./RuleSet/Extra/ChinaIP.yaml, url: 'https://nthu.cc/Clash/RuleSet/Extra/ChinaIP.yaml', interval: 86400 }
    Private: { type: http, behavior: domain, path: ./RuleSet/private.yaml, url: 'https://nthu.cc/Clash/RuleSet/private.txt', interval: 86400 }
    TldNotCN: { type: http, behavior: domain, path: ./RuleSet/tld-not-cn.yaml, url: 'https://nthu.cc/Clash/RuleSet/tld-not-cn.txt', interval: 86400 }
    LanCIDR: { type: http, behavior: ipcidr, path: ./RuleSet/lancidr.yaml, url: 'https://nthu.cc/Clash/RuleSet/lancidr.txt', interval: 86400 }
rules:
    - 'DOMAIN,*.sub-nthu.com,DIRECT'
    - 'DOMAIN-SUFFIX,scdn.co,DIRECT'
    - 'DOMAIN-SUFFIX,edu.tw,DIRECT'
    - 'RULE-SET,PayPal,DIRECT'
    - 'RULE-SET,StreamingSE,🇲🇴港台專區'
    - 'RULE-SET,Streaming,📺串流媒體'
    - 'RULE-SET,Global,🚀NTHU.CC'
    - 'RULE-SET,Scholar,DIRECT'
    - 'RULE-SET,TldNotCN,🚀NTHU.CC'
    - 'RULE-SET,China,DIRECT'
    - 'RULE-SET,Private,DIRECT'
    - 'RULE-SET,LanCIDR,DIRECT'
    - 'RULE-SET,ChinaIP,DIRECT'
    - 'MATCH,🚀NTHU.CC'
