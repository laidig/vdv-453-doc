Server Interface for Real-time Information

Changes to SIRI schema 1.3c         since 1.0 

Note that this is a work in progress version that may be updated further

(C) CEN SIRI 2007,2008

2007 04 17 
    Name Space improvements
        revise to use explicit namespaces
        Change name space :  http://siri.org.uk/ ==? siri.org.uk/siri
        
    harmonise Facility Monitoring 
         Revise SpecialNeeds to use  acsb package
         Use Ifopt facility etc        
         Factor out Extensions to utilty file
         
2007 10  17 
      Add Situation Exchange & Facility Exchange services.
      Added a  siri_all-v1.2.xsd, ifopt_allStopPlace-v0.3.xsd, acsp_all.xsd packages to force explicit declaration of all elements in an imported namespace on the first reference. This overcomes a limitation of some XML tools that only pick up thos elements on the first import and ignotre all subsequent imports.  
      
2008 02  12    
      Add SIRI-SX revisions Datex2 harmonisation features
      
2008 03  12    
       Add comments for elements and arrtributes that lacked them
       Correct wdsl errors 
       strip out degree character
       BeyondHorizon type corrected 
       
2008 03 26
      fix SituationIDentity to have ref to ifotp_all so that JAXB binding works
      correct ifopt_All to have all files
      Remove ref to £ from name
        
      Add LineDirection wrapper to request to fix AXIS binding probkem
         ProductionTimetableRequest 
         EstimatedTimetableRequets
      Drop Flat forms in response for
          StopTimetableService  TargetedVisit
          StopMonitoringService StopVisit  StopMonitoringServicePointsFlattenedGroup
          VehicleMonitoringService  VehicleActivity VehicleActivityFlattenedMonitoredJourneyGroup
          rdsPublic\siri\schema\1.3\siri_stopMonitoring_service.xsd(434): <xsd:group name="">
            
      Drop untyped FacilityRef in StopMonitoringResponse
     
            
2008 03 27
    Fix up ifopt & ACSB version numbers to match ifopt 0.4 

2008 04 17 
    Add missing order to stop visit cancellation