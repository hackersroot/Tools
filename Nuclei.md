# Nuclei Setup

$ go install -v github.com/projectdiscovery/nuclei/v2/cmd/nuclei@latest

$ sudo nuclei -update-templates

Usage:

$ nuclei -u http://testphp.vulnweb.com/ -t technologies/ngix-version.yaml

$ nuclei -u https://evil.com -t cves/ - evclude-templates cves/2020/

$ nuclei -u https://evil.com -t cves/ -etags xss

$ nuclei -u evil -t cves/ -etags sqli.rce

$ nuclei -l target_urls.txt -include-tags iot,misc,fuzz
