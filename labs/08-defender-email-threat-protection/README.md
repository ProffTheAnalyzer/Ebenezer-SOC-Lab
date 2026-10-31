# Email Policies & Threat Protection

**Original page title:** Configuring Email Policies & Threat Protection  
**Date shown on original site:** Not specified  
**Evidence:** 21 screenshots from the published site

> **Migration note:** Text and image order are transcribed from the PUBLISHED Google Sites export dated October 30, 2026. The original lab conclusions are preserved as written and have not been independently revalidated. Review screenshots for personal or sensitive data before publishing.

## Original lab write-up

**Objective:** Harden email infrastructure against phishing campaigns using Defender for Office 365.

- **Visibility & Tracking:** Utilized the Email & Collaboration Threat Explorer to monitor the environment, gaining deep visibility into user clicks, quarantine statuses, and phishing campaigns.
- **Policy Engineering:** While standard protections provide a baseline, advanced threats require custom rules. I engineered a tailored Safe Links policy (ebpracticelab-safelink) designed to proactively rewrite and neutralize suspicious URLs, effectively neutralizing malicious links before a user can compromise their endpoint.
- **Live Testing:** Emulated an external threat actor by sending a sample scam-themed email containing a test link. The engineered rules successfully detected the anomaly and routed the threat directly to the junk folder.
- **Posture Hardening:** Leveraged the Configuration Analyzer to audit the current email environment against strict security baselines, systematically applying recommended actions to continuously strengthen the perimeter.

## Screenshots (original order)

<details>
<summary>Show all 21 screenshots</summary>

**Screenshot 01**

![Email Policies & Threat Protection — screenshot 01](screenshots/01-cc699615a9872b7174626a1c46cee18f.jpg)

**Screenshot 02**

![Email Policies & Threat Protection — screenshot 02](screenshots/02-a347d94703e19c9a33748993e9ec779b.jpg)

**Screenshot 03**

![Email Policies & Threat Protection — screenshot 03](screenshots/03-92c8d23cd65fded6be090585e7314744.jpg)

**Screenshot 04**

![Email Policies & Threat Protection — screenshot 04](screenshots/04-4b2b5019c22566d213cd2c501c3fc6e7.jpg)

**Screenshot 05**

![Email Policies & Threat Protection — screenshot 05](screenshots/05-43bd4fe76af6cfb4ccb14e43917e77b4.jpg)

**Screenshot 06**

![Email Policies & Threat Protection — screenshot 06](screenshots/06-4e8528aa0d66a755ee2b6c99a907ae1c.jpg)

**Screenshot 07**

![Email Policies & Threat Protection — screenshot 07](screenshots/07-fe9d0153732ab313151f49b299531bbe.jpg)

**Screenshot 08**

![Email Policies & Threat Protection — screenshot 08](screenshots/08-506393e15f0b0274e48a27dd49f96797.jpg)

**Screenshot 09**

![Email Policies & Threat Protection — screenshot 09](screenshots/09-46628d47542bc7c43eaca125744fd1e5.jpg)

**Screenshot 10**

![Email Policies & Threat Protection — screenshot 10](screenshots/10-a26385f11be6d227c5245902eaf5b6d1.jpg)

**Screenshot 11**

![Email Policies & Threat Protection — screenshot 11](screenshots/11-f9fc944aecb964962ce21e2981d752fc.jpg)

**Screenshot 12**

![Email Policies & Threat Protection — screenshot 12](screenshots/12-00bd8d87bd19a5eb13b4ba3b30bdef31.jpg)

**Screenshot 13**

![Email Policies & Threat Protection — screenshot 13](screenshots/13-fb3cc8edc16e9740e4b4c46e72a43272.jpg)

**Screenshot 14**

![Email Policies & Threat Protection — screenshot 14](screenshots/14-9aea0f4348d27ca77685a78b8cabb119.jpg)

**Screenshot 15**

![Email Policies & Threat Protection — screenshot 15](screenshots/15-b9deb8e7d85f8e912b7286492c18e536.jpg)

**Screenshot 16**

![Email Policies & Threat Protection — screenshot 16](screenshots/16-7fdb6008e4bac54b8d4fbcb223354001.jpg)

**Screenshot 17**

![Email Policies & Threat Protection — screenshot 17](screenshots/17-5275ed2e258dcdcaa7d9058b2f62733d.jpg)

**Screenshot 18**

![Email Policies & Threat Protection — screenshot 18](screenshots/18-fe3906fac0f7985aee3418ece78ecf32.jpg)

**Screenshot 19**

![Email Policies & Threat Protection — screenshot 19](screenshots/19-41d385e1f670e0b35587046b7ebf5e45.jpg)

**Screenshot 20**

![Email Policies & Threat Protection — screenshot 20](screenshots/20-f485f59b8e52d586734817df274a4740.jpg)

**Screenshot 21**

![Email Policies & Threat Protection — screenshot 21](screenshots/21-42b2e737317e922db317348422493b11.jpg)

</details>

---

[Back to portfolio index](../../README.md)
