### How to use **Tokenizer** task

Follow the below steps to upload this task to your account:

* Download the Tasks repo as [zip file](https://github.com/openalm/VSOTasks/archive/master.zip) or clone it using git:
```
> git clone https://github.com/openalm/VSOTasks.git
```
* Extract the zip file
* Open command prompt and navigate to the folder: **Tokenizer\x.x.x** where x.x.x is the version number for the task.
* Install ```tfx-cli``` utility
```
> npm install -g tfx-cli
```
* To avoid providing credentials in every command, you can login once. Currently supported credential types are Personal Access Tokens and basic auth. [Create a personal access token](http://roadtoalm.com/2015/07/22/using-personal-access-tokens-to-access-visual-studio-online) and paste it in the login command
```
> tfx login
Copyright Microsoft Corporation
Enter collection url > https://youraccount.visualstudio.com/DefaultCollection
Enter personal access token >
logged in successfully
```
You can alternatively use basic auth by passing ```--authType basic``` (read [Configuring Basic Auth](https://github.com/Microsoft/tfs-cli/blob/master/docs/configureBasicAuth.md)).
* Upload the task to your account:
```
> tfx build tasks upload ./
```
* Once the task is uploaded, you would be able to view this task under **Utility** section of tasks 
