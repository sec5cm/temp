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
    - { name: 'π­π° [2.5] ι¦ζΈ― S01', type: ss, server: lgz.sub-nthu.com, port: 51003, cipher: aes-128-gcm, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true }
    - { name: 'π―π΅ [2.5] δΈδΊ¬ S01', type: ss, server: lgz.sub-nthu.com, port: 51002, cipher: aes-128-gcm, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true }
    - { name: 'πΉπΌ [2.5] ε°η£ S01', type: ss, server: lgz.sub-nthu.com, port: 51004, cipher: aes-128-gcm, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true }
    - { name: 'πΈπ¬ [2.5] ζζ΄² S01', type: ss, server: lgz.sub-nthu.com, port: 51001, cipher: aes-128-gcm, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true }
    - { name: 'πΊπΈ [2.5] ηΎε S01', type: ss, server: lgz.sub-nthu.com, port: 51000, cipher: aes-128-gcm, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true }
    - { name: 'π°π· [2.5] ι©ε½ S01', type: ss, server: lgz.sub-nthu.com, port: 51005, cipher: aes-128-gcm, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true }
    - { name: 'πΊπΈ ηΎε A01', type: trojan, server: ygzyd.sub-nthu.com, port: 35000, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: us-1.sub-nthu.com }
    - { name: 'πΊπΈ ηΎε B01', type: trojan, server: shlt.sub-nthu.com, port: 35000, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: us-1.sub-nthu.com }
    - { name: 'πΊπΈ ηΎε D01', type: trojan, server: cn2hn.sub-nthu.com, port: 35000, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: us-1.sub-nthu.com }
    - { name: 'π―π΅ ζ±δΊ¬ A01', type: trojan, server: ygzyd.sub-nthu.com, port: 35001, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: jp-1.sub-nthu.com }
    - { name: 'π―π΅ ζ±δΊ¬ B01', type: trojan, server: shlt.sub-nthu.com, port: 35001, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: jp-1.sub-nthu.com }
    - { name: 'π―π΅ ζ±δΊ¬ D01', type: trojan, server: cn2hn.sub-nthu.com, port: 35001, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: jp-1.sub-nthu.com }
    - { name: 'π­π° ι¦ζΈ― A01', type: trojan, server: ygzyd.sub-nthu.com, port: 35002, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: hk-1.sub-nthu.com }
    - { name: 'π­π° ι¦ζΈ― B01', type: trojan, server: shlt.sub-nthu.com, port: 35002, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: hk-1.sub-nthu.com }
    - { name: 'π­π° ι¦ζΈ― D01', type: trojan, server: cn2hn.sub-nthu.com, port: 35002, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: hk-1.sub-nthu.com }
    - { name: 'π­π° ι¦ζΈ― A02', type: trojan, server: ygzyd.sub-nthu.com, port: 35006, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: hk-0.sub-nthu.com }
    - { name: 'π­π° ι¦ζΈ― B02', type: trojan, server: shlt.sub-nthu.com, port: 35006, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: hk-0.sub-nthu.com }
    - { name: 'π­π° ι¦ζΈ― D02', type: trojan, server: cn2hn.sub-nthu.com, port: 35006, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: hk-0.sub-nthu.com }
    - { name: 'πΈπ¬ ζ°ε ε‘ A01', type: trojan, server: ygzyd.sub-nthu.com, port: 35003, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: sg-1.sub-nthu.com }
    - { name: 'πΈπ¬ ζ°ε ε‘ B01', type: trojan, server: shlt.sub-nthu.com, port: 35003, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: sg-1.sub-nthu.com }
    - { name: 'πΈπ¬ ζ°ε ε‘ D01', type: trojan, server: cn2hn.sub-nthu.com, port: 35003, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: sg-1.sub-nthu.com }
    - { name: 'πΉπΌ ε°η£ A01', type: trojan, server: ygzyd.sub-nthu.com, port: 35005, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: tw-1.sub-nthu.com }
    - { name: 'πΉπΌ ε°η£ B01', type: trojan, server: shlt.sub-nthu.com, port: 35005, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: tw-1.sub-nthu.com }
    - { name: 'πΉπΌ ε°η£ D01', type: trojan, server: cn2hn.sub-nthu.com, port: 35005, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: tw-1.sub-nthu.com }
    - { name: 'π°π· ι©ε½ A01', type: trojan, server: ygzyd.sub-nthu.com, port: 35007, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: kr-1.sub-nthu.com }
    - { name: 'π°π· ι©ε½ B01', type: trojan, server: shlt.sub-nthu.com, port: 35007, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: kr-1.sub-nthu.com }
    - { name: 'π°π· ι©ε½ D01', type: trojan, server: cn2hn.sub-nthu.com, port: 35007, password: bfa69659-348f-42f2-801a-6c850186aae3, udp: true, sni: kr-1.sub-nthu.com }
