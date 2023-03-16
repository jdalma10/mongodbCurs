
##git url projecte
https://github.com/jdalma10/mongodbCurs.git

##mongosh path
C:\Program Files\mongosh-1.6.2-win32-x64\mongosh-1.6.2-win32-x64\bin

## mongosh exectute external js files

mongosh "mongodb+srv://cluster0.h2kybvz.mongodb.net/school" --apiVersion 1 --username jdalma10 "C:\Program Files\mongosh-1.6.2-win32-x64\mongosh-1.6.2-win32-x64\bin\scripts\CreateSchoolSchema.js"

##execute postman files via newnam
newman run "MongoDB Data API.postman_collection.json" -e "Data API.postman_environment.json"

##execute newmans report
npm install -g newman-reporter-htmlextra 
newman run "MongoDB Data API.postman_collection.json" -e "Data API.postman_environment.json" -r htmlextra

###Execute CrudStudentsExercice.js to Atlas MongoDB Database
mongosh "mongodb+srv://cluster0.h2kybvz.mongodb.net/school" --apiVersion 1 --username jdalma10 "C:\Program Files\mongosh-1.6.2-win32-x64\mongosh-1.6.2-win32-x64\bin\scripts\CrudStudentsExercise.js"

-You must install firs pymongo via pip python -m pip install pymongo

###Mongosh Executes an external javascript file
mongosh "127.0.0.1/school" "StudentsValidation.js" mongosh "127.0.0.1/school" "StudentsInsert.js"