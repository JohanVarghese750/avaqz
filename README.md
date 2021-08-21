# avaqz
avaqz is a Solution for bulk jira creation/update with an interactive UI

## About avaqz
Jira is the tool used inside our organization to track issues/testcases. In my previous role as a quality assurance engineer my team had to create testcases with
a Jira extension called zephyr, and sometimes it is a mammoth of a task creating/updating more than 10 Jiras in a single go thanks to the heavy loading time of the UI.
So I decided to come up with a script that could automatically create  testcase tickets, and this is the result!

Seeing the amount of time that was saved by this tool creating testcases, this was extended to the larger team so they could also worry less about tracking test casea and actually work on the testing! :)

For the ease of use among other team members passing the script as such was not the best option, so decided to extend a UI so that with a click of a button everything was over!

Thus born avaqz!!

## Apologies
Im really sorry on not including the code for avaqz, because this has been adopted as the official tool by the QA team! so the code resideds on the org premise with some sensitive data but its my duty to help anyone who faces issue while developing a similar application, and hey this also gives you the freedom to use the language of your preference while creating a similar application

#### Jira API documentation : https://developer.atlassian.com/server/jira/platform/rest-apis/


API for creating an issue(POST)  : http://localhost:8080/jira/rest/api/2/issue/

Sample Payload  from documentation:
{
    "fields": {
       "project":
       {
          "id": "10000"
       },
       "summary": "No REST for the Wicked.",
       "description": "Creating of an issue using ids for projects and issue types using the REST API",
       "issuetype": {
          "id": "3"
       }
   }
}
------------------------------------------------------------------------------------------------------------------
API for updating an issue(PUT)  : http://localhost:8080/jira/rest/api/2/issue/

Sample Payload  from documentation:
{
    "fields": {
       "project":
       {
          "id": "10000"
       },
       "summary": "No REST for the Wicked.",
       "description": "Creating of an issue using ids for projects and issue types using the REST API",
       "issuetype": {
          "id": "3"
       }
   }
}


citation : The above API and its payload samples are from the very detailed Jira documentation. Please check it out for more info!
