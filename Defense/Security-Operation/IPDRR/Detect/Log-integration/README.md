## Process



## Type
 ```mermaid
graph TD;
    log-->security;
    log-->business;
    log-->CMDB;
    
    CMDB-->assets;
    CMDB-->vuls;
    
    assets-->domain;
    assets-->IP;
    assets-->version/software;
    assets-->acl;
    
    business-->web-access;
    business-->audit;
    audit-->apigw;
    audit-->vpn;
    
    security-->network;
    security-->host;
    security-->application;
    
    host-->alarms;
    host-->rt-access;
    host-->history/cmds;
    
    
    network-->NDR;
    network-->NIPS;
    network-->honeypot;
    
    application-->WAF;
    application-->RASP;
    application-->fingerprint;
    
```


