# Jira-Rest-API
coded in C#

Development platform : Visual studio 2019 

https://github.com/guihen01/Jira-Rest-API/blob/main/Capture.PNG

use Microsoft Net.Core 

use Json package (newtonsoft.Json v12.0.3)

# How to use
allow to make a rest api request to jira server 
it is based on rest api library of Atlassian 
ref : https://docs.atlassian.com/software/jira/docs/api/REST/8.13.2/
the excutable code when lounched ask some questions for starting the corresponding rest API

# Parameters 
1) pathanme and name of the json file   
   could be :  C:\C#Rest-API\Execute-RestAPI-POST\Execute-Jira-RestAPi\create-issue.json
   
   the json file could be the json file yu choose, 
   but it must match the json format required in https://docs.atlassian.com/software/jira/docs/api/REST/8.13.2/
2) URL of the jira server : that is the point on which to send the REst API httprequest :  
  ( ie : exemple : http://localhost:8080/rest/api/2/issue )
3) auth : username and password of a granted account to jira server

# it is distributed as nuget package 
reference to download the package is : 
https://www.nuget.org/packages/Execute-Jira-RestAPi/

# Sample
See sample in https://github.com/guihen01/Jira-Rest-API/tree/main/Test-Create-Issue

sample is the use of a "create issue" whith rest api : https://docs.atlassian.com/software/jira/docs/api/REST/8.13.2/#api/2/issue-createIssue
Creates an issue or a sub-task from a JSON representation.
the issueType field must correspond to a sub-task issue type (you can use /issue/createmeta to discover sub-task issue types), and
you must provide a parent field in the issue create request containing the id or key of the parent issue.
