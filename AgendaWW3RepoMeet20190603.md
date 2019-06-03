## WAVEWATCH III Trusted Repos Code Manager Meeting - Minutes - June 3rd 02019 0930EDT

### Participants:
- Ifremer: Mickael
- NCEP-EMC: Henrique, Jessica
- UKMet: Andy
- USACE: Tyler

1. WW3 Development meeting
- Rescheduled to 6/5/19 10:30am
 + Andy Saulter will present
   * Will send title and abstract today
   * Will check if adjustments need to be made to use google hangouts
 + Will go through changes and general procedures, GitFlow, development through centralized issue reporting at auth repo, pull request.
 + Other suggestions of topics?
   * Ty: Encourage developers that they contact code managers and inform about what's going on, in addition to issues add code manager github @name to inform.

2. Regtests, matrix scripts
- Ali prepared draft page, 
  + Henrique and Jessica to revise
  + Add guidance to users on how to use regtests, and when to use matrix
    * Add documentation about regtests, when to use
  + Ali to publish prior to Wednesday meeting 
- Status of regtests/matrix at trusted repos
  + ERDC: Ty was able to run the matrix in one of ERDC computers, went through the procedure, is further testing. Looks like all is running well, will move on to test with different branches.
  + UKMO:

3. Transferring branches Vlab-> github 
- Status?
  + Mickael will confirm with Fabrice for deletion
    * Still waiting to hear from Fabrice,
    * Mickael will send email to Jessica today
  + ERDC status? 
    * Ali planned to talk to Ty about it: needs following up
    * Ty thinks all is moved and ready to be deleted.
  + Jessica will send out emails to individual users based on a spreadsheet.
    
4. Updates on activities in each trusted repo
- NCEP
  + Updated esmf feature branch (Makefile for NEMS applications), 
    * Uses generalized cmplr.env and comp/link.tmpl
    * New updates to be added this week
    * When done will create a branch to eliminate specific comp and link scripts (Henrique with Mickael)
  + Status on the strategy to port gridgen to GitHub?
    * Henrique and Jessica and Ali will discuss this
  + Status on the current wiki page and GitFlow inconsistencies
    * Jessica will update and send an email prior to Wed meeting
  + Henrique added io page for code admin minutes/agenda.
- ERDC
  + fix for triads
    * No progress to report
  + limiter for shallow water
    * No progress to report
  + Thornton/Guza + Neumann boundary
    * No progress to report
  + Regtest for Boers case: status?
    * Some of these features/bugfixes were planned to enter develop in the past two weeks
    * Tyler will report
- Ifremer
  + Bugfixes, submitted pull request
    * netcdf
    * fixed format for ounf
    * bug with shel
    * wind correction switch, missing in make_makefile
    * unstructured mesh boundary points, arrays out of index on open boundaries
      * Most should be considered hotfixes
  + Finished development for tidal constituents that were not working correctly
    * Will push to Ifremer dev branch this
- UKMO
  + Issue with Cray parallel make
    * Chris has made progress and fixed,
    * Submitted pull request will be reviewed by Jessica and Mickael,
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
    * Jessica has indicated page exists, will be updated when needed 
    
8. Unfulfilled to dos:
  + Need to add trusted repos POC addresses to GitHub wiki 
  + Add code manager email to Ifremer (Henrique will add Mickael)

9. Action items
  + gridgen will be needed for summer schools by end of June
    * Will create github repository for gridgen
    * Will move to github: Mickael will push changes made to fix bugs
    * Andy: developments towards python have been made by Tom Durrant, suggested that should feature as a branch under new gridgen repo, 
      * Will discuss on next cod manager meeting
  + Add reviewers to pull requests
