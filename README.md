##mongosh path
C:\Program Files\mongosh-1.6.2-win32-x64\mongosh-1.6.2-win32-x64\bin

## mongosh exectute external js files
mongosh "mongodb+srv://cluster0.h2kybvz.mongodb.net/school" --apiVersion 1 --username jdalma10 "C:\Program Files\mongosh-1.6.2-win32-x64\mongosh-1.6.2-win32-x64\bin\scripts\CreateSchoolSchema.js"

##execute postman files via newnam
newman run "MongoDB Data API.postman_collection.json" -e "Data API.postman_environment.json"

##execute newmans report
npm install -g newman-reporter-htmlextra
newman run "MongoDB Data API.postman_collection.json" -e "Data API.postman_environment.json" -r htmlextra