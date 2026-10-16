# Summary of INTERMAGNET Definitive Data Meeting (March 4, 2026)

This summary presents the key points, discussions, and action items from
the INTERMAGNET Definitive Data meeting held on March 4, 2026. The
meeting covered updates on data checking processes, data publication,
workflow automation, data format issues, and upcoming workshops. The
following sections organize the content into thematic areas and a
timeline of action items.
 **Participants**: Roman Leonhardt (Host), Jan Reda, Barbara Leichter,
Tero Raita, Manjula Lingala, David Calp, Emmanuel Nahayo, Jan Wittke,
Orsi Baillie, Marcos Vinicius da Silva, Kusumita Arora, Seiki Asari,
Benoit Heumez

### Agenda Overview

 1. Approval of the agenda
 2. Review and update of DD action items from Lisbon 2025
 3. Status updates on 1-minute and 1-second definitive data,
  including updates on data checking team, data checking procedures
and automatic notifications in the data review process
 4. Presentation and deliberation on the single DOI (Digital Object
Identifier) and quick publication proposal
 5. Specific discussion points:
  1. IMO Ledger Bot concept (D. Calp)
2. Treatment of G=0 in missing-component calculations based on
scalar S (J. Reda)
 6. Summary and update of action items
 7. Any other business

 ### 2025 Action Items from Lisbon and current status summary:

| ActionItem | Responsible | Task / Description | Status / Note |
| :--- | :--- | :--- | :--- |
| **DD.1** | JRD | Sending CALL FOR ONE-MINUTE DEFINITIVE DATA FOR 2025 by end of January 2026 | DONE |
| **DD.2** | RL | Sending CALL FOR ONE-SECOND DEFINITIVE DATA FOR 2024 and 2025 by the end of February 2026 | To be send out in march 2026 |
| **DD.3** | MVS, JRD | Communication of incomplete/wrong jump signs in yearmean and request for updates in 2026 submission | ONGOING |
| **DD.4** | RL | Reminder for review if not completed within 2 months after data submission, message to chair -include into IMBOT | DONE |
| **DD.5** | DC | DKA format description for Technical Manual - check Jankowski 1991 | ONGOING |
| **DD.6** | RL | K indices, methods and citations | ONGOING |
| **DD.7** | MG, SB, RL | Produce a template of IBFV 3.00 file | ONGOING |
| **DD.8** | TR, BH, all data checkers | Updating/reviewing the cookbook and make it ready for TM | DONE |
| **DD.9** | IM | Add the data checking template to the cookbook | DONE |
| **DD.10** | RL | Include 1-sec checklist to the cookbook | ONGOING |
| **DD.11** | DC, BH, MVS | Organizing a data checking course at IAGA WS Kakioka | Time slot parallel to poster session, hybrid |
| **DD.12** | MVS | Yearly data quality report | To be shown in Japan |
| **DD.13** | TR | Site difference analysis | ONGOING |
| **DD.14** | All, JM | Change of DOI handling: Create DOI as growing repositories for both 1min and 1sec definitive data. | ONGOING |
| **DD.15** | RL | Thank you message with option to obtain updated certificate by Excon. | DONE |

 ### Key Topics and Discussions

 #### 1. **Meeting Minutes Automation and Moderation**

- The meeting minutes are generated automatically using an artificial
intelligence tool.
- **Importance of manual review:** AI-generated minutes require
careful verification by designated persons before official
publication.
- The minutes are circulated among the group for comments prior to
finalization.
 #### 2. **Review of Action Items from Lisbon Meeting**
 - **Total action items:** 15 listed at the last meeting (see above).
 - Major ongoing actions include calls for definitive data submissions
for one-minute and one-second resolution.
 - Communication about incomplete or incorrect jump signs in
near-real-time data is in progress but not yet completed.
 - Automatic reminder notifications for data review deadlines are
operational.
 - Enhancement of data format descriptions, notably for the DKA format,
is underway.
  **Data Format and Documentation: DKA Format**
 - The DKA format is an ASCII representation of binary data intended
for easier inspection of K values.
 - Clarification is needed regarding the presence of SK and AK columns
in current and historical files.
 - The current version is preferred for documentation and software
compatibility.
 - DKA files are optional and automatically generated but can be
produced and submitted manually.
 - The technical manual currently lacks a full description of the DKA
format; updates are planned.
 - Software tools like Magpy and IMCDView can read and process DKA
files, but header format inconsistencies have caused issues.
#### 3.1 **Data Checking and Quality Assurance**
 - A large team of data checkers is involved, with two new members for
one-minute data.
- The review process is emphasized as a **unique selling point** of
INTERMAGNET, ensuring high-quality, independently reviewed
definitive data.
- Automated systems (IMBOT) assist in data checking but still require
human oversight.
- Data checking templates, checklists, and a "cookbook" guide have
been developed and are available on INTERMAGNET's GitHub repository.
- A data checking course is planned for the upcoming IAGA workshop in
Kakioka, with discussions on hybrid or online participation options.
 #### 3.2 **One-Second Definitive Data Status**
 - One-second data submissions are handled automatically for initial
steps, with human review ongoing.
- A critical publication step (step 3) is not yet established at the
Paris data center, delaying public availability.
- Reminders have been sent to responsible parties to resolve this
publication bottleneck.
- Production of one-second data has been effective, with many datasets
accepted and awaiting publication.
 #### 3.3 **Automatic Notifications System**
 - Providers receive notifications when their data advances through
review steps (step 1 to step 2 to step 3).
- A reminder email is sent if data review is on hold for two months.
- Notifications aim to improve communication and accelerate data
publication.
- Formal certificates of data acceptance can be issued upon request.
 #### 3.4 **Automation of Data Publication Process**
 - Current step 2 to step 3 publication procedures involve manual
