# 4.1 Information Gathering
## 4.1.1 Conduct Search Engine Discovery Reconnaissance for Information Leakage

[OWASP Wiki link](https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/01-Information_Gathering/01-Conduct_Search_Engine_Discovery_Reconnaissance_for_Information_Leakage.html)

Use a search engine to search for potentially sensitive information

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
- [ ] Select the target page and search information from different search engines. How much do results are different? Give a short description of what search engines to use in different situations.
- [ ] Try searching with operators in search engines and see can you find something interesting. Write down any interesting findings.
	- site:target.url
	- inurl:phpinfo
	- intitle:"index of /"
	- filetype:pdf

- [ ] Try to combinate different operators to get a more precise search. Write down what combinations you came up with and what results they gave.
	- site:target.url intitle:"index of /" inurl:backups

### Cached Content
- [ ] Try to use cache:target.url and see if the page is any different. Write down your findings.

### Google Hacking/Dorking
- [ ] Browse through possible dorks and list the top 3 that you think are exposing critical information. Give a short explanation of why this information is critical.

## 4.1.2 Fingerprint Web Server
[OWASP Wiki link](https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/01-Information_Gathering/02-Fingerprint_Web_Server.html)

- [ ] Perform banner grabbing to at least 3 different targets. Write down your findings.
- [ ] Sending malformed requests to at least 3 different targets. Write down your findings.
- [ ] Extra mile: Write a script that can perform these two actions automatically when the target URL is provided.
- [ ] Try out [Netcraft](https://sitereport.netcraft.com/) on target and write down your findings.

## 4.1.3 Review Webserver Metafiles for Information Leakage
[OWASP Wiki link](https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/01-Information_Gathering/03-Review_Webserver_Metafiles_for_Information_Leakage.html)

- [ ] Find if the target page has robots.txt file and what interesting things it contains. Write down your findings.
- [ ] Use google to find different robots.txt files. Write down used google search terms and any interesting findings. 
- [ ] Find if the target page has sitemap.xml file and what interesting things it contains. Write down your findings.
- [ ] Use google to find different sitemap.xml files. Write down used google search terms and any interesting findings. 
- [ ] Extra mile: Write a script that takes sitemap.xml file and parses it to extract all the URLs and requests each one through a specified proxy (Burp).
- [ ] Use google to find different security.txt files. Write down used google search terms and any interesting findings.
- [ ] Use google to find different humans.txt files. Write down used google search terms and any interesting findings.
- [ ] Extra mile: Make list of all .well-known/ filenames for future use in fuzzing.
- [ ] Extra mile: Write a script that will check the target website for all .well-known/ files and store found values.

## 4.1.4 Enumerate Applications on Webserver
[OWASP Wiki link](https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/01-Information_Gathering/04-Enumerate_Applications_on_Webserver.html)

- [ ] Write down possible other versions of URLs you would try in order to discover other pages. Base Url: http://www.example.com/alpha. What google search would help to discover pages in this case?
- [ ] Write down possible other versions of URLs you would try in order to discover other pages. Base Url: http://www.vpn.example.com/. What google search would help to discover pages in this case?
- [ ] Write down typical non-standard ports that should be checked first.
- [ ] Extra mile: Use Nessus to scan the target for all ports
- [ ] Perform zone transfer for zonetransfer.me domain.  Write down successful commands and findings.
- [ ] Use reverse-IP services with the target IP address to discover new information. Write down your findings.

## 4.1.5 Review Webpage Content for Information Leakage
[OWASP Wiki link] (https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/01-Information_Gathering/05-Review_Webpage_Content_for_Information_Leakage.html)

- [] Use Burp suite to find HTML comments. Write down if anything interesting was found.
- [] What META tags are used on the target page and do they give out any information? Write down your findings.
- [] Look through target javascript files and terminate if the target uses source map files. Write down if anything interesting was found.

## 4.1.6 Identify Application Entry Points

## 4.1.7 Map Execution Paths Through Application

## 4.1.8 Fingerprint Web Application Framework

## 4.1.9 Fingerprint Web Application
[OWASP Wiki link] (https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/01-Information_Gathering/09-Fingerprint_Web_Application.html)

Merged with the previous one.

## 4.1.10 Map Application Architecture