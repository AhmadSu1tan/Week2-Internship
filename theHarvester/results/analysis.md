# theHarvester Practical Analysis

## 1. Objective
Demonstrate passive OSINT collection using theHarvester.

## 2. Environment
- Operating System: Kali Linux
- Tool: theHarvester 4.11.1
- Data Source: CRT.sh
- Target: example.com
- Collection Limit: 10

## 3. Command Executed
theHarvester -d example.com -l 10 -b crtsh -f example-domain-demo

## 4. Results
- Hostnames discovered: 1
- IP addresses discovered: 0
- Email addresses discovered: 0
- People identified: 0

### Hostname Returned
- emudhra-lab.example.com

## 5. Generated Evidence
- example-domain-demo.json
- example-domain-demo.xml

## 6. Analysis
The tool successfully queried the CRT.sh certificate-transparency
source and returned one hostname.

No IP addresses, email addresses, or people were identified.
The results demonstrate that passive OSINT findings depend on
the selected data source and the available public records.

## 7. Limitations
This was a controlled demonstration using example.com.
It was not a full assessment of a real organization.
No active scanning, exploitation, or vulnerability testing
was performed.

## 8. Conclusion
TheHarvester was successfully installed and executed.
The JSON and XML reports were generated and preserved
for evidence and further analysis.
