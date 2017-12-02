# gundulf-commons

nothing really interesting here  
it is just a jar for commons  

in order to deploy it on heroku it is necessary to follow this:
https://devcenter.heroku.com/articles/local-maven-dependencies

1. create a repo directory
2. install this file
3. create a repository entry in the target pom
4. deploy this jar in the localproject.repo
5. deploy to heroku

<code>mvn deploy:deploy-file -Durl=file:///Users/luigi/projects/cmdrp/gundulf.products/repo/ -Dfile=gundulf.commons-1.0.0.jar -DgroupId=org.kj6682 -DartifactId=gundulf.commons -Dpackaging=jar -Dversion=1.0.0</code>

