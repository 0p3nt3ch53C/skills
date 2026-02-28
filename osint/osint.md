# OSINT (Open Source Intelligence) Skill

## Description

This skill enables comprehensive Open Source Intelligence gathering and analysis. It provides structured methodologies for collecting, processing, and analyzing publicly available information about targets including individuals, organizations, domains, IP addresses, and digital assets.

## Triggers

- "osint on [target]"
- "investigate [target]"
- "gather intelligence on [target]"
- "research [person/company/domain]"
- "find information about [target]"
- "reconnaissance on [target]"

## Capabilities

### Person Investigation
- Social media footprint analysis
- Professional network mapping (LinkedIn, GitHub, etc.)
- Email address discovery and verification
- Username enumeration across platforms
- Public records and data breach exposure checks

### Organization Investigation
- Corporate structure and ownership
- Employee enumeration
- Technology stack identification
- Public filings and financial records
- News and media mentions
- Supplier and partner relationships

### Domain/Infrastructure Investigation
- WHOIS and DNS enumeration
- Subdomain discovery
- SSL/TLS certificate analysis
- Historical DNS records
- IP address geolocation and ASN mapping
- Web technology fingerprinting
- Exposed services and ports

### Digital Asset Investigation
- Cryptocurrency wallet analysis
- Code repository mining
- Document metadata extraction
- Image EXIF data analysis
- Cached and archived content retrieval

## Methodology

### Phase 1: Target Definition
1. Clearly define the target (person, organization, domain, IP, etc.)
2. Establish scope boundaries (what is in/out of scope)
3. Define objectives (what information is needed and why)
4. Document legal and ethical constraints

### Phase 2: Passive Reconnaissance
1. Search engine queries (Google dorks, Bing, DuckDuckGo)
2. Social media analysis
3. Public records and databases
4. WHOIS and DNS lookups
5. Certificate transparency logs
6. Archive.org and cached content
7. Data breach databases (ethical use only)

### Phase 3: Semi-Passive Reconnaissance
1. Website crawling and scraping
2. Metadata extraction from public documents
3. Technology stack identification
4. Job posting analysis for tech stack hints

### Phase 4: Analysis and Correlation
1. Cross-reference findings across sources
2. Build relationship maps
3. Timeline construction
4. Identify patterns and anomalies
5. Validate and verify critical findings

### Phase 5: Reporting
1. Executive summary
2. Detailed findings by category
3. Risk assessment (if applicable)
4. Recommendations
5. Source attribution and confidence levels

## Tools Reference

### Search Engines & Dorks
- Google (site:, filetype:, inurl:, intitle:, cache:)
- Bing, DuckDuckGo, Yandex
- Shodan, Censys, ZoomEye (internet-connected devices)

### Domain/IP Tools
- WHOIS lookup services
- DNSDumpster, SecurityTrails
- Sublist3r, Amass, Subfinder
- BuiltWith, Wappalyzer
- crt.sh (certificate transparency)

### Social Media / People
- Namechk, KnowEm (username search)
- Hunter.io, Phonebook.cz (email discovery)
- Pipl, That'sThem (people search)
- Social Searcher, Social Blade

### Code & Technical
- GitHub, GitLab, Bitbucket search
- Grep.app (code search)
- PublicWWW (source code search)
- Wayback Machine (archive.org)

### Visualization
- Maltego
- SpiderFoot
- Recon-ng
- theHarvester

## Output Format

```markdown
# OSINT Report: [TARGET]

## Executive Summary
[Brief overview of key findings]

## Target Information
- **Target Type:** [Person/Organization/Domain/IP]
- **Primary Identifier:** [Name/Domain/IP]
- **Investigation Date:** [Date]
- **Scope:** [What was investigated]

## Findings

### [Category 1]
| Finding | Source | Confidence | Notes |
|---------|--------|------------|-------|
| [Data]  | [URL]  | High/Med/Low | [Context] |

### [Category 2]
...

## Relationship Map
[Visual or textual representation of connections]

## Risk Assessment
[If applicable - exposure level, vulnerabilities identified]

## Recommendations
[Actionable next steps or security improvements]

## Sources
[List of all sources consulted with timestamps]

## Disclaimers
- All information gathered from publicly available sources
- Findings should be independently verified
- This report is for authorized use only
```

## Ethical Guidelines

1. **Legal Compliance**: Only gather publicly available information; never access private systems
2. **Authorization**: Ensure proper authorization before conducting OSINT on any target
3. **Privacy Respect**: Do not collect or store sensitive personal information unnecessarily
4. **No Social Engineering**: This skill is for passive/semi-passive collection only
5. **Data Handling**: Securely store and properly dispose of collected data
6. **Disclosure**: Report critical vulnerabilities through responsible disclosure channels

## Example Usage

### Example 1: Domain Investigation
```
User: "osint on example.com"

Response: Conducting OSINT investigation on example.com...

Phase 1: Target Definition
- Target: example.com
- Type: Domain/Organization
- Scope: Domain infrastructure, technology stack, exposed assets

Phase 2: Passive Reconnaissance
[Proceeds with WHOIS, DNS, subdomain enumeration, etc.]
```

### Example 2: Person Investigation
```
User: "investigate John Smith, CEO of Acme Corp"

Response: Conducting OSINT investigation...

Phase 1: Target Definition
- Target: John Smith
- Role: CEO, Acme Corp
- Scope: Professional presence, public statements, digital footprint

Phase 2: Passive Reconnaissance
[Proceeds with LinkedIn, news articles, public filings, etc.]
```

## Integration Notes

- This skill can be combined with security assessment skills
- Findings can feed into threat modeling workflows
- Supports both manual analysis and automated tool orchestration
- Results should be stored in secure, encrypted formats

## Version
- **Version:** 1.0.0
- **Last Updated:** 2026-02-27
- **Author:** 0p3nt3ch53C
- **License:** MIT
