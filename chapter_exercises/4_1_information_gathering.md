# 4.1 Information Gathering
## 4.1.1 Conduct Search Engine Discovery Reconnaissance for Information Leakage

[OWASP Wiki link](https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/01-Information_Gathering/01-Conduct_Search_Engine_Discovery_Reconnaissance_for_Information_Leakage.html)

Use a search engines to search for potentially sensitive information

Search Engines:
- [Baidu](https://www.baidu.com/)
- [Bing](https://www.bing.com/) > [Search syntax](http://help.bing.microsoft.com/#apex/18/en-US/10001/-1)
- [DuckDuckGo](https://duckduckgo.com/) > [Search syntax](https://help.duckduckgo.com/duckduckgo-help-pages/results/syntax/)
- [Google](https://www.google.com/) > [Search syntax](https://support.google.com/websearch/answer/2466433)
- [Archive.org](https://archive.org/web/)
- [Startpage](https://www.startpage.com/) > [Search syntax](https://support.startpage.com/index.php?/Knowledgebase/Article/View/989/0/advanced-search-which-search-operators-are-supported-by-startpagecom)
- [Binsearch.info](https://binsearch.info/)
- [Commoncrawl](https://commoncrawl.org/)
- [Shodan](https://www.shodan.io/)


### Search Engines & Operators
- [ ] Select target page and search information from different search engines. How much does are results different? Give a short description of what search engines to use in different situations.
- [ ] Try searching with operators in search engines and see can you find something intresting. Write down any intresting findings.
	- site:target.url
	- inurl:phpinfo
	- intitle:"index of /"
	- filetype:pdf

- [ ] Try to combinate different operators to get more precise search. Write down what combinations you came up with and what results they gave.
	- site:target.url intitle:"index of /" inurl:backups

### Cached Content
- [ ] Try to use cache:target.url and see if page is any different. Write down your findings.

### Google Hacking/Dorking
- [ ] Browse through possible dorks and list the top 3 that you think are exposing critical information. Give a short explanation of why this information is critical.

## 4.1.2 Fingerprint Web Server
- [ ] Perform banner grabbing to at least 3 different targets. Write down your findings.
- [ ] Sending malformed requests to at least 3 different targets. Write down your findings.
- [ ] Extra mile: Write a script that can perform these two actions automatically when the target URL is provided.
- [ ] Try out [Netcraft](https://sitereport.netcraft.com/) on target and write down your findings.

## 4.1.3 Review Webserver Metafiles for Information Leakage

## 4.1.4 Enumerate Applications on Webserver

## 4.1.5 Review Webpage Content for Information Leakage

## 4.1.6 Identify Application Entry Points

## 4.1.7 Map Execution Paths Through Application

## 4.1.8 Fingerprint Web Application Framework

## 4.1.9 Fingerprint Web Application

## 4.1.10 Map Application Architecture
