echo 'Hello Pipeline'
 def printFunc(val,str){
        if(val==0){
            print str+" is available"
        }else{
             print str+" is Not available"
        }
    }
node("master"){
   
    stage("dotnet"){
        ret =bat(script:"dotnet --version>nul",returnStatus:true);
        printFunc(ret,"Dotnet");
       
    }
     stage("git"){
        ret =bat(script:"git --version>nul",returnStatus:true);
        printFunc(ret,"GIT");
    }
     stage("Angular"){
        ret =bat(script:"ng --version>nul",returnStatus:true);
         printFunc(ret,"Angular");
    }
    stage("Phyton"){
        ret =bat(script:"python --version>nul",returnStatus:true);
         printFunc(ret,"Phyton");
    }
     stage("Node"){
        ret =bat(script:"node --version>nul",returnStatus:true);
        printFunc(ret,"Node");
    }
}
