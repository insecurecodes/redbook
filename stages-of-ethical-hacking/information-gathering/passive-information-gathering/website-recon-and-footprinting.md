# Website Recon & Footprinting



### Things to look for

* IP addresses
* Directories hidden from search engines
* Names
* Email addresses
* Phone Numbers
* Physical Addresses
* Web technologies being used

#### Resolve website hostname

```bash
host www.google.com
```

#### Robots.txt

```bash
curl -L google.com/robots.txt
```

#### sitemaps.xml

```bash
curl -L google.com/sitemap.xml
curl -L google.com/sitemaps.xml
```

#### Browser plugins

They will help identifying the technologies sites are using.

* [Wappalyzer](https://chrome.google.com/webstore/detail/wappalyzer-technology-pro/gppongmhjkpfnbhagpmjfkannfbllamg)
* [BuiltWith](https://chrome.google.com/webstore/detail/builtwith-technology-prof/dapjbgnjinbpoindlpdmhochffioedbn/related?hl=en)

#### WhatWeb

WhatWeb identifies websites. Its goal is to answer the question, "What is that Website?". WhatWeb recognises web technologies including content management systems (CMS), blogging platforms, statistic/analytics packages, JavaScript libraries, web servers, and embedded devices. WhatWeb has over 1800 plugins, each to recognise something different. WhatWeb also identifies version numbers, email addresses, account IDs, web framework modules, SQL errors, and more.

```
whatweb reddit.com

<http://reddit.com> [301 Moved Permanently] Country[UNITED STATES][US], HTTPServer[snooserv], IP[151.101.65.140], RedirectLocation[<https://www.reddit.com/>], UncommonHeaders[retry-after,x-served-by,x-cache-hits,x-timer], Via-Proxy[1.1 varnish]
<https://www.reddit.com/> [200 OK] Cookies[edgebucket,eu_cookie_v2,loid,rabt,rseor3,session_tracker,token], Country[UNITED STATES][US], Email[banner@2x.png,snoo-home@2x.png], Frame, HTML5, HTTPServer[snooserv], HttpOnly[token], IP[151.101.37.140], Open-Graph-Protocol[website], Script[text/javascript], Strict-Transport-Security[max-age=15552000; includeSubDomains; preload], Title[reddit: the front page of the internet], UncommonHeaders[fastly-restarts,x-served-by,x-cache-hits,x-timer], Via-Proxy[1.1 varnish], X-Frame-Options[SAMEORIGIN]
```

#### HTTrack

HTTrack is a free (GPL, libre/free software) and easy-to-use offline browser utility.

It allows you to download a World Wide Web site from the Internet to a local directory, building recursively all directories, getting HTML, images, and other files from the server to your computer. HTTrack arranges the original site's relative link-structure. Simply open a page of the "mirrored" website in your browser, and you can browse the site from link to link, as if you were viewing it online. HTTrack can also update an existing mirrored site, and resume interrupted downloads. HTTrack is fully configurable, and has an integrated help system.



<figure><img src="../../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>



```
Mirroring operation complete.
Click Exit to quit WebHTTrack.
See log file(s) if necessary to ensure that everything is OK.

Thanks for using WebHTTrack!

Path : /home/rtm/websites/test website

    Browse Mirrored Website
    View log files
```
