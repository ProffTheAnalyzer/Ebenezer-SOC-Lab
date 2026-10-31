# Cloud Storage Phishing — Email Header & Payload Analysis

**Original page title:** Email Header Analysis -  Cloud Storage Phishing Email leads to credential harvesting & potential identity theft  
**Date shown on original site:** Not specified  
**Evidence:** 15 screenshots from the published site

> **Migration note:** Text and image order are transcribed from the PUBLISHED Google Sites export dated October 30, 2026. The original lab conclusions are preserved as written and have not been independently revalidated. Review screenshots for personal or sensitive data before publishing.

## Original lab write-up

**Objective:** To conduct a comprehensive analysis of a suspicious "Billing Failure" email by analyzing raw SMTP headers to identify the originating infrastructure, and securely detonating the embedded payload within an isolated sandbox environment to map the complete attack chain and adversary objectives.

**Context:** An unsolicited email was received claiming a 2TB "Premium Cloud" subscription payment had failed. The message leveraged high-pressure social engineering tactics, stating the account was in "Pending Deletion" and threatening permanent, irreversible data loss if payment details were not updated within 24 hours. The email lacked any specific branding from a legitimate cloud provider.

### Phase 1: Static Header Analysis

### An inspection of the raw email headers revealed several classic indicators of burner phishing infrastructure and defense evasion techniques:

### Phase 2: Static Header Analysis

An inspection of the raw email headers revealed several classic indicators of burner phishing infrastructure and defense evasion techniques:

- **Sender Obfuscation:** The "From" address utilized MIME Encoded-Word syntax (=?UTF-8?...) to obscure the display name. This technique is deliberately used by threat actors to blind basic string-matching spam filters that might flag keywords like "Cloud Storage Alert."
- **Infrastructure Tracing:** The first external hop (95.154.235.136) originated from Iomart Managed Services (RapidSwitch), a commercial data center in the UK. This indicates the adversary utilized a rented Virtual Private Server (VPS), VPN or compromised cloud infrastructure to launch the campaign, rather than a residential IP.
- **Authentication & Domain Age:** While the email passed DKIM and DMARC checks, it failed SPF. Further OSINT investigation into the sending domain (rveband.com) revealed it was registered only three months prior. The primary domain in the redirect chain was created four months prior, a strong indicator of disposable attacker infrastructure.

### Phase 3: Dynamic Payload Detonation & Attack Chain Mapping

To safely observe the email's behavior and the attacker's ultimate goal, the embedded URL was extracted and detonated within a secure, isolated cloud browser session in this case, ("browser.lol" for free analysis).

The analysis revealed a sophisticated, multi-stage redirection scheme, designed to potentially harvest credentials, financial data and identity:

- **Stage 1 (Intermediary Redirection):** The initial link routed to a domain named prizeswin.com. This page executed a fake "verification" script (displaying checks for Location, User Info, and Entry Status) to build a false sense of legitimacy.
- **Stage 2 (The Lure):** The session was then redirected to secure.totaldrive.com. The page displayed a fraudulent offer for discounted cloud storage services, prompting the user to check out via a prominent PayPal button.
- **Stage 3 (Credential Harvesting):** Clicking the payment button initiated a redirect to a highly convincing, spoofed PayPal portal. The site was engineered to capture data regardless of user action; both the "Sign In" and "Create an Account" workflows immediately prompted the victim for Personally Identifiable Information (PII), billing addresses, and full bank/credit card details.
- Conclusion This campaign demonstrates a well-orchestrated credential harvesting operation. By combining psychological urgency with obfuscated routing and multi-stage redirects, the adversary aimed to bypass email security gateways to commit identity theft and financial fraud.

## Screenshots (original order)

<details>
<summary>Show all 15 screenshots</summary>

**Screenshot 01**

![Cloud Storage Phishing — Email Header & Payload Analysis — screenshot 01](screenshots/01-cadd2b35ea2277ae432d23ad2419797a.jpg)

**Screenshot 02**

![Cloud Storage Phishing — Email Header & Payload Analysis — screenshot 02](screenshots/02-689f0b624b03f8cebc809ac6cf33a611.jpg)

**Screenshot 03**

![Cloud Storage Phishing — Email Header & Payload Analysis — screenshot 03](screenshots/03-e07ec644f9a9cc7647e841ed94279b10.jpg)

**Screenshot 04**

![Cloud Storage Phishing — Email Header & Payload Analysis — screenshot 04](screenshots/04-83297381787de4de4207532608647846.jpg)

**Screenshot 05**

![Cloud Storage Phishing — Email Header & Payload Analysis — screenshot 05](screenshots/05-0eda8271b1c7f0217bc7dbe2563661a2.jpg)

**Screenshot 06**

![Cloud Storage Phishing — Email Header & Payload Analysis — screenshot 06](screenshots/06-9c401be9f9b286d26bc9dd7596a8f859.jpg)

**Screenshot 07**

![Cloud Storage Phishing — Email Header & Payload Analysis — screenshot 07](screenshots/07-1deece8cb25f8ea9de3712a5703dc16a.jpg)

**Screenshot 08**

![Cloud Storage Phishing — Email Header & Payload Analysis — screenshot 08](screenshots/08-66e37f8c4e5df9e9df883046bf523e39.jpg)

**Screenshot 09**

![Cloud Storage Phishing — Email Header & Payload Analysis — screenshot 09](screenshots/09-ac3e8cc59ddfd74845b789e0966eca14.jpg)

**Screenshot 10**

![Cloud Storage Phishing — Email Header & Payload Analysis — screenshot 10](screenshots/10-7f0fe56cd0ad7c884cd94dca89bcad2b.jpg)

**Screenshot 11**

![Cloud Storage Phishing — Email Header & Payload Analysis — screenshot 11](screenshots/11-3ba4430979118d706df7b887e6fd3695.jpg)

**Screenshot 12**

![Cloud Storage Phishing — Email Header & Payload Analysis — screenshot 12](screenshots/12-3499c24bc503eb75bf2b21c8456f80e3.jpg)

**Screenshot 13**

![Cloud Storage Phishing — Email Header & Payload Analysis — screenshot 13](screenshots/13-7d44c416160abb0b696e65d7e746e9fa.jpg)

**Screenshot 14**

![Cloud Storage Phishing — Email Header & Payload Analysis — screenshot 14](screenshots/14-f90924262d3ea8dd0df3d0831e228a36.jpg)

**Screenshot 15**

![Cloud Storage Phishing — Email Header & Payload Analysis — screenshot 15](screenshots/15-8bda1fcb5bb11109cca057968347248c.jpg)

</details>

---

[Back to portfolio index](../../README.md)
