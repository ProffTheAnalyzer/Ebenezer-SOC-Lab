# Conditional Access Policy Test

**Original page title:** Conditonal Access Policy Test (May, 2026)  
**Date shown on original site:** May 2026  
**Evidence:** 22 screenshots from the published site

> **Migration note:** Text and image order are transcribed from the PUBLISHED Google Sites export dated October 30, 2026. The original lab conclusions are preserved as written and have not been independently revalidated. Review screenshots for personal or sensitive data before publishing.

## Original lab write-up

**Objective:** Test Zero Trust access controls and evaluate how identity signals are processed to prevent unauthorized access.

- **The Framework:** Conditional Access functions as an intelligent "if-then" gatekeeper, evaluating real-time signals (identity, device health, network location) before granting access to resources.
- **Execution:** After disabling baseline security defaults, I configured a custom block policy targeting authentications originating from a specific "Named Location" (Germany). I then routed my connection through a German VPN node and attempted to authenticate into Outlook.
- **Outcome:** The authentication was successfully blocked post-credential entry. This demonstrates how conditional access mitigates risks like Adversary-in-the-Middle (AiTM) attacks or stolen session cookies by enforcing environmental constraints regardless of valid credentials.
- **Detection Bonus:** The rapid shift in geography between my actual location (United States) and the VPN node (Germany) successfully triggered a custom "Impossible Travel" analytic rule I had previously engineered in Sentinel.

## Screenshots (original order)

<details>
<summary>Show all 22 screenshots</summary>

**Screenshot 01**

![Conditional Access Policy Test — screenshot 01](screenshots/01-8a2da1d4e50f9c5220e7ecdd7e7425c9.jpg)

**Screenshot 02**

![Conditional Access Policy Test — screenshot 02](screenshots/02-89cc78aa24129e6bc92189eda304f13b.jpg)

**Screenshot 03**

![Conditional Access Policy Test — screenshot 03](screenshots/03-794a3e7b7545d265eeac92756eab45fb.jpg)

**Screenshot 04**

![Conditional Access Policy Test — screenshot 04](screenshots/04-4e0ec625e4d84db9b425de673bde2e5b.jpg)

**Screenshot 05**

![Conditional Access Policy Test — screenshot 05](screenshots/05-50df2ebb919fcae8ff4fd80e109406a2.jpg)

**Screenshot 06**

![Conditional Access Policy Test — screenshot 06](screenshots/06-2ae07ffa86726f447581cc73a9fb9fd3.jpg)

**Screenshot 07**

![Conditional Access Policy Test — screenshot 07](screenshots/07-ae2a988ccfc2dbf430f01886dfc63a22.jpg)

**Screenshot 08**

![Conditional Access Policy Test — screenshot 08](screenshots/08-f40a5ecff2af6c994e081bf3e56a9baf.jpg)

**Screenshot 09**

![Conditional Access Policy Test — screenshot 09](screenshots/09-709547953232b7af529520e2355adcd2.jpg)

**Screenshot 10**

![Conditional Access Policy Test — screenshot 10](screenshots/10-139aba1dd3b8e1753399711976d73a5c.jpg)

**Screenshot 11**

![Conditional Access Policy Test — screenshot 11](screenshots/11-e444b4a2f0fed0cb8d258f793608ec78.jpg)

**Screenshot 12**

![Conditional Access Policy Test — screenshot 12](screenshots/12-d69c7af34f81bb662bc404d924176393.jpg)

**Screenshot 13**

![Conditional Access Policy Test — screenshot 13](screenshots/13-c16fcfcedd86562895ce46f317693b3d.jpg)

**Screenshot 14**

![Conditional Access Policy Test — screenshot 14](screenshots/14-3ac35b27d99dd1d713662ea41c51fc90.jpg)

**Screenshot 15**

![Conditional Access Policy Test — screenshot 15](screenshots/15-4217b4525d9eabd9f8d0d849583e4769.jpg)

**Screenshot 16**

![Conditional Access Policy Test — screenshot 16](screenshots/16-9ff0023e356f2cbe470c7a832aa1b345.jpg)

**Screenshot 17**

![Conditional Access Policy Test — screenshot 17](screenshots/17-9215d388e62f51e60db64347328fda04.jpg)

**Screenshot 18**

![Conditional Access Policy Test — screenshot 18](screenshots/18-e2b8e7d93a87b975fe3745bad27d2a9d.jpg)

**Screenshot 19**

![Conditional Access Policy Test — screenshot 19](screenshots/19-eac7f79bdfcd462f52504d2adcb3945a.jpg)

**Screenshot 20**

![Conditional Access Policy Test — screenshot 20](screenshots/20-3fca054c56993cb2e1ea84ebe448c30b.jpg)

**Screenshot 21**

![Conditional Access Policy Test — screenshot 21](screenshots/21-cb43ed78d8fcff4efd67140dd5603ea2.jpg)

**Screenshot 22**

![Conditional Access Policy Test — screenshot 22](screenshots/22-87467706718cf9a931ecd0b03583f625.jpg)

</details>

---

[Back to portfolio index](../../README.md)
