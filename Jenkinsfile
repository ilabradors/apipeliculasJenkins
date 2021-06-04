pipeline {
   agent { label "master" }
   stages { 
      stage("build"){
      steps { 
         sh "docker build -t apipeliculasIsaias ."
      }
   }
   
   stage("run") { 
      steps { 
         sh "docker run --rm -d  -p 8000:5000/tcp apipeliculasIsaias:latest"
      }
   }

   }

}
