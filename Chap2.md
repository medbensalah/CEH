## Footprinting and reconaissance

_____________________________________

### Footprinting
Gathering data about the target.\
1st step of attacking.\
Planning the kill chain comes after footprinting.
  - Uncover vulnerabilities.
  - Collecting info (including infra)
    - **Organisational information:**
      - Employees data.
      - Smishing.
      - Vishing.
      - Physical addresses.
      - 3ed party data (Solarwinds).
      - Web links / techs.
      - Docs.
    - **Network information:**
      - IPs.
      - DNS records.
      - Exposed infrastructure / Topology.
      - Misconfiguration.
    - **System information:**
      - Emails.
      - Credentials.
      - Tokens.
      - Keys (Config files).

**Passive footprinting:**  No direct interaction with the target.
  - Social media.
  - Search engine.
  - Deep / Dark web.
  - Error Pages.
  - Groups / forums.
  - Social engineering.
  - Archive.org.
  - Websites:
    - contact.
    - hidden files.
    - IP addresses.
    - info about technologies and infrastructure.
    - TLS certificate.
  - Hard to detect (no logs).
  - Can be detected by honeypot.

**Active footprintng:** 
  - Querying public servers.
  - Searching particular files.
  - Downloading from the official company channels (dear buster / foca).
  - Extracting website links.
  - Gathering word lists.
  - Harvesting email lists.
  - More likely to be detected.

**Social engineering**

### Objectives:
  - Reduce Focus (for attackers).
  - Identify potential vulnerabilities.
  - Creating a network map.

### Threats:
  - SE.
  - information disclosure.
  - Business / corporate Loss

### Methodology
  - Social media.
  - Different tools depending on the skill level.
  - Public resources.
  - Payed resources.

### Techniques:
  - Search engines (Google Dorks).
    - cache.
    - search for particular data / file type ... .
  - Reverse image search.
  - Shodan
    -  Has external network sensors.\
    -  An IoT search enginr/\
    -  CVEs (ex : 202144228)\
    -  defenders know the attack surface\
    -  used for controlling accessible deices.
  - Video searchs
  - TLDs
    - Find amm domains belonging to an organization.
    - Whois.
    - Sublister.
    - Netcraft.
    - Especially against test services.
  - Social networks
    - Email addresses
    - Phone numbers.
    - Ex: 
      - The harvester.
  - Websites
    - Localiser
    - Burp suit
  - DBs
    - Whois
  - DNS reports
    - When aliasses for subdomains are not deleted there's a risk of take over.
  - Alerts
  - Trackers
  - Reverse lookup
    - Finding IPs --> C&C domains.

_________________________________________

## Side notes
Complete address : ip + port\
CIDR : non routabke IPs
<br>
<br>
Telnet port : 23
<br>
<br>
Canari tokens : Fake docs / pages that they are kept somewhere not easy to find
and when someone reaches them then they are performing footpinting.
<br>
<br>
Education and awareness is most important