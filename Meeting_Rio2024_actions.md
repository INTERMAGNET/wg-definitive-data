###  Action items from 2024 Rio meeting

| Number | Responsible | Description | Status 
| ------ | ----------- | ----------- | -----------
|        |             |             | Green completed, Orange ongoing; Red not started
| DD.1   | JRD          | Sending CALL FOR ONE-MINUTE DEFINITIVE DATA FOR 2024 by end of January 2025 | 
| DD.2   | RL   | Sending CALL FOR ONE-SECOND DEFINITIVE DATA FOR 2023 by the end of February 2025 |
| DD.3   | All, JM | Change of DOI handling:  Create DOI as growing repositories for both 1min and 1sec definitive data. To be hosted at GFZ. Automatic transfer and publication time stamping. To be started as soon as possible including 2021 onwards |
| DD.4   | RL, SF, SB |  Migration of 1-min definitive data from IAF to CDF formats. This is a long ongoing process to start after softwares to deal with CDF are available (2026?) | 
| DD.5   | MS, DataCheckers | Incorrect jump signs in year mean files. Not to be corrected by IM. Asking IMOs to correct in latest file and add note in comments. | Marcos to check all existing and non existing IMOs to communicate or add comment. (Contact with Will Brown from BGS/WDC)
| DD.6   | DataCheckers, BH, TR | Clarify permission for data checkers to modify files, to be added into the data checkers guidelines. No changes to be made on existing files in step1. Give 4 weeks to imos to make change before it is made automatic | 
| DD.7   | TR, BH | Frequency of absolute S measures. Data checkers to add this parameter on check list. And communicate with IMOs to either report missing values or start performing regular measures. Only for recent data. | TR volunteered to make a script to detect gaps or lack of pilar measure
| DD.8   | BH,JRD, RL,EXCON | Official letter to IMOs (for def data acceptance). Manually by email for 2020. Later years made automatic using IMBOT. To be signed by Excon.  | 
| DD.9   | Excon | Certificate for Data Checkers | 
| DD.10  |       | Update Technical Manual - Data checking 1-minute | Mention IMBOT, add MagPy 
| DD.11  |       | Update Technical Manual - Data checking 1-minute |
| DD.12  | MG, RL, SB | Development of a new version IBFV base line format to account for manual and automatic measurements | 


Note:
Compilation of the initial version step3-1min for the period 1991-present on the GFZ server based on:
- DOI2020 (1991-2020)
- step2-Paris (2021-present)
- step3-Paris-obsmag (2021-present)


Note:
Structure 
1minute step3 in Paris: 
- Jan informs Benoit about acceptance
- Benoit is "stamping" the data (with actual Publication Date)
- Benoit copies stamped data to obsmag (step3 Paris)
- Issues: steps 3 contains zipped IAF files but no Metadata

New procedure:
- Jan informs - places a specific file on step2.
- IMBOT stamps data (verify!!!!!) and copies complete step2 structure (*1) to step3 and to GFZ
- IMBOT mailer is using READNE contacts
  
(*1) - sometimes, extra files may appear in step 2 that should not be copied to step 3-GFZ.


Testing and application:

1.) develop IMBOT routine to obtain step2 data and stamping ( compare to manually stamped files)
2.) develop notification routine for IMBOT to notify IMO about acceptance
3.) develop upload routine to GFZ
4.) Upload e-mail receiver list to GITHUB IMBOT config

Suggestions for next IAGA Workshop:

- Summer school specifically for data checking (both IMO side and IM side)

Invite:
- Kristina (accepted)
- Marcos (accepted)
- Matthew (accepted)