time-stamping and data formatting.
- Plans to automate this process aim to reduce publication delays.
- Faster publication ensures data is available promptly after final
acceptance.
 #### 4. **Single DOI Quick Publication Issue**
- Currently, only data published up to 2020 has a DOI (Digital Object
Identifier) for citable reference.
- A new scheme is proposed to enable continuous, quick publication
with a **single growing repository** for all definitive geomagnetic
data.
- Challenges include maintaining reproducibility of cited data and
adapting file structures/software (IMCDView) to support this new
approach.
- Further technical and organizational discussions are planned; the
topic is postponed to the next INTERMAGNET meeting.
 #### 5.1. **IM Ledger Bot Concept for Workflow Automation**
 - Proposed by David Calp, the IM Ledger Bot is a GitHub-based
automated system to manage data checking workflows and calls for
data.
- The system logs task assignments, progress, and completion in a
dynamic, transparent ledger.
- Benefits include automated reminders, status reporting, and improved
management of bottlenecks in data checking.
- The concept is currently a prototype used by one person.
- Plans for a live demonstration at the next workshop (Kakioka or
Kyoto) are agreed upon.
- Emphasis on balancing technical complexity with ease of use for data
checkers.
 #### 5.2. **Treatment of G Values and Missing Components in Data**
 - The G value represents the difference between vector sum components
and scalar F values.
 - Issue: When missing components (e.g., Z) are calculated from the
scalar F value, the G value becomes zero, losing its original
meaning as a quality check.
 - Different observatories have handled this differently; some use
special codes like 99999 or 88888 to indicate missing or
recalculated values.
 - **Agreement** that:
  - Recalculated components must be flagged clearly in the data.
- The G value should be set to a special missing value
(e.g., 99999) rather than zero.- The README file accompanying data should document when
recalculations have been performed.
- The technical manual and data checker guide need to be updated
to explain these procedures.
 - New number codes could be established in the future to indicate
which component has been modified or whether just F is missing.
Future software updates (for IMCDView, Magpy) are needed to
recognize new flagging conventions.
 #### 6.1. **Workshop and Training Planning**
 - Data checking course to be organized alongside the IAGA workshop in
Kakioka.
- Scheduling to consider available time slots, possibly running in
parallel with poster session.
- Options for hybrid or online participation to accommodate budget and
travel constraints.
- Plans to distribute workshop materials afterwards for wider
accessibility.
 #### 6.2. **Communication and Miscellaneous**
 - Some participants reported not receiving recent calls for data;
action assigned to Jan Reda and Roman Leonhardt to ensure complete
and proper distribution.
- Technical issues with sharing presentations and using Microsoft
Teams were noted; possible switch back to Zoom for future meetings.
- All meeting slides and materials will be distributed to participants
post-meeting.


### Timeline Table: Key Action Items and Status

| Action Item | Description | Assigned To | Status/Notes |
| :--- | :--- | :--- | :--- |
| **DD.1** | Call for one-minute definitive data | JR | Recently sent out |
| **DD.2** | Call for one-second definitive data | RL | To be sent within two weeks |
| **DD.3** | Communicate incomplete/wrong jump signs in near-mean data | MVS, JR | In progress; |
| **DD.4** | Automatic reminder for review within two months | RL | Active; |
| **DD.5** | Description of DKA format in technical manual | DC | Underway; focusing on current DKA version |
| **DD.6** | Review of K-indices and citations in observatory readmes | RL | Started; ongoing |
| **DD.7** | Template for new baseline format supporting AutoDiff | MG | Prepared template; testing pending |
| **DD.8** | Update and review the data checking cookbook | Now all | Cookbook online; feedback ongoing |
| **DD.9** | Add data checking template and checklist to cookbook | IM | Completed and uploaded |
| **DD.10** | Complete one-second data checking checklist | RL | Still missing; ongoing work; online discussion |
| **DD.11** | Organize data checking course at IAGA workshop | DC, BH, MVS | Planning ongoing; hybrid/online options considered |
| **DD.13** | Site difference analysis | TR | Analysis done; summary pending |
| **DD.14** | Change DOI handling and create growing repository | RL, JR, JM | Started; ongoing discussion |
| **DD.15** | Send thank you message upon data reaching publication step | RL | Implemented; messages sent after 2025 data publication |
| **DD.New 1** | IM Ledger Bot demo at Kakioka workshop | DC | Agreed; demo planned |
| **DD.New 2** | Automate step 2 to step 3 data stamping | RL | Assigned; work in progress |
| **DD.New 3** | Update technical manual on calculated components and G value | JR | Assigned; discussion ongoing |
| **DD.New 4** | Resend call for data emails | JR, RL | Assigned; issue to be identified and to be resolved |

### Key Insights and Conclusions
  
 - **Data quality and review** remain central to INTERMAGNET's mission,
with ongoing efforts to improve automation without compromising
manual oversight.
- The **automation of workflows** (IMBOT, IM Ledger Bot) promises to
increase efficiency and transparency but requires careful
integration and user acceptance.
- **Data format clarity**, especially regarding the DKA format and
handling of recalculated components, is critical for data
interoperability and user confidence.
- The **publication process bottleneck** for one-second data must be
resolved promptly to ensure timely public availability.
- The **single DOI publication model** represents a strategic shift--toward continuous, citable data dissemination but faces technical
and organizational challenges.
Workshops, training, and improved communication channels are
prioritized to support data checkers and contributors worldwide.
Clear **flagging protocols** for recalculated data components and
associated metadata are necessary to maintain data integrity and
user understanding.