proxy-groups:
    - { name: πNTHU.CC, type: select, proxies: [πθͺειΈζ, 'π­π° [2.5] ι¦ζΈ― S01', 'π―π΅ [2.5] δΈδΊ¬ S01', 'πΉπΌ [2.5] ε°η£ S01', 'πΈπ¬ [2.5] ζζ΄² S01', 'πΊπΈ [2.5] ηΎε S01', 'π°π· [2.5] ι©ε½ S01', 'πΊπΈ ηΎε A01', 'πΊπΈ ηΎε B01', 'πΊπΈ ηΎε D01', 'π―π΅ ζ±δΊ¬ A01', 'π―π΅ ζ±δΊ¬ B01', 'π―π΅ ζ±δΊ¬ D01', 'π­π° ι¦ζΈ― A01', 'π­π° ι¦ζΈ― B01', 'π­π° ι¦ζΈ― D01', 'π­π° ι¦ζΈ― A02', 'π­π° ι¦ζΈ― B02', 'π­π° ι¦ζΈ― D02', 'πΈπ¬ ζ°ε ε‘ A01', 'πΈπ¬ ζ°ε ε‘ B01', 'πΈπ¬ ζ°ε ε‘ D01', 'πΉπΌ ε°η£ A01', 'πΉπΌ ε°η£ B01', 'πΉπΌ ε°η£ D01', 'π°π· ι©ε½ A01', 'π°π· ι©ε½ B01', 'π°π· ι©ε½ D01'] }
    - { name: πθͺειΈζ, type: load-balance, proxies: ['π­π° [2.5] ι¦ζΈ― S01', 'π―π΅ [2.5] δΈδΊ¬ S01', 'πΉπΌ [2.5] ε°η£ S01', 'πΈπ¬ [2.5] ζζ΄² S01', 'πΊπΈ [2.5] ηΎε S01', 'π°π· [2.5] ι©ε½ S01', 'πΊπΈ ηΎε A01', 'πΊπΈ ηΎε B01', 'πΊπΈ ηΎε D01', 'π―π΅ ζ±δΊ¬ A01', 'π―π΅ ζ±δΊ¬ B01', 'π―π΅ ζ±δΊ¬ D01', 'π­π° ι¦ζΈ― A01', 'π­π° ι¦ζΈ― B01', 'π­π° ι¦ζΈ― D01', 'π­π° ι¦ζΈ― A02', 'π­π° ι¦ζΈ― B02', 'π­π° ι¦ζΈ― D02', 'πΈπ¬ ζ°ε ε‘ A01', 'πΈπ¬ ζ°ε ε‘ B01', 'πΈπ¬ ζ°ε ε‘ D01', 'πΉπΌ ε°η£ A01', 'πΉπΌ ε°η£ B01', 'πΉπΌ ε°η£ D01', 'π°π· ι©ε½ A01', 'π°π· ι©ε½ B01', 'π°π· ι©ε½ D01'], url: 'http://www.msftconnecttest.com/connecttest.txt', interval: 300 }
    - { name: π²π΄ζΈ―ε°ε°ε, type: select, proxies: [DIRECT, πNTHU.CC, 'π­π° [2.5] ι¦ζΈ― S01', 'π―π΅ [2.5] δΈδΊ¬ S01', 'πΉπΌ [2.5] ε°η£ S01', 'πΈπ¬ [2.5] ζζ΄² S01', 'πΊπΈ [2.5] ηΎε S01', 'π°π· [2.5] ι©ε½ S01', 'πΊπΈ ηΎε A01', 'πΊπΈ ηΎε B01', 'πΊπΈ ηΎε D01', 'π―π΅ ζ±δΊ¬ A01', 'π―π΅ ζ±δΊ¬ B01', 'π―π΅ ζ±δΊ¬ D01', 'π­π° ι¦ζΈ― A01', 'π­π° ι¦ζΈ― B01', 'π­π° ι¦ζΈ― D01', 'π­π° ι¦ζΈ― A02', 'π­π° ι¦ζΈ― B02', 'π­π° ι¦ζΈ― D02', 'πΈπ¬ ζ°ε ε‘ A01', 'πΈπ¬ ζ°ε ε‘ B01', 'πΈπ¬ ζ°ε ε‘ D01', 'πΉπΌ ε°η£ A01', 'πΉπΌ ε°η£ B01', 'πΉπΌ ε°η£ D01', 'π°π· ι©ε½ A01', 'π°π· ι©ε½ B01', 'π°π· ι©ε½ D01'] }
    - { name: πΊδΈ²ζ΅εͺι«, type: select, proxies: [πNTHU.CC, 'π­π° [2.5] ι¦ζΈ― S01', 'π―π΅ [2.5] δΈδΊ¬ S01', 'πΉπΌ [2.5] ε°η£ S01', 'πΈπ¬ [2.5] ζζ΄² S01', 'πΊπΈ [2.5] ηΎε S01', 'π°π· [2.5] ι©ε½ S01', 'πΊπΈ ηΎε A01', 'πΊπΈ ηΎε B01', 'πΊπΈ ηΎε D01', 'π―π΅ ζ±δΊ¬ A01', 'π―π΅ ζ±δΊ¬ B01', 'π―π΅ ζ±δΊ¬ D01', 'π­π° ι¦ζΈ― A01', 'π­π° ι¦ζΈ― B01', 'π­π° ι¦ζΈ― D01', 'π­π° ι¦ζΈ― A02', 'π­π° ι¦ζΈ― B02', 'π­π° ι¦ζΈ― D02', 'πΈπ¬ ζ°ε ε‘ A01', 'πΈπ¬ ζ°ε ε‘ B01', 'πΈπ¬ ζ°ε ε‘ D01', 'πΉπΌ ε°η£ A01', 'πΉπΌ ε°η£ B01', 'πΉπΌ ε°η£ D01', 'π°π· ι©ε½ A01', 'π°π· ι©ε½ B01', 'π°π· ι©ε½ D01'] }
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
    - 'RULE-SET,StreamingSE,π²π΄ζΈ―ε°ε°ε'
    - 'RULE-SET,Streaming,πΊδΈ²ζ΅εͺι«'
    - 'RULE-SET,Global,πNTHU.CC'
    - 'RULE-SET,Scholar,DIRECT'
    - 'RULE-SET,TldNotCN,πNTHU.CC'
    - 'RULE-SET,China,DIRECT'
    - 'RULE-SET,Private,DIRECT'
    - 'RULE-SET,LanCIDR,DIRECT'
    - 'RULE-SET,ChinaIP,DIRECT'
    - 'MATCH,πNTHU.CC'
