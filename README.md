# QualityMicroART
Replication bundle of the SAC2019 paper

Require:

-- Cyclomatic complexity calculator https://www.npmjs.com/package/complexity-report installed and available on system path   
-- Java 1.8    
-- Maven > 3.3    
  
Installation:

-- include in project build path weavingmodel.jar      
-- include in project build path the user libraries you can find inside /src/main/resources/oclLibrary     
-- mvn install    

Configuration:  
   
-- modify cfg.properties inside src/resource to configure the application:     
    
	qmpath = Quality model path
	msapath = Microservice architecture model path
	gitlocal = Folder to save the microservice architecture repository specified in gitremote property, to conduct static analysis(cyclomatic complexity)
	gitremote = Remote repository of your microservice architecture 

-- anyway the project comes configured with defaults to execute the acmair case study(gitremote=https://github.com/yanglei99/acmeair-nodejs.git)

Output:  

-- evaluated quality model, src/model/qmevaluated.qualitymetamodel   
-- Weaving Model src/model/weaving.mqr     
-- Eclipse modelink to open the modelink editor in Eclipse EMF, src/main/model/result.modelink         


