<img align="right" width="250" height="47" src="images/Gematik_Logo_Flag_With_Background.png"/> <br/>    
 
# Release Notes ePA Basic
## Release 3.0.1-1
### changes
- bugfix regex UserAgentType (C_11780)
- typo correction in I_Authorization_Service.yaml
- x-useragent mandatory in I_Information_Service.yaml (C_11779)
- changed http-statuscodes from 200 to 201 or 204 in openapis (C_11811)
- all changed consent decisions in response of updateConsentDecision in I_Consent_Decision_Management.yaml (C_11783)
- regex correction TelematikIdType I_Entitlement_Management.yaml and I_Test_Driver_FdV.yaml (C_11782)
## Release 3.0.1
- release ePA-3.0.1
- (all changes from changelist 'ePAfueralle_3.0.1' and final review)
### changes
- added 'exp' to JWT 'bearerToken' and 'clientAttestation' in I_Authorization_Service.yaml (C_11759)
- changed enc-certificate handling for health record relocation (C_11697) 
- changes in legal policy (concept) for KTR and new category added
- correction of several typos
- added link to 'ref-ePA-HealthRecordMigration' repo for information
- changed amr for the x-authorize-representative situation in I_Authorization_Service.yaml
- reworked correction of depending consent decisions 'medication' and 'erp-submission' (C_11720) after review
- added handling of export package in I_Health_Record_Relocation_Service.yaml (C_11763)
- removed requirement to delete email address of representative if entitlement is deleted
- removed fixed validTo for entitlements via ePA-FdV (OEGD, AM) (concept)
- added vau user pseudonym (VAU-NP) to authorization operation responses in I_Authorization_Service.yaml
## Release 3.0.1 RC
- release candidate ePA-3.0.1
### changes
- added description for allowed PDF/A formats (I_Audit_Event_Render - C_11690) 
- I_Audit_Event_Render_Insurant.yaml renamed to I_Audit_Event_Render.yaml (C_11725) 
- rendered audit events pdf signed or unsigned, also for ombudsoffice (I_Audit_Event_Render - C_11725) 
- correction of depending consent decisions 'medication' and 'erp-submission' (I_Consent_Decicion_Management - C_11720) 
- exclude users with oid_versicherter from category locking related to consent 'medication' (I_Consent_Decicion_Management - C_11691)
- representative can delete own entitlement (I_Entitlement_Management - C_11699)
- reworked device management for explicit device registration and confirmation with confirmation code (I_Device_Management_Insurant - C_11689) 
- reworked concept for device management with confirmation code (concept)
- changes from comment gkv-sv_216 (concept)
- added email management API (I_Email_Management - C_11738)
- reworked authorization service (I_Authorization_Service - C_11707)
- changed http statuscode for setUserExperienceResult (I_Information_Service - C_11750)
- clarification of 'validTo' timestamp for entitlements (I_Entitlement_Management - C_11417)
- bugfixes in I_Audit_Event.yaml
- reworked test driver fdv considering all changes of release 3.0.1 (C_11743)
## Release 3.0.0
- release ePA-3.0
### changes
- editorial changes
- state change fhir resources to _active_
## Release 3.0.0 RC
- release candidate ePA-3.0
## Release 0.0.3
- initial content (pre-release ePA-3.0)
## Release 0.0.2
- initial setup branch
## Release 0.0.1
- initial setup repository
