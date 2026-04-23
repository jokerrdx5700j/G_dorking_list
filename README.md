# Google Dorking Commands - Complete Reference Guide

**⚠️ DISCLAIMER:** These commands are for educational purposes only. Only use these techniques for authorized security testing, legitimate research, or bug bounty programs. Unauthorized access to systems or data is illegal.

---

## Table of Contents

1. [Core Search Operators (1-20)](#core-search-operators-1-20)
2. [URL & Directory Dorks (21-40)](#url--directory-dorks-21-40)
3. [File Type Dorks (41-60)](#file-type-dorks-41-60)
4. [Sensitive Data Dorks (61-80)](#sensitive-data-dorks-61-80)
5. [Logical Operators & Modifiers (81-100)](#logical-operators--modifiers-81-100)
6. [Advanced File Discovery (101-120)](#advanced-file-discovery-101-120)
7. [Environment & Configuration Files (121-140)](#environment--configuration-files-121-140)
8. [Cloud & API Keys (141-160)](#cloud--api-keys-141-160)
9. [Database Exposure (161-180)](#database-exposure-161-180)
10. [Vulnerability & Security Testing (181-200)](#vulnerability--security-testing-181-200)
11. [Specific Technologies (201-220)](#specific-technologies-201-220)
12. [Credentials & Secrets (221-240)](#credentials--secrets-221-240)
13. [Personal & Contact Information (241-260)](#personal--contact-information-241-260)
14. [Medical & Legal (261-280)](#medical--legal-261-280)
15. [Financial & Banking (281-300)](#financial--banking-281-300)

---

## Core Search Operators (1-20)

| # | Command | Description | Example |
|---|---------|-------------|---------|
| 1 | `site:` | Search within a specific website or domain | `site:example.com` |
| 2 | `inurl:` | Find pages with a specific term in the URL | `inurl:admin` |
| 3 | `intitle:` | Find pages with keywords in the title | `intitle:"index of"` |
| 4 | `filetype:` | Search for specific file types/extensions | `filetype:pdf` |
| 5 | `ext:` | Search by file extension (alternative to filetype) | `ext:pdf` |
| 6 | `intext:` | Search for keywords within page text/body | `intext:"password"` |
| 7 | `link:` | Find pages that link to a specific URL | `link:example.com` |
| 8 | `cache:` | Show cached version of a page | `cache:example.com` |
| 9 | `allinurl:` | All search terms must be in the URL | `allinurl:admin login` |
| 10 | `allintitle:` | All search terms must be in the page title | `allintitle:login admin` |
| 11 | `allintext:` | All search terms must be in the text | `allintext:username password` |
| 12 | `related:` | Find websites similar to a given URL | `related:example.com` |
| 13 | `info:` | Get information about a specific URL | `info:example.com` |
| 14 | `define:` | Get definitions of words | `define:security` |
| 15 | `stocks:` | Search stock information | `stocks:AAPL` |
| 16 | `weather:` | Check weather information | `weather:london` |
| 17 | `movie:` | Search for movie information | `movie:inception` |
| 18 | `map:` | Search for maps | `map:paris` |
| 19 | `book:` | Search for books | `book:1984` |
| 20 | `scholar:` | Search academic papers | `scholar:machine learning` |

---

## URL & Directory Dorks (21-40)

| # | Command | Description | Example |
|---|---------|-------------|---------|
| 21 | `intitle:"index of"` | Find directory listings | `intitle:"index of"` |
| 22 | `intitle:"index of" parent directory` | Open directories with parent access | `intitle:"index of" parent directory` |
| 23 | `inurl:/admin/` | Find admin panels | `inurl:/admin/` |
| 24 | `inurl:config` | Locate configuration files | `inurl:config` |
| 25 | `inurl:backup` | Find backup files | `inurl:backup` |
| 26 | `inurl:.git` | Expose Git repositories | `inurl:.git` |
| 27 | `inurl:uploads` | Find upload directories | `inurl:uploads` |
| 28 | `inurl:private` | Locate private directories | `inurl:private` |
| 29 | `inurl:sensitive` | Find sensitive files | `inurl:sensitive` |
| 30 | `inurl:confidential` | Locate confidential documents | `inurl:confidential` |
| 31 | `inurl:secret` | Find secret files | `inurl:secret` |
| 32 | `inurl:wp-admin` | Find WordPress admin panels | `inurl:wp-admin` |
| 33 | `inurl:phpmyadmin` | Locate phpMyAdmin installations | `inurl:phpmyadmin` |
| 34 | `inurl:cpanel` | Find cPanel login pages | `inurl:cpanel` |
| 35 | `inurl:plesk` | Locate Plesk panels | `inurl:plesk` |
| 36 | `inurl:webmail` | Find webmail interfaces | `inurl:webmail` |
| 37 | `inurl:control` | Find control panels | `inurl:control` |
| 38 | `inurl:user` | Find user directories | `inurl:user` |
| 39 | `inurl:administrator` | Locate administrator pages | `inurl:administrator` |
| 40 | `inurl:password` | Find pages with passwords in URL | `inurl:password` |

---

## File Type Dorks (41-60)

| # | Command | Description | Example |
|---|---------|-------------|---------|
| 41 | `filetype:pdf` | Find PDF files | `filetype:pdf` |
| 42 | `filetype:doc` | Find Word documents | `filetype:doc` |
| 43 | `filetype:docx` | Find modern Word documents | `filetype:docx` |
| 44 | `filetype:xls` | Find Excel spreadsheets | `filetype:xls` |
| 45 | `filetype:xlsx` | Find modern Excel files | `filetype:xlsx` |
| 46 | `filetype:ppt` | Find PowerPoint presentations | `filetype:ppt` |
| 47 | `filetype:sql` | Find SQL database files | `filetype:sql` |
| 48 | `filetype:xml` | Find XML configuration files | `filetype:xml` |
| 49 | `filetype:conf` | Find configuration files | `filetype:conf` |
| 50 | `filetype:ini` | Find INI settings files | `filetype:ini` |
| 51 | `filetype:cfg` | Find config files | `filetype:cfg` |
| 52 | `filetype:log` | Find log files | `filetype:log` |
| 53 | `filetype:txt` | Find text files | `filetype:txt` |
| 54 | `filetype:bak` | Find backup files | `filetype:bak` |
| 55 | `filetype:tar` | Find tar archives | `filetype:tar` |
| 56 | `filetype:gz` | Find compressed files | `filetype:gz` |
| 57 | `filetype:zip` | Find ZIP archives | `filetype:zip` |
| 58 | `filetype:7z` | Find 7-Zip archives | `filetype:7z` |
| 59 | `filetype:rar` | Find RAR archives | `filetype:rar` |
| 60 | `filetype:iso` | Find ISO images | `filetype:iso` |

---

## Sensitive Data Dorks (61-80)

| # | Command | Description | Example |
|---|---------|-------------|---------|
| 61 | `intext:"password"` | Find exposed passwords | `intext:"password"` |
| 62 | `intext:"username"` | Find exposed usernames | `intext:"username"` |
| 63 | `intext:"api_key"` | Find exposed API keys | `intext:"api_key"` |
| 64 | `intext:"secret"` | Find secrets in text | `intext:"secret"` |
| 65 | `intext:"token"` | Find authentication tokens | `intext:"token"` |
| 66 | `intext:"credentials"` | Find login credentials | `intext:"credentials"` |
| 67 | `intext:"email"` | Find email addresses | `intext:"email"` |
| 68 | `intext:"phone"` | Find phone numbers | `intext:"phone"` |
| 69 | `intext:"ssn"` | Find social security numbers | `intext:"ssn"` |
| 70 | `intext:"credit card"` | Find credit card information | `intext:"credit card"` |
| 71 | `intext:"confidential"` | Find confidential documents | `intext:"confidential"` |
| 72 | `intext:"private"` | Find private information | `intext:"private"` |
| 73 | `intext:"database"` | Find database references | `intext:"database"` |
| 74 | `intitle:"password"` | Pages with passwords in title | `intitle:"password"` |
| 75 | `intitle:"login"` | Find login pages | `intitle:"login"` |
| 76 | `intitle:"admin"` | Find admin pages | `intitle:"admin"` |
| 77 | `"Index of /" database` | Find exposed databases | `"Index of /" database` |
| 78 | `"Index of /" database.sql` | Find SQL database dumps | `"Index of /" database.sql` |
| 79 | `intext:"database.sql"` | Find SQL dumps in text | `intext:"database.sql"` |
| 80 | `intext:"mysql_dump"` | Find MySQL dumps | `intext:"mysql_dump"` |

---

## Logical Operators & Modifiers (81-100)

| # | Command | Description | Example |
|---|---------|-------------|---------|
| 81 | `-` (Minus) | Exclude results with specific terms | `filetype:log -github.com` |
| 82 | `OR` | Search for either term | `inurl:admin OR inurl:login` |
| 83 | `\|` (Pipe) | Alternative to OR operator | `inurl:admin \| inurl:login` |
| 84 | `AND` | Include all search terms | `inurl:admin AND intext:password` |
| 85 | `+` (Plus) | Force inclusion of a term | `+password +username` |
| 86 | `""` (Quotes) | Search for exact phrases | `"confidential document"` |
| 87 | `*` (Asterisk) | Wildcard for any word | `"index of" *.db` |
| 88 | `..` (Range) | Search within a numeric range | `2020..2025` |
| 89 | `$` (Dollar sign) | Price searches | `$100..$500` |
| 90 | `@` (At symbol) | Social media/email searches | `@twitter` |
| 91 | `#` (Hashtag) | Find hashtags | `#security` |
| 92 | `()` (Parentheses) | Group search terms | `(admin OR administrator)` |
| 93 | `?` (Question mark) | Single character wildcard | `file?.txt` |
| 94 | `AROUND()` | Find terms near each other | `password AROUND(2) username` |
| 95 | `~` (Tilde) | Find synonyms | `~security` |
| 96 | `//` (Double slash) | Alternative site search | `//example.com` |
| 97 | `intitle:index.of` | Find directory indexes (variation) | `intitle:index.of` |
| 98 | `inurl:upload filetype:php` | Find PHP upload forms | `inurl:upload filetype:php` |
| 99 | `site:example.com inurl:admin` | Find admin on specific site | `site:example.com inurl:admin` |
| 100 | `filetype:pdf site:example.com` | Find PDFs on specific site | `filetype:pdf site:example.com` |

---

## Advanced File Discovery (101-120)

| # | Command | Description | Example |
|---|---------|-------------|---------|
| 101 | `intitle:"index of" parent directory` | Find open directories with parent access | `intitle:"index of" parent directory` |
| 102 | `intitle:"index of" "backup"` | Find backup directory listings | `intitle:"index of" "backup"` |
| 103 | `intitle:"index of" "database"` | Find database directory listings | `intitle:"index of" "database"` |
| 104 | `intitle:"index of" ".git"` | Expose Git repositories | `intitle:"index of" ".git"` |
| 105 | `intitle:"index of" ".svn"` | Expose Subversion repositories | `intitle:"index of" ".svn"` |
| 106 | `intitle:"index of" ".env"` | Find environment files | `intitle:"index of" ".env"` |
| 107 | `intitle:"index of" ".htaccess"` | Find Apache configuration files | `intitle:"index of" ".htaccess"` |
| 108 | `intitle:"index of" ".passwd"` | Find password files | `intitle:"index of" ".passwd"` |
| 109 | `intitle:"index of" ".mysql"` | Find MySQL configuration files | `intitle:"index of" ".mysql"` |
| 110 | `intitle:"index of" "web.config"` | Find IIS configuration files | `intitle:"index of" "web.config"` |
| 111 | `intitle:"index of" "config.php"` | Find PHP config files | `intitle:"index of" "config.php"` |
| 112 | `intitle:"index of" "settings.py"` | Find Django settings files | `intitle:"index of" "settings.py"` |
| 113 | `intitle:"index of" "application.yml"` | Find YAML config files | `intitle:"index of" "application.yml"` |
| 114 | `intitle:"index of" "secrets.json"` | Find secrets files | `intitle:"index of" "secrets.json"` |
| 115 | `intitle:"index of" "credentials.txt"` | Find credentials files | `intitle:"index of" "credentials.txt"` |
| 116 | `intitle:"index of" "private_key"` | Find private key files | `intitle:"index of" "private_key"` |
| 117 | `intitle:"index of" "ssh"` | Find SSH directories | `intitle:"index of" "ssh"` |
| 118 | `intitle:"index of" "certificates"` | Find certificate directories | `intitle:"index of" "certificates"` |
| 119 | `intitle:"index of" "keys"` | Find encryption key directories | `intitle:"index of" "keys"` |
| 120 | `intitle:"index of" "uploads"` | Find upload directories | `intitle:"index of" "uploads"` |

---

## Environment & Configuration Files (121-140)

| # | Command | Description | Example |
|---|---------|-------------|---------|
| 121 | `inurl:.env -github` | Find environment files outside GitHub | `inurl:.env -github` |
| 122 | `inurl:.env.local` | Find local environment files | `inurl:.env.local` |
| 123 | `inurl:.env.example` | Find example environment files | `inurl:.env.example` |
| 124 | `inurl:wp-config.php -github` | Find WordPress config files | `inurl:wp-config.php -github` |
| 125 | `inurl:config.php -github` | Find PHP config files | `inurl:config.php -github` |
| 126 | `inurl:database.yml` | Find database configuration files | `inurl:database.yml` |
| 127 | `inurl:secrets.yml` | Find secrets configuration files | `inurl:secrets.yml` |
| 128 | `inurl:settings.ini` | Find INI configuration files | `inurl:settings.ini` |
| 129 | `inurl:application.properties` | Find Java application properties | `inurl:application.properties` |
| 130 | `inurl:appsettings.json` | Find .NET app settings | `inurl:appsettings.json` |
| 131 | `inurl:web.xml` | Find web application configuration | `inurl:web.xml` |
| 132 | `inurl:pom.xml` | Find Maven project files | `inurl:pom.xml` |
| 133 | `inurl:build.gradle` | Find Gradle build files | `inurl:build.gradle` |
| 134 | `inurl:package.json` | Find Node.js package files | `inurl:package.json` |
| 135 | `inurl:requirements.txt` | Find Python requirements files | `inurl:requirements.txt` |
| 136 | `inurl:Gemfile` | Find Ruby Gemfile | `inurl:Gemfile` |
| 137 | `inurl:docker-compose.yml` | Find Docker compose files | `inurl:docker-compose.yml` |
| 138 | `inurl:dockerfile` | Find Dockerfile | `inurl:dockerfile` |
| 139 | `inurl:kubernetes.yml` | Find Kubernetes config files | `inurl:kubernetes.yml` |
| 140 | `inurl:terraform.tf` | Find Terraform files | `inurl:terraform.tf` |

---

## Cloud & API Keys (141-160)

| # | Command | Description | Example |
|---|---------|-------------|---------|
| 141 | `intext:"AKIA"` | Find AWS access keys | `intext:"AKIA"` |
| 142 | `intext:"aws_secret_access_key"` | Find AWS secret keys | `intext:"aws_secret_access_key"` |
| 143 | `intext:"api.github.com"` | Find GitHub API references | `intext:"api.github.com"` |
| 144 | `intext:"github_token"` | Find GitHub tokens | `intext:"github_token"` |
| 145 | `intext:"github_secret"` | Find GitHub secrets | `intext:"github_secret"` |
| 146 | `intext:"stripe_api_key"` | Find Stripe API keys | `intext:"stripe_api_key"` |
| 147 | `intext:"stripe_secret"` | Find Stripe secrets | `intext:"stripe_secret"` |
| 148 | `intext:"slack_token"` | Find Slack tokens | `intext:"slack_token"` |
| 149 | `intext:"slack_webhook"` | Find Slack webhooks | `intext:"slack_webhook"` |
| 150 | `intext:"twilio_api_key"` | Find Twilio API keys | `intext:"twilio_api_key"` |
| 151 | `intext:"sendgrid_api_key"` | Find SendGrid keys | `intext:"sendgrid_api_key"` |
| 152 | `intext:"mailgun_api_key"` | Find Mailgun keys | `intext:"mailgun_api_key"` |
| 153 | `intext:"digitalocean_token"` | Find DigitalOcean tokens | `intext:"digitalocean_token"` |
| 154 | `intext:"heroku_api_key"` | Find Heroku API keys | `intext:"heroku_api_key"` |
| 155 | `intext:"firebase_api_key"` | Find Firebase keys | `intext:"firebase_api_key"` |
| 156 | `intext:"google_api_key"` | Find Google API keys | `intext:"google_api_key"` |
| 157 | `intext:"microsoft_graph_token"` | Find Microsoft Graph tokens | `intext:"microsoft_graph_token"` |
| 158 | `intext:"azure_access_key"` | Find Azure access keys | `intext:"azure_access_key"` |
| 159 | `intext:"gcp_service_account"` | Find GCP service accounts | `intext:"gcp_service_account"` |
| 160 | `intext:"alibaba_access_key"` | Find Alibaba Cloud keys | `intext:"alibaba_access_key"` |

---

## Database Exposure (161-180)

| # | Command | Description | Example |
|---|---------|-------------|---------|
| 161 | `intext:"mysql_dump"` | Find MySQL database dumps | `intext:"mysql_dump"` |
| 162 | `intext:"SQL dump"` | Find SQL database dumps | `intext:"SQL dump"` |
| 163 | `intext:"BEGIN; SELECT"` | Find SQL backup formats | `intext:"BEGIN; SELECT"` |
| 164 | `filetype:sql "CREATE TABLE"` | Find SQL table creation statements | `filetype:sql "CREATE TABLE"` |
| 165 | `filetype:sql "INSERT INTO"` | Find SQL insert statements | `filetype:sql "INSERT INTO"` |
| 166 | `filetype:sql "UPDATE"` | Find SQL update statements | `filetype:sql "UPDATE"` |
| 167 | `filetype:sql "DELETE FROM"` | Find SQL delete statements | `filetype:sql "DELETE FROM"` |
| 168 | `filetype:sql "password"` | Find SQL files with passwords | `filetype:sql "password"` |
| 169 | `filetype:sql "email"` | Find SQL files with emails | `filetype:sql "email"` |
| 170 | `filetype:sql "phone"` | Find SQL files with phone numbers | `filetype:sql "phone"` |
| 171 | `filetype:sql "credit_card"` | Find SQL files with credit cards | `filetype:sql "credit_card"` |
| 172 | `filetype:sql "ssn"` | Find SQL files with SSNs | `filetype:sql "ssn"` |
| 173 | `filetype:db "sqlite"` | Find SQLite database files | `filetype:db "sqlite"` |
| 174 | `filetype:backup "database"` | Find database backups | `filetype:backup "database"` |
| 175 | `filetype:dump "mysql"` | Find MySQL dumps | `filetype:dump "mysql"` |
| 176 | `"database.sql"` | Find exposed database files | `"database.sql"` |
| 177 | `"backup.sql"` | Find backup SQL files | `"backup.sql"` |
| 178 | `"export.sql"` | Find SQL export files | `"export.sql"` |
| 179 | `"users.sql"` | Find user SQL files | `"users.sql"` |
| 180 | `"admin.sql"` | Find admin SQL files | `"admin.sql"` |

---

## Vulnerability & Security Testing (181-200)

| # | Command | Description | Example |
|---|---------|-------------|---------|
| 181 | `intitle:"phpinfo()"` | Find PHP info pages | `intitle:"phpinfo()"` |
| 182 | `intitle:"Test Page"` | Find test/debug pages | `intitle:"Test Page"` |
| 183 | `intitle:"ERROR"` | Find error pages with information disclosure | `intitle:"ERROR"` |
| 184 | `intitle:"Warning"` | Find warning pages with stack traces | `intitle:"Warning"` |
| 185 | `intitle:"Exception"` | Find exception pages with traces | `intitle:"Exception"` |
| 186 | `intitle:"Debug"` | Find debug pages | `intitle:"Debug"` |
| 187 | `intitle:"Development"` | Find development pages | `intitle:"Development"` |
| 188 | `intitle:"Staging"` | Find staging environment pages | `intitle:"Staging"` |
| 189 | `intext:"Stack trace"` | Find pages showing stack traces | `intext:"Stack trace"` |
| 190 | `intext:"Exception in thread"` | Find Java exceptions | `intext:"Exception in thread"` |
| 191 | `intext:"Traceback"` | Find Python tracebacks | `intext:"Traceback"` |
| 192 | `intext:"call stack"` | Find call stack information | `intext:"call stack"` |
| 193 | `inurl:"/admin/login"` | Find admin login pages | `inurl:"/admin/login"` |
| 194 | `inurl:"/admin/panel"` | Find admin panels | `inurl:"/admin/panel"` |
| 195 | `inurl:"/administrator/"` | Find administrator directories | `inurl:"/administrator/"` |
| 196 | `inurl:"/user/login"` | Find user login pages | `inurl:"/user/login"` |
| 197 | `inurl:"/user/register"` | Find user registration pages | `inurl:"/user/register"` |
| 198 | `inurl:"/api/v1/"` | Find API endpoints | `inurl:"/api/v1/"` |
| 199 | `inurl:"/api/admin"` | Find admin API endpoints | `inurl:"/api/admin"` |
| 200 | `inurl:"/api/users"` | Find user API endpoints | `inurl:"/api/users"` |

---

## Specific Technologies (201-220)

| # | Command | Description | Example |
|---|---------|-------------|---------|
| 201 | `intitle:"Dashboard [Jenkins]"` | Find Jenkins dashboards | `intitle:"Dashboard [Jenkins]"` |
| 202 | `intitle:"Grafana"` | Find Grafana dashboards | `intitle:"Grafana"` |
| 203 | `intitle:"Kibana"` | Find Kibana dashboards | `intitle:"Kibana"` |
| 204 | `intitle:"Splunk"` | Find Splunk dashboards | `intitle:"Splunk"` |
| 205 | `intitle:"Docker Registry"` | Find Docker registries | `intitle:"Docker Registry"` |
| 206 | `intitle:"GitLab"` | Find GitLab instances | `intitle:"GitLab"` |
| 207 | `intitle:"Redmine"` | Find Redmine project management | `intitle:"Redmine"` |
| 208 | `intitle:"Jira"` | Find Jira instances | `intitle:"Jira"` |
| 209 | `intitle:"Confluence"` | Find Confluence wikis | `intitle:"Confluence"` |
| 210 | `intitle:"phpMyAdmin"` | Find phpMyAdmin interfaces | `intitle:"phpMyAdmin"` |
| 211 | `intitle:"Adminer"` | Find Adminer database tools | `intitle:"Adminer"` |
| 212 | `intitle:"WebDAV"` | Find WebDAV directories | `intitle:"WebDAV"` |
| 213 | `intitle:"FTP List"` | Find FTP listings | `intitle:"FTP List"` |
| 214 | `intitle:"SFTP"` | Find SFTP interfaces | `intitle:"SFTP"` |
| 215 | `inurl:":3000"` | Find services on port 3000 | `inurl:":3000"` |
| 216 | `inurl:":5000"` | Find services on port 5000 | `inurl:":5000"` |
| 217 | `inurl:":8000"` | Find services on port 8000 | `inurl:":8000"` |
| 218 | `inurl:":8080"` | Find services on port 8080 | `inurl:":8080"` |
| 219 | `inurl:":8443"` | Find services on port 8443 | `inurl:":8443"` |
| 220 | `inurl:":9000"` | Find services on port 9000 | `inurl:":9000"` |

---

## Credentials & Secrets (221-240)

| # | Command | Description | Example |
|---|---------|-------------|---------|
| 221 | `intext:"password =" filetype:conf` | Find password assignments | `intext:"password =" filetype:conf` |
| 222 | `intext:"password: " filetype:txt` | Find password listings | `intext:"password: " filetype:txt` |
| 223 | `intext:"user: " intext:"pass: "` | Find user/pass pairs | `intext:"user: " intext:"pass: "` |
| 224 | `intext:"username: " intext:"password: "` | Find credentials | `intext:"username: " intext:"password: "` |
| 225 | `intext:"login: " intext:"password: "` | Find login credentials | `intext:"login: " intext:"password: "` |
| 226 | `intext:"db_user" intext:"db_password"` | Find database credentials | `intext:"db_user" intext:"db_password"` |
| 227 | `intext:"mysql_user" intext:"mysql_password"` | Find MySQL credentials | `intext:"mysql_user" intext:"mysql_password"` |
| 228 | `intext:"root:" filetype:txt` | Find root credentials | `intext:"root:" filetype:txt` |
| 229 | `intext:"admin:" filetype:txt` | Find admin credentials | `intext:"admin:" filetype:txt` |
| 230 | `intext:"ssh_key" filetype:txt` | Find SSH keys | `intext:"ssh_key" filetype:txt` |
| 231 | `intext:"private_key" filetype:txt` | Find private keys | `intext:"private_key" filetype:txt` |
| 232 | `intext:"rsa_private_key"` | Find RSA private keys | `intext:"rsa_private_key"` |
| 233 | `intext:"dsa_private_key"` | Find DSA private keys | `intext:"dsa_private_key"` |
| 234 | `intext:"-----BEGIN PRIVATE KEY-----"` | Find encrypted private keys | `intext:"-----BEGIN PRIVATE KEY-----"` |
| 235 | `intext:"-----BEGIN RSA PRIVATE KEY-----"` | Find RSA keys | `intext:"-----BEGIN RSA PRIVATE KEY-----"` |
| 236 | `intext:"-----BEGIN OPENSSH PRIVATE KEY-----"` | Find OpenSSH keys | `intext:"-----BEGIN OPENSSH PRIVATE KEY-----"` |
| 237 | `intext:"password123"` | Find common passwords | `intext:"password123"` |
| 238 | `intext:"admin123"` | Find admin passwords | `intext:"admin123"` |
| 239 | `intext:"letmein"` | Find weak passwords | `intext:"letmein"` |
| 240 | `intext:"qwerty"` | Find keyboard pattern passwords | `intext:"qwerty"` |

---

## Personal & Contact Information (241-260)

| # | Command | Description | Example |
|---|---------|-------------|---------|
| 241 | `intext:"email@example.com"` | Find email addresses | `intext:"email@example.com"` |
| 242 | `intext:"contact@"` | Find contact emails | `intext:"contact@"` |
| 243 | `intext:"support@"` | Find support emails | `intext:"support@"` |
| 244 | `intext:"info@"` | Find info emails | `intext:"info@"` |
| 245 | `intext:"phone:" filetype:txt` | Find phone numbers | `intext:"phone:" filetype:txt` |
| 246 | `intext:"mobile:" filetype:txt` | Find mobile numbers | `intext:"mobile:" filetype:txt` |
| 247 | `intext:"fax:" filetype:txt` | Find fax numbers | `intext:"fax:" filetype:txt` |
| 248 | `intext:"address:" filetype:txt` | Find addresses | `intext:"address:" filetype:txt` |
| 249 | `intext:"zip code:" filetype:txt` | Find ZIP codes | `intext:"zip code:" filetype:txt` |
| 250 | `intext:"ssn:" filetype:txt` | Find social security numbers | `intext:"ssn:" filetype:txt` |
| 251 | `intext:"social security"` | Find SSN references | `intext:"social security"` |
| 252 | `intext:"driver license"` | Find driver license references | `intext:"driver license"` |
| 253 | `intext:"passport"` | Find passport references | `intext:"passport"` |
| 254 | `intext:"credit card"` | Find credit card references | `intext:"credit card"` |
| 255 | `intext:"cvv:" filetype:txt` | Find CVV numbers | `intext:"cvv:" filetype:txt` |
| 256 | `intext:"expiration date:" filetype:txt` | Find credit card expiration | `intext:"expiration date:" filetype:txt` |
| 257 | `intext:"name:" intext:"email:" intext:"phone:"` | Find contact lists | `intext:"name:" intext:"email:" intext:"phone:"` |
| 258 | `intext:"employee" intext:"contact" filetype:xls` | Find employee lists | `intext:"employee" intext:"contact" filetype:xls` |
| 259 | `intext:"customer" intext:"email" filetype:csv` | Find customer lists | `intext:"customer" intext:"email" filetype:csv` |
| 260 | `intext:"member" intext:"password" filetype:txt` | Find member lists | `intext:"member" intext:"password" filetype:txt` |

---

## Medical & Legal (261-280)

| # | Command | Description | Example |
|---|---------|-------------|---------|
| 261 | `filetype:pdf "patient"` | Find patient documents | `filetype:pdf "patient"` |
| 262 | `filetype:pdf "medical record"` | Find medical records | `filetype:pdf "medical record"` |
| 263 | `filetype:pdf "prescription"` | Find prescription records | `filetype:pdf "prescription"` |
| 264 | `filetype:pdf "diagnosis"` | Find diagnosis documents | `filetype:pdf "diagnosis"` |
| 265 | `filetype:pdf "confidential" "medical"` | Find confidential medical docs | `filetype:pdf "confidential" "medical"` |
| 266 | `filetype:doc "patient name" "diagnosis"` | Find patient documents | `filetype:doc "patient name" "diagnosis"` |
| 267 | `filetype:xls "patient" "treatment"` | Find patient treatment records | `filetype:xls "patient" "treatment"` |
| 268 | `filetype:pdf "contract"` | Find contracts | `filetype:pdf "contract"` |
| 269 | `filetype:pdf "agreement"` | Find agreements | `filetype:pdf "agreement"` |
| 270 | `filetype:pdf "legal"` | Find legal documents | `filetype:pdf "legal"` |
| 271 | `filetype:pdf "confidential" "legal"` | Find confidential legal docs | `filetype:pdf "confidential" "legal"` |
| 272 | `filetype:doc "NDA"` | Find NDAs | `filetype:doc "NDA"` |
| 273 | `filetype:doc "proprietary"` | Find proprietary information | `filetype:doc "proprietary"` |
| 274 | `filetype:doc "confidential"` | Find confidential documents | `filetype:doc "confidential"` |
| 275 | `filetype:pdf "cease and desist"` | Find C&D letters | `filetype:pdf "cease and desist"` |
| 276 | `filetype:pdf "litigation"` | Find litigation documents | `filetype:pdf "litigation"` |
| 277 | `filetype:xls "case" "notes"` | Find case notes | `filetype:xls "case" "notes"` |
| 278 | `filetype:pdf "attorney"` | Find attorney documents | `filetype:pdf "attorney"` |
| 279 | `filetype:pdf "law firm"` | Find law firm documents | `filetype:pdf "law firm"` |
| 280 | `filetype:pdf "court"` | Find court documents | `filetype:pdf "court"` |

---

## Financial & Banking (281-300)

| # | Command | Description | Example |
|---|---------|-------------|---------|
| 281 | `intext:"routing number"` | Find routing numbers | `intext:"routing number"` |
| 282 | `intext:"account number"` | Find account numbers | `intext:"account number"` |
| 283 | `intext:"swift code"` | Find SWIFT codes | `intext:"swift code"` |
| 284 | `intext:"iban"` | Find IBAN information | `intext:"iban"` |
| 285 | `filetype:pdf "invoice"` | Find invoices | `filetype:pdf "invoice"` |
| 286 | `filetype:xls "invoice"` | Find invoice spreadsheets | `filetype:xls "invoice"` |
| 287 | `filetype:pdf "receipt"` | Find receipts | `filetype:pdf "receipt"` |
| 288 | `filetype:pdf "statement"` | Find bank statements | `filetype:pdf "statement"` |
| 289 | `filetype:xls "balance"` | Find balance spreadsheets | `filetype:xls "balance"` |
| 290 | `filetype:pdf "transaction"` | Find transaction documents | `filetype:pdf "transaction"` |
| 291 | `filetype:xls "payment"` | Find payment records | `filetype:xls "payment"` |
| 292 | `filetype:xls "refund"` | Find refund records | `filetype:xls "refund"` |
| 293 | `filetype:pdf "tax return"` | Find tax returns | `filetype:pdf "tax return"` |
| 294 | `filetype:xls "tax"` | Find tax spreadsheets | `filetype:xls "tax"` |
| 295 | `filetype:pdf "w-2"` | Find W-2 forms | `filetype:pdf "w-2"` |
| 296 | `filetype:pdf "1099"` | Find 1099 forms | `filetype:pdf "1099"` |
| 297 | `filetype:xls "financial"` | Find financial spreadsheets | `filetype:xls "financial"` |
| 298 | `filetype:pdf "financial statement"` | Find financial statements | `filetype:pdf "financial statement"` |
| 299 | `filetype:xls "payroll"` | Find payroll records | `filetype:xls "payroll"` |
| 300 | `filetype:pdf "salary"` | Find salary documents | `filetype:pdf "salary"` |

---

## Advanced Search Combinations

### Example Queries

**Find Admin Panels with Credentials:**
```
inurl:admin filetype:txt intext:"password"
site:example.com inurl:admin
```

**Discover Database Files:**
```
filetype:sql "CREATE TABLE" OR filetype:db
intext:"mysql_dump" OR intext:"database.sql"
```

**Locate API Keys and Secrets:**
```
intext:"api_key" OR intext:"secret" filetype:json
intext:"AKIA" OR intext:"aws_secret_access_key"
```

**Find Exposed Backups:**
```
intitle:"index of" "backup" OR "backup.zip" OR "backup.tar.gz"
filetype:bak OR filetype:backup
```

**Discover Configuration Files:**
```
inurl:.env OR inurl:wp-config.php OR inurl:config.php -github
filetype:xml OR filetype:ini OR filetype:conf
```

**Look for Sensitive Documents:**
```
filetype:pdf "confidential" OR "proprietary" OR "secret"
filetype:doc "password" OR "credentials"
```

---

## Important Safety & Legal Guidelines

### ✅ LEGAL USES:
- Authorized security testing and penetration testing
- Legitimate research and educational purposes
- Finding and reporting your own exposed information
- Bug bounty programs with explicit permission
- Security awareness training (with proper authorization)
- Competitive research on publicly available information
- Academic studies on information disclosure

### ❌ ILLEGAL USES:
- Unauthorized access to computer systems
- Data theft or exfiltration
- Identity theft or fraud
- Corporate espionage
- Privacy violations
- Hacking or exploitation
- Extortion or blackmail
- Any unauthorized use of discovered information

### 📋 RESPONSIBLE DISCLOSURE:
If you discover sensitive information:
1. Do NOT access systems you're not authorized to access
2. Do NOT download or store confidential data
3. Report findings to the organization immediately
4. Use responsible disclosure practices
5. Give reasonable time for remediation
6. Follow ethical hacking guidelines

### ⚖️ LEGAL CONSEQUENCES:
Unauthorized access or exploitation can result in:
- Criminal charges and imprisonment
- Civil lawsuits and damages
- Fines up to $250,000+ (in some jurisdictions)
- Permanent criminal record
- Loss of employment and professional licenses

---

## Resources for Learning

- [Google Advanced Search Help](https://support.google.com/websearch/answer/2466433)
- [OWASP Security Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)
- [HackerOne Bug Bounty Platform](https://www.hackerone.com/)
- [Bugcrowd Security Testing](https://www.bugcrowd.com/)
- [Defensive Security Mindset](https://www.defensivesecurity.org/)

---

**Last Updated:** 2026-04-23  
**Total Commands:** 300+  
**Status:** Complete Reference Guide
