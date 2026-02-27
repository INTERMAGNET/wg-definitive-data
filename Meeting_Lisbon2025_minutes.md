### Summary of INTERMAGNET Definitive Data (DD) Subcommittee Meeting Agenda and Reports – Lisbon 2025

This document provides a comprehensive overview of the INTERMAGNET DD Subcommittee meeting scheduled for Lisbon 2025. The content covers agenda items, action item follow-ups from 2024, detailed reports on 1-minute and 1-second definitive geomagnetic data processing, data checking protocols, challenges faced by USGS in data production, technical discussions on data formats, and administrative matters related to notifications and certification.

---

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

| Action Item Code | Description                                       | Status/Notes                                |
|------------------|-------------------------------------------------|---------------------------------------------|
| DD.02            | Call for 1-second data submissions for 2023     | To be sent out by end of February 2025      |
| DD.02 (future)   | Call for 1-second data submissions for 2025     | Planned for sending out in 2026              |
| DD.05            | Investigation of jumps in yearmeans              | Report by Marcos Vinicius da Silva           |

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
- Continued monitoring of USGS involvement and impact on data products.
- Enhancement of documentation and communication with stakeholders.

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

The meeting agenda and supporting reports reflect a commitment to continuous improvement in geomagnetic data management, balancing legacy systems with evolving technological capabilities.

---

**All information is strictly based on the provided source content.**
