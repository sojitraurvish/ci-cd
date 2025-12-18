how and why ci and cd

continous integration (why you check test here because husky is precommint hook which runing before you make commit but peopel can fool it via some command like git commit -m "messs" --no-verify)
ci - build project
   - ruining automated test
   - are test runing 
   - are they folloing best practices
   - is code linted well


continouse deployment - here you deploy the code and above you just check the code 
cd - dev stage prod

//deployment should not happen when someone creates a pool req, depolyment should happend when commit happes for master branch the deploment should happen

so in comanies first you make changes to dev and dev automatically deploy to dev.100x.com

and once every two week you merge dev branch to master branch and it deploys to prod and this is called releas cycly

// cd things

// you have to first push iamge to docker hub so you need to login first so create access token direct from docker hub and you can directly put these secrate
in pipeline file but it got expose to the word so go to (in repo) setting > secrate and variables > actions > Repository secrets > here create two vars
DOCKER_USERNAME=sojitraurvish
DOCKER_PASSWORK=your docker hub access token 
and use it in your pipeline files

and make the commit and check this things


