### Steps to make a Pull request

0. gw formatSource na pasta que sofreu as alterações
1. mcritic src (para checar os arquivos soy)
2. check_sf *file*
3. git checkout -b *novaissue*
4. Send files to staging area on Sourcetree
5. Press commit
6. Add a comment: *issue* + comments
7. git pull --rebase upstream master
8. git push -f origin [branch name]
9. gh pr --submit liferay
10. Copy URL that will be opened on browser
11. Put url on On JIRA

### Pegar PR de outros usuários
gh pr -u username #numerodoPR

### Steps Ant all
Na pasta Cd/workspace/portal-master/liferay-portal
1. Git checkout master 
2. git pull upstream master
3. git push origin master 
4. Deletar pasta liferay-portal do bundles
5. Adicionar arquivos de configuração
6. Limpar as tabelas do lportal
7. Rodar: git reset --hard HEAD
8. desligar Catalina 
9. ant all

#### Na pasta onde vou trabalhar
Ex: cd/worspace/com.dyna.../dynamic-data-form-builder
1. Ligar catalina
2. /Users/aline/workspace/liferay-portal/gradlew clean deploy

## Desligar catalina
Na pasta /Users/aline/workspace/bundles/liferay-portal/tomcat-8.0.32/bin
1.  ps aux | grep java
2. kill -9 [proccess-number]

## Start do mySql
Mysql.server start
