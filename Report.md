##A  Supplementary Report

One of the first things I discovered during the research for this project was how difficult it is to retrieve structured information about Chinese-language books if you are outside of the nation and don’t have institutional access or a China-issued phone number. Most digital infrastructure for books in China, state-backed or otherwise, is closed off. Major sites like Douban, Dangdang, and Bookschina implement either restrict crawlers or have strict rate-limiting ( especially for foreign IPs, the system will block even a few manual queries with a login wall if you’re on a foreign IP address). Nearly all platforms now require mobile phone verification tied to a Chinese ID. This means that researchers, students, developers, or bookstore workers based abroad are pretty much locked out of these resources.

I looked through many tutorials in my seach for workarounds, but most tutorials for these resources were outdated and unusuable. However they are still actively being circulated and therefore misleading. For example, a widely shared, beginner-friendly, and very detailed tutorial on scraping Dangdang called [爬取当当网图书信息并进行数据清洗](https://cloud.tencent.com/developer/article/1756147) with BeautifulSoup walks through from the steps to set up a python environment to the basics of web scraping and data cleaning very clearly. However, it does not take into account rate-limits nowadays or what happens or how to tell when the site blocks you, so a good portion of the tutorial is unusable. 
Another tutorial called[python学习之使用selenium爬取豆瓣图书信息](https://blog.csdn.net/m0_58050808/article/details/136995993) claimed to show how to scrape Douban with Selenium was behind a forum paywall and failed to acknowledge Douban’s strict login wall and anti-scraping mechanisms. 

At the same time, I explored platforms more accessible from the US. Zotero, which queries WorldCat and other catalogs, was able to return about 200 matches out of 700 ISBNs. ISBNdb, a paid API service, returned around 520. Sometimes these sources don't have a comprehensive or clean metadata set for Chinese-language titles. Some only returned pinyin instead of Chinese characters. Others were missing descriptions, publishers, or page counts. There is a need for resources that compare the various sources of publication metadata for the publications outside the English speaking world in terms of their coverage, accuracy, or completeness. 

This project is intended for anyone who might help with inventory at Accent Sisters in the future, and also a wider group of people like researchers, students, and digital humanists who are trying to retrieve and clean Chinese-language book data from either easily accessible or difficult sources. I wanted this workflow to show both what methods are currently working and the dead ends. 







