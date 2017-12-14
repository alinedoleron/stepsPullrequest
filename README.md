### Steps to make a Pull request

1. check_sf *file*
2. git checkout -b *novaissue*
3. Send files to staging area on Sourcetree
4. Press commit
5. Add a comment: *issue* + comments
6. git pull --rebase upstream master
7. git push -f origin [branch name]
8. gh pr --submit liferay
9. Copy URL that will be opened on browser
10. Put url on On JIRA

### Steps Ant all
Cd/workspace/liferay-portal
1. Git checkout master 
2. git pull upstream master
3. git push origin master  
4. desligar Catalina 
5. ant all


#### No subrepo (com.dynamic...)
Cd/workspace/com.dynamic...
1. git checkout master
2. git push origin master
3. git checkout -b issue (ex: LPS-75844) 

#### Na pasta onde vou trabalhar
Ex: cd/worspace/com.dyna.../dynamic-data-form-builder
1. Ligar catalina
2. /Users/aline/workspace/liferay-portal/gradlew clean deploy

## Desligar catalina
Na pasta /Users/aline/workspace/bundles/liferay-portal/tomcat-8.0.32/bin
1.  ps aux | grep java
2. kill -9 35081
