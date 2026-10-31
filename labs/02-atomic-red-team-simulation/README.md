# Atomic Red Team Simulation & Detection

**Original page title:** Atomic Red Team Simulation & Detection (May, 2026)  
**Date shown on original site:** May 2026  
**Evidence:** 14 screenshots from the published site

> **Migration note:** Text and image order are transcribed from the PUBLISHED Google Sites export dated October 30, 2026. The original lab conclusions are preserved as written and have not been independently revalidated. Review screenshots for personal or sensitive data before publishing.

## Original lab write-up

**Objective:** Generate realistic threat telemetry to test and validate Defender’s out-of-the-box and custom detection logic.

- **Preparation:** Configured an intentional Antivirus/ASR exclusion path for the C:\ directory housing the Atomic Red Team framework. This ensured Defender would not preemptively quarantine the execution scripts before the tests could run.
- **Adversary Emulation:** Deployed targeted simulations mapped directly to the MITRE ATT&CK framework, specifically executing Persistence (T1547.001) and Credential Access (T1555) techniques.
- **Outcome:** The simulations successfully executed, generating the necessary telemetry to trigger a multi-stage incident within Defender for triage and analysis.

## Screenshots (original order)

<details>
<summary>Show all 14 screenshots</summary>

**Screenshot 01**

![Atomic Red Team Simulation & Detection — screenshot 01](screenshots/01-ff5a1cba3041c83f645b0112be3b34a7.jpg)

**Screenshot 02**

![Atomic Red Team Simulation & Detection — screenshot 02](screenshots/02-7e96e8c4e046ba33986e32242820d76d.jpg)

**Screenshot 03**

![Atomic Red Team Simulation & Detection — screenshot 03](screenshots/03-dec5ffc93f00a08b70e95b609be44e0e.jpg)

**Screenshot 04**

![Atomic Red Team Simulation & Detection — screenshot 04](screenshots/04-9004c91dd5d98adde7a5c8dfeadf10e1.jpg)

**Screenshot 05**

![Atomic Red Team Simulation & Detection — screenshot 05](screenshots/05-a8e39c7ccbabdde24885d4a3459dad53.jpg)

**Screenshot 06**

![Atomic Red Team Simulation & Detection — screenshot 06](screenshots/06-177568d2f12bc8279f0d9d6aa934943a.jpg)

**Screenshot 07**

![Atomic Red Team Simulation & Detection — screenshot 07](screenshots/07-eca6ea925d1e5fe30f0e4cd7a63db5bd.jpg)

**Screenshot 08**

![Atomic Red Team Simulation & Detection — screenshot 08](screenshots/08-8940ff17d6a1359ea567dd4ed8d70975.jpg)

**Screenshot 09**

![Atomic Red Team Simulation & Detection — screenshot 09](screenshots/09-e035baeff55554685580a42e0e14cb0f.jpg)

**Screenshot 10**

![Atomic Red Team Simulation & Detection — screenshot 10](screenshots/10-9e444a0e949f831d84778b3fec572d51.jpg)

**Screenshot 11**

![Atomic Red Team Simulation & Detection — screenshot 11](screenshots/11-a8b15b49b772b38c406349a43bfe3596.jpg)

**Screenshot 12**

![Atomic Red Team Simulation & Detection — screenshot 12](screenshots/12-a22c7b51f596ac07f614876e626e3fd5.jpg)

**Screenshot 13**

![Atomic Red Team Simulation & Detection — screenshot 13](screenshots/13-db446477c986ccc3f9e739e8132bc2cf.jpg)

**Screenshot 14**

![Atomic Red Team Simulation & Detection — screenshot 14](screenshots/14-56a10a724a81f99baa490d2e74d1c196.jpg)

</details>

---

[Back to portfolio index](../../README.md)
