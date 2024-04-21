# Burp-AutoDropHosts

This repository contains black lists for Burp Suite's Proxy Action Rules extension. It can be used to block ads, tracking sites, malware sites, etc.

When testing web applications on the Internet, you may encounter a huge number of unnecessary requests to sites to track metrics performed by the web application on our part. We can get rid of this behavior using a bunch of **Include in scope** and **Drop all out-of-scope requests** settings. But they force us to create clear white lists of addresses, which is not always convenient.

Unfortunately, Burp Suite does not support blacklists for unwanted sites, although [requests to developers were made back in 2018](https://forum.portswigger.net/thread/suite-wide-level-traffic-blacklist-90c8072a), but the idea never progressed. But to solve this problem you can use the **Proxy Action Rules** plugin.

The idea here is to use [Burp Suite's Proxy Action Rules plugin](https://portswigger.net/bappstore/01376d8325c846b988730e9417016039) and configure **AutoDrop Hosts** to drop all unwated requests. This will be our black list for Burp Suite.

## Structure

- trackers-all.txt - every possible tracking site
- trackers-ru.txt - russian tracking sites 

## Contribute

I'll appreciate for contributing in this project by adding more unwated websites in lists to cover them all (if possible).
