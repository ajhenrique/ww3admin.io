## WAVEWATCH III Trusted Repos Code Manager Meeting - Minutes - June 17th 02019 0930EDT

### Participants:
- Ifremer: 
- NCEP-EMC: Henrique, 
- UKMet: 
- USACE: 

Progress report:
- ERDC
  + Formulating plan to get triads, limiters and lateral boudaries for getting back into develop
    * Triads seem to work well from the coding side, need to have specific reg test to verify this and other features,
- UKMO
  + Preparation for upgrade of op models, not entirely focused on other issues
  + Start work on feature branch for hybrid processing on SMC
- Ifremer
  + Has run matrix to pull requests, will add report of matrix.comp -> reintegrate to develop
  + For master reintegration NCEP should also run reg test


1. WW3 Development meeting
- Google calendar entry with invites to dev list members
  + Will ask code managers to revise and add participants
  + Ty: Encourage developers that they contact code managers and inform about what's going on, in addition to issues add code manager github @name to inform.

2. Regtests, matrix scripts
- Page is published 
  + Added guidance to users on how to use regtests, and when to use matrix
    * Add documentation about regtests, when to use
  + Jessica will add page about code manager procedures 
    * WIll work on that for the next coupe of weeks
- Status of regtests/matrix at trusted repos
  + ERDC: Ty was able to run the matrix in one of ERDC computers, went through the procedure, is further testing. Looks like all is running well, will move on to test with different branches.
  + UKMO: 
  + NCEP: issues with slurm are delaying tests of pull requests, will solve early this week

3. Transferring branches Vlab -> github 
- Huge progress
  + Should be completed  in th enext couple of weeks
    
4. Updates on activities in each trusted repo
- NCEP
  + Updated esmf feature branch (Makefile for NEMS applications), 
    * Ready for reintegration   
  + Gridgen ported to GitHub?
  + Status on the current wiki page and GitFlow inconsistencies
- ERDC
  + fix for triads
  + limiter for shallow water
  + Thornton/Guza + Neumann boundary
  + Regtest for Boers case
- Ifremer
  + Bugfixes, submitted pull request
  + Finished development for tidal constituents that were not working correctly
- UKMO
  + Issue with Cray parallel make
  + Andy will add his code to uprstr over Summer

5. Updating develop and master (next two weeks time frame)
- Develop
  + Update to bugfix fixed file in ounf for NCEP applications
  + Update to bugfix ww3_shel (Andres Sepulveda/Mickael) (Hotfix)
  + Shared object ww3 library (Stelios: integrated to develop)
  + Ifremer: 
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
