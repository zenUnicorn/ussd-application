Install the Heroku CLi
So open up the terminal or Git bash to the root folder of where you have the project for the USSD application
$ heroku login
login using your credentials to the Heroku CLI:
$ git init
Initialized the project as a Git repository:
$ heroku git:remote -a <Your app name here you created on heroku>
Adding the Heroku remote to have access to push to it:
$ git add .
Adding the file to Git for staging:
$ git commit -am "initial commit for ussd application"
pushing the code:
$ git push heroku master
Pushing to the Heroku master branch for deployment. If success, head over to Heroku, reload and click on the open app button at the top right then copy the URL.

The URL will look something like below:
https://ussd-applee.herokuapp.com/
Click on the Go To Sandbox app
Click on the USSD section tab at the left-hand side and click on Create Channel.
Then add your channel number and enter the Heroku app url then click on create a channel.
Now, it’s time to test our application, click on the launch simulator.
Then choose your country from the dropdown option and enter your mobile number and click on launch.
Click on USSD from the simulator option
Then enter your service code in the input box provided and click on call, to simulate how it will work like when been use by the public.
You can also download the mobile app from Play store “Africa stalking” which will still do the same with the web simulator.
Note: Building the USSD and testing with the simulator is free but when you want the public to use your USSD code without using the simulator then you need to pay for the service, you might want to check the pricing out.




Below are some variables used in the Code:

$sessionId: This generates a unique value when the session starts and sent every time a mobile subscriber response has been received.
$serviceCode: This refer to your USSD code
$text: This shows the user input. which is an empty string in the first notification of a session which after that concatenates all the user input within the session until the session ends.
$response: This hold the answer to the user input.
echo: Prints out the response for the user to read.
CON: It means an intermediate menu Or that the session is CONtinuing
END: Means the final menu and will trigger session termination i.e session is ENDing.
