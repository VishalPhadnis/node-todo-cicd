# Documentation to setup Jenkins CICD pipeline node-todo Application

![image](https://github.com/VishalPhadnis/node-todo-cicd/assets/20634099/528c09f6-535f-471a-9338-dd457a2e1cd4)

# Step 1: Fork the repository: https://github.com/LondheShubham153/node-todo-cicd

![image](https://github.com/VishalPhadnis/node-todo-cicd/assets/20634099/e5e46d51-43b1-499d-b9e6-997a504b37ff)




# Step 2: Login into the Jenkins dashboard and create a freestyle Project

![image](https://github.com/VishalPhadnis/node-todo-cicd/assets/20634099/17c1e569-34da-419f-901b-226b44b0b6c3)




# Step 3: Enter the GitHub repo URL of your forked repository here

![image](https://github.com/VishalPhadnis/node-todo-cicd/assets/20634099/98fd14fc-20f2-42e1-8524-d68d3de4b575)




# Step 4: Select the Source Code Management as Git and paste the URL from the forked repository.

![image](https://github.com/VishalPhadnis/node-todo-cicd/assets/20634099/25193937-ed39-4e6e-a249-2fac3d3003f8)




# Step 5: In Build Triggers: Select the GitHub hook trigger for Gitscm Polling.

![image](https://github.com/VishalPhadnis/node-todo-cicd/assets/20634099/098c310f-9a10-48ac-8aa8-50864d3ee4ff)




# Step 6: Build a link between your Jenkins task and your GitHub Repository through GitHub Integration by utilizing a Git Webhook. Input the git URL of your project.

# Step 7: Open the forked GitHub repository, Go to the repository's "Settings" tab.

# Step 8: Select "Webhooks" from the left-hand menu & Click on the "Add webhook" button.

![image](https://github.com/VishalPhadnis/node-todo-cicd/assets/20634099/9431e87b-7506-4c1e-baf7-3aaf5d385caa)




# Step 9: In the "Payload URL" field, enter the Jenkins URL & Select the events that you want to trigger the webhook.

![image](https://github.com/VishalPhadnis/node-todo-cicd/assets/20634099/c6c787cf-05a9-492c-bb02-d400c02b452a)




# Step 10: Click "Add webhook" to save the webhook configuration.

![image](https://github.com/VishalPhadnis/node-todo-cicd/assets/20634099/94d76ce0-9afb-4dd1-b852-37f089e368a4)




# Step 11: Again come to the Jenkins dashboard, click on Build steps > Execute Shell > Enter the command that will be executed after the job is built & save.

![image](https://github.com/VishalPhadnis/node-todo-cicd/assets/20634099/754e580a-dc36-498f-8324-75d7818126f2)





# Step 12: Now, refresh the page unless the webhook URL is ticked as shown below.

![image](https://github.com/VishalPhadnis/node-todo-cicd/assets/20634099/65d85599-303b-42ea-9619-75e7c10055c0)




# Step 13: Now, to test the webhook, make a small code change in your GitHub repository and commit it:

![image](https://github.com/VishalPhadnis/node-todo-cicd/assets/20634099/f83d7d74-1503-4a78-9244-e52939a1f199)
![image](https://github.com/VishalPhadnis/node-todo-cicd/assets/20634099/3cd4d813-0a6d-463a-939c-c12d0a3b6c00)







# Step 14: Now, whenever you push code to your GitHub repository, the webhook will send a request to the Jenkins job's URL. This will trigger the Jenkins job automatically, running your specified build and deployment steps.

![image](https://github.com/VishalPhadnis/node-todo-cicd/assets/20634099/fbb39a70-24da-4448-bf79-85e0dd66fd9d)
![image](https://github.com/VishalPhadnis/node-todo-cicd/assets/20634099/1e3146c1-f9ec-4153-b601-de7e2d3a4d41)







