## Summary of INTERMAGNET Definitive Data (DD) Subcommittee Meeting Agenda and Reports – Lisbon 2025

This document provides a comprehensive overview of the INTERMAGNET DD Subcommittee meeting scheduled for Lisbon 2025. The content covers agenda items, action item follow-ups from 2024, detailed reports on 1-minute and 1-second definitive geomagnetic data processing, data checking protocols, challenges faced by changes in the data checking team, technical discussions on data formats, and administrative matters related to notifications and certification.

---

### In-situ and online participants
Andrew Lewis (AL), Benoit Heumez (BH), Charles Blais (CB), David Calp (DC), Igor Mandic (IM), Jan Reda (JRD), Jürgen Matzka (JM), Marcos Vinicius da Silva (MVS), Matthew Gard (MG), Roman Leonhardt (RL), Simon Flower (SMF), Shun Imajo (SI), Stephan Bracke (SB), Tero Raita (TR), Virginie Maury (VM)

### Key Highlights and Meeting Agenda

- **Approval of meeting agenda and review of outstanding action items from November 2024.**
- **Reports on the status and progress of 1-minute and 1-second definitive geomagnetic data collection and publication.**
- **Data checking challenges and guidelines, including a “cookbook” for data checkers.**
- **Issues arising from the halt of USGS definitive data production/data checking, with discussion on consequences and mitigation strategies.**
- **Technical discussions on:**
  - K value determination methods for IAF files.
  - Potential updates or creation of a new IBFV 3.00 baseline file format suitable for automatic DI measurements.
  - Possible change of the 1-minute definitive data format from IAF to ImagCDF.
- **Matters related to official notifications, certificates, and communication following publication of definitive data.**
- **Summary of subcommittee action items following the 2025 meeting and any other relevant business.**

---

### 2024 Action Items Review

| Number | Responsible | Description | Status 
| ------ | ----------- | ----------- | -----------
|        |             |             | Green completed, Orange ongoing; Red not started
| DD.1   | JRD          | Sending CALL FOR ONE-MINUTE DEFINITIVE DATA FOR 2024 by end of January 2025 | DONE -sent Feb 5, 2025
| DD.2   | RL   | Sending CALL FOR ONE-SECOND DEFINITIVE DATA FOR 2023 by the end of February 2025 | DONE -sent Feb 28, 2025
| DD.3   | All, JM | Change of DOI handling:  Create DOI as growing repositories for both 1min and 1sec definitive data. To be hosted at GFZ. Automatic transfer and publication time stamping. To be started as soon as possible including 2021 onwards | ongoing
| DD.4   | RL, SF, SB |  Migration of 1-min definitive data from IAF to CDF formats. This is a long ongoing process to start after softwares to deal with CDF are available (2026?) | ongoing
| DD.5   | MS, DataCheckers | Incorrect jump signs in year mean files. Not to be corrected by IM. Asking IMOs to correct in latest file and add note in comments. | DONE communicated?
| DD.6   | DataCheckers, BH, TR | Clarify permission for data checkers to modify files, to be added into the data checkers guidelines. No changes to be made on existing files in step1. Give 4 weeks to imos to make change before it is made automatic | DONE. The document can be added to the Manual appendices and/or sent to the Definitive data checkers along with the call for data.
| DD.7   | TR, BH | Frequency of absolute S measures. Data checkers to add this parameter on check list. And communicate with IMOs to either report missing values or start performing regular measures. Only for recent data. | ongoing. TR volunteered to make a script to detect gaps or lack of pilar measure
| DD.8   | BH,JRD, RL,EXCON | Official letter to IMOs (for def data acceptance). Manually by email for 2020. Later years made automatic using IMBOT. To be signed by Excon.  | Ongoing. A template exists, an Automatic routine is being prepared
| DD.9   | Excon | Certificate for Data Checkers | Ongoing
| DD.10  |       | Update Technical Manual - Data checking 1-minute | Ongoing. Requires the publication of the IMBOT article and 1‑min cookbook (both items will be presented)
| DD.11  | MG, RL, SB | Development of a new version IBFV base line format to account for manual and automatic measurements | Ongoing. Started already, suggestions on IBFV will be presented and discussed

---

### 1-Minute Definitive Data Report

- **Current focus on archival completeness and migration to GFZ architecture.**
- **Consideration of processing steps and necessity of current workflows.**
- **Replacement of the existing FTP connection at Paris GIN with more secure protocols (SFTP).**
- **Communication issues between step 2 and step 3 of data processing under review.**

