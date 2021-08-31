# dialogflowcx_agent_complaints
Participation in Google's dialogflow-cx competition in August 2021 to create an open source flow/agent

## In this repo you will find
1. [Exported agent blob](agent/exported_agent_complaints.blob)

## Quick Summary:
This is an agent that assist users in filing complaints, retrieving and updating complaints that were filed before. 


#### Aside from above objectives, some important components instilled are:
1. Handling for user verification (ask for phone number, ID/passport)
2. Redirects to human agent when prompted or when bot can't handle the conversation


#### This use case sufficiently demonstrate:
1. Bypass sequential form filling method; instead use intents and entities to perform slot filling of multiple parameters in one go
2. Reuse of one flow (user verification) to redirects to multiple downstream flows based on session parameters


#### What I learnt?
1. Designing conversation is a rabbit hole. You cannot aim to be perfect in every single way
2. It's impossible to cover all angles/possibilities of small talk. That's a job for language model such as GPT-3 and the likes
3. Useful conversation requires structure and intention, chat bots needs to be able to lead conversation with a purpose.


## DEMO
![video](/resources/dialogflowcx-demo.mp4 "dialogflowcx-demo")
<iframe width="560" height="315" src="https://github.com/EnJunChoong/dialogflowcx_agent_complaints/blob/main/resources/dialogflowcx-demo.mp4?raw=true" frameborder="0" allowfullscreen></iframe>
</iframe>


## FLOWS
### Default Start Flow
![Alt text](/resources/default-start-flow.PNG?raw=true "Default Start Flow")

### Redirect_Agent
![Alt text](/resources/redirect-agent.PNG?raw=true "Redirect_Agent")

### Exit_Conversation
![Alt text](/resources/exit-conversation.PNG?raw=true "Exit_Conversation")

### Complaint_File_New
![Alt text](/resources/complaint-file-new.PNG?raw=true "Complaint_File_New")

### Complaint_Update
![Alt text](/resources/complaint-update.PNG?raw=true "Complaint_Update")