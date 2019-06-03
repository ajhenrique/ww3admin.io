## WAVEWATCH III Trusted Repos Code Manager Meeting - Minutes - June 3rd 02019 0930EDT

### Participants:
- Ifremer: 
- NCEP-EMC: 
- UKMet: 
- USACE: 

1. WW3 Development meeting
- Rescheduled to 6/5/19 10:30am
 + Andy Saulter will present
 + Will go through changes and general procedures, GitFlow, development through centralized issue reporting at auth repo etc.
 + Othe suggestions of topics?

2. Regtests, matrix scripts
- Ali prepared draft page, 
  + Henrique and Jessica to revise
  + Ali to publish prior to Wednesday meeting 
- Status of regtests/matrix at trusted repos
  + ERDC: 
  + UKMO:

3. Transferring branches Vlab-> github 
- Status?
  + Mickael will confirm with Fabrice for deletion
    * Status?
  + ERDC status? 
    * Ali was supposed to talk to Ty about it: status? 
    
4. Updates on activities in each trusted repo
- NCEP
  + Updated esmf feature branch (Makefile for NEMS applications), 
    * Uses generalized cmplr.env and comp/link.tmpl
    * New updates to be added this week 
    * When done will create branch to eliminate specific comp and link scripts (Henrique with Mickael)
  + Status on strategy to port gridgen to GitHub?
  + Status on current wiki page and GitFlow inconsistencies
  + Henrique added io page for code admin minutes/agenda.
- ERDC
  + fix for triads: status?
  + limiter for shallow water: status?
  + Thornton/Guza + Neumann boundary: status?
  + Regtest for Boers case: status?
    * Some of these features/bugfixes were planned to enter develop in the past two weeks
    * Tyler will report
- UKMO
  + Issue with Cray parallel make. Status?
    * Chris has made progress, will report on meeting.
  + Andy will add his code to uprstr over Summer

5. Updating develop and master (next two weeks time frame)
- Develop
  + Update to bugfix fixed file in ounf for NCEP applications
  + Update to bugfix ww3_shel (Andres Sepulveda/Mickael) (Hotfix)
  + Shared object ww3 library (Stelios: integrated to develop)
  + Ifremer: 
    * bugfix for ounf (Hotfix)
    * bigger bugfix for prnc (Hotfix)
- Master
  + Noted Hotfixes for develop will make it to master -> New tag v6.07.2

6. New developments
  + Status of Milestones/issues

7. Forum/FAQ
  + Any further ideas on forum?
    * None this time
  + Status of adding FAQ to wiki (Jessica and Mickael)
    * Jessica has indicated page exists. Needs updates?
    
8. Unfulfilled to dos:
  + Need to add trusted repos POC addresses to GitHub wiki 
  + Add code manager email to Ifremer (Henrique will add Mickael)