**Observers responsible for subsets of observatories include:**

| Observer               | Observatories Covered                                                                                   |
|------------------------|-------------------------------------------------------------------------------------------------------|
| Andrew Lewis           | BRD, EBR, FUR, JCO, MAB, NGK, PIL, PST, SUA, VAL, VSS                                                |
| Matthew Gard           | GCK, IRT, KIV, KMH, PAG, PEG, PPT, SBL, SJG                                                          |
| Benoit Heumez          | BOU, BRW, BSL, CMO, DED, FRD, FRN, GUA, IQA, NEW, SFS, SHU                                           |
| David Calp             | API, ASP, CSY, CTA, EYR, GDH, KDU, LRM, MAW, TDC, THL                                               |
| Kusumita Arora         | ESK, FCC, HAD, KHB, MMB, SPG, TSU                                                                    |
| Emmanuel Nahayo        | ARS, CKI, CPL, HUA, KEP, TAM, VOS, YAK                                                               |
| Igor Mandic            | AIA, BEL, GUI, HLP, LVV, STT, WIC                                                                     |
| Orsi Baillie           | HBK, TUC, SIT, VIC                                                                                    |
| Claudia Rossavik       | CLF, DLT, KAK, KOU, MCQ, NAQ, SHE, WNG                                                               |
| Marcos Vinicius da Silva| ABG, BDV, GNG, NCK, SBA                                                                              |
| Hiroaki Toh            | BMT, HER, HYB, LON, LYC, MGD, NVS, VNA                                                               |
| Seiki Asari            | ABK, ASC, BLC, BOX, CBB, HRN, NUR, PET, SOD, TTB                                                     |
| Barbara Leichter       | HON, KIR, PHU                                                                                          |
| Jan Reda               | BFO, DOU, DUR, HRB, IZN, MEA, OTT, RES, SPT, STJ, THY                                                |
| Tero Raita             | CNB, CYG, GAN, JAI, KNY, LER, ORC, UPS, YKC                                                         |

---

### 1-Second Definitive Data Report

- **Data Submission and Processing Workflow**

| Step   | Description                                                                                                   |
|--------|---------------------------------------------------------------------------------------------------------------|
| Step 1 | Data providers submit data to Paris GIN; IMBOT reviews data automatically, converts to ImagCDF 1.3/1.3.1, assigns quality levels (0-2). |
| Step 2 | Data checker manually reviews Step 1 accepted data (levels 1 and 2), provides summary reports and acceptance decisions.                      |
| Step 3 | Final editorial check by DD 1-sec chair; approved data published with DOI by BGS/GFZ.                                                             |

- **IMBOT Automatic Review System:**
  - Identifies new or modified data.
  - Converts data to ImagCDF format.
  - Assigns quality levels: 0 (poor) to 2 (best).
  - Requests data provider review if quality < 2.
  - Assigns manual data checker for level 2 quality data.

- **Software Support:**
  - Two INTERMAGNET public software packages updated for 1-second data preparation and checking.
  - IMCDView is among the notable tools supporting processing and visualization.

---

### Data Checking and Quality Control

- **Cookbook for data checkers reviewed to ensure consistency and clarity in procedures.**
- **Focused discussion on the halt of USGS definitive data production and data checking:**
  - USGS currently on hold; this impacts production and quality control.
  - Consequences include inability to produce:
    - Nowcast Kp index without calibrated variometer data from FRD and SIT.
    - Definitive Kp values without USGS K values from FRD and SIT.
  - Mitigation depends on whether USGS continues providing variometer data and shares software/algorithms for K value calculation.
  - Impact on Dst index production is *Not specified/Uncertain*.
- **Offer from Christina Rossavik to influence mitigation and alternative strategies.**

---

### K Value Determination for IAF Files

- **Methods, differences in approaches, and the DKA data format are under review.**
- **Data checking processes related to K values are being refined to ensure accuracy and consistency.**

---

### Discussion on Updating Data Formats

| Topic                      | Discussion Points                                                                                                            | Proposed Solutions / Considerations                                         |
|----------------------------|------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------|
| Updating IBFV Baseline Files| Current IBFV 2.00 format unsuitable for automatic DI measurements due to limited temporal resolution.                        | - Allow multiple records per day.<br>- Add instrument indicator (manual vs automatic).<br>- Use numeric key:value coding.<br>- Switch to ISO 8601 date format.<br>- Include D, I, F data from DI measurement.<br>- Introduce new IBFV 3.00 format alongside IBFV 2.00 to ensure backward compatibility.<br>- Gradual software package updates to support new format. |
| Changing 1-Minute Data Format| Consideration of switching from IAF to ImagCDF format for 1-minute definitive data.                                           | - Assess necessity and impact on software/checking routines.<br>- Include K values within the data.<br>- Add extensive README/meta-information fields.<br>- Address inclusion of auxiliary data like BLV.<br>- Evaluate overall benefits and implementation challenges. |

