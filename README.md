# dplit-agent

the ernvironment we have right now:
the problem is , jira , sonarqube , github , jira is linked to devlake.
grafana shows all the analytics by running queries to devlake right u know this very well.
the ngage is the company official application for tracking employees data , like attendace , performance etc

now the problem :
when the ceo wants to check the code health  , project developement , or employee performance , or why the project is not performing well , is it because of any employee absency or not worknig well , or any other problem , the exectives look at the kpis , examine it ,it took hald an hour , so we want to remove this and an agent do this for us.


requeirements:
u know the project will be successful if it costs us less also keep this in mind. but does not compromise on result
we will use gemini free apis , the agent reasons properly on every question , solution based on proper resoning,
proper tool calling , if tool calling fails , then resolve the issue properly, like claude works a proper agent , 
like claude traks the conversation points , changes etc, a full agent

front-end a react anglulare or react native android mobile application
back-end as u know models are created in python , u decide the framework the bestfit


what i think :
quering the devlake database on every request if calling needed , it will cost us database load ,  i think what if we create another database local or cloud based , and create a tables according to grafa kpis , and run all the queries that grafa runs , in the new database to get the data in structured way as grafa gets it , and save it there in new database , 
for updataed data , we will run these quereis on every morning to update the data , as we only saves 6 months data.
then we can create tools for every graph , the llm will be able to call and get the data ,this is my theory u can create a better one as well. Ngage will be needed as well to get employee data and resons for answers, database may also have employee data as well ,we may have multiple dashboards on grafa keep this in mind as well


your work:
Cluade is the best engineer i have encountered. Now your work is to create me a pipeline of this project , in document, the best solution u think is best fit , use visuals as well, this is the scope of work document , and u know the rules of scope of work document , how to write it ,


look below this is how a scope of work document look like:
Write your Scope of Work document
Before anything else, before planning, before designing, before coding, each team needs to produce a Scope of Work document. This is the single most important thing you will do in the next few days.
A Scope of Work is not a technical document. It is a clarity document. It forces you to answer: what exactly are we building, for whom, why, and what does done look like? If you cannot write it clearly, you are not ready to build yet.
What your Scope of Work must include:
Problem statement, one paragraph, no jargon. What is broken and who feels it.
Objectives, what will be true when this is done that is not true today.
Scope, what is included in version one. Be specific. List the features.
Out of scope, what you are deliberately not building right now. This is just as important as what you are building.
Stakeholders, who is involved, who is the main user, who signs off.
Deliverables, what exactly will you hand over at the end.
Timeline, week by week, what are you delivering.
Assumptions and risks, what are you assuming to be true, and what could go wrong.