---

### Notifications, Certificates, and Official Correspondence

- Discussion on automating notifications regarding publication status of definitive data.
- Issuance of certificates for data checkers to acknowledge their contribution.
- Consideration of additional official letters for data providers or checkers to formalize processes and maintain transparency.

---

### Summary of Action Items Post-2025 Meeting

- Compilation and assignment of new and ongoing action items to ensure progress on data collection, processing, format updates, and quality assurance.
- Focus on addressing technology upgrades, data flow improvements, and procedural clarifications.
- Enhancement of documentation and communication with stakeholders.


| Number | Responsible | Description | Status 
| ------ | ----------- | ----------- | -----------
|        |             |             | Green completed, Orange ongoing; Red not started
| DD.1   | JRD          | Sending CALL FOR ONE-MINUTE DEFINITIVE DATA FOR 2025 by end of January 2026 | 
| DD.2   | RL   | Sending CALL FOR ONE-SECOND DEFINITIVE DATA FOR 2024 and 2025 by the end of February 2026 |  
| DD.3   | MVS, JRD | communication of incomplete/wrong jump signs in yearmean and request for updates in 2026 submission | 
| DD.4   | RL   | reminder for review if not completed within 2 months after data submission, message to chair -include into IMBOT |  included in IMBOT2.0.2 (2025-09-12)
| DD.5   | DC   |  DKA format description for Technical Manual - check Jankowski 1991 | 
| DD.6   | RL   | K inidces, methods and citations | 
| DD.7   | MG, SB, RL | Produce a template of IBFV 3.00 file | 
| DD.8   | TR, BH, all data checkers | updating/reviewing the cookbook and make it ready for TM | 
| DD.9   | IM  | add the data checking template to the cookbook | 
| DD.10   | RL  | include 1-sec checklist to the cookbook | 
| DD.11   | DC,BH, MVS | organizing a data checking course at IAGA WS Kakioka | 
| DD.12  | MVS  | yearly data quality report | 
| DD.13  | TR  | site difference analysis | 
| DD.14  | All, JM  | Change of DOI handling:  Create DOI as growing repositories for both 1min and 1sec definitive data. | 
| DD.15  | RL  | Thank you message with option to obtain updated certificate by Excon. | included in IMBOT2.0.2 (2025-09-12)


---

### Any Other Business (AOB)

- Open floor for additional topics not covered in the agenda.
- Opportunity for members to raise miscellaneous issues or proposals.

---

### Core Concepts and Terminology

| Term                    | Definition / Description                                                                                               |
|-------------------------|-----------------------------------------------------------------------------------------------------------------------|
| **Definitive Data (DD)**| High-quality, finalized geomagnetic data used for scientific and operational purposes.                               |
| **IAF Format**           | INTERMAGNET ASCII format used for definitive data storage.                                                            |
| **ImagCDF Format**       | NetCDF-based format supporting complex metadata and multidimensional data structures, increasingly used in INTERMAGNET data. |
| **IBFV**                 | INTERMAGNET Baseline File Version, used to store baseline geomagnetic measurements.                                    |
| **DI Measurements**      | Variations of the geomagnetic field components D (declination), I (inclination), and F (field intensity).             |
| **Kp Index**             | Planetary geomagnetic activity index derived from observatory data.                                                    |
| **Dst Index**            | Disturbance Storm Time index measuring geomagnetic storm intensity.                                                   |
| **IMBOT**                | Automated data review system used to process and check 1-second definitive data.                                       |
| **Data Checker**         | Designated person responsible for manual review and quality control of submitted data.                                |

---

### Conclusion

The INTERMAGNET DD Subcommittee meeting for Lisbon 2025 is focused on advancing the collection, quality assurance, and publication of definitive geomagnetic data, especially for 1-minute and 1-second resolutions. Key challenges include mitigating the impact of USGS's halted data production, updating legacy data formats to accommodate modern automatic measurements, and ensuring robust data checking protocols supported by updated software tools. The committee emphasizes clear communication, enhanced data security, and procedural transparency through official notifications and certifications.

