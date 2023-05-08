Download Link: https://assignmentchef.com/product/solved-sdev400-homework3-amazon-lambda-and-api-gateway
<br>



In this homework, you will create a REST APIs using API Gateway. The API will use Lambda as the backend service. You are welcome to use other services we have covered for example S3 and

DynamoDB to store the data but you may also just use methods and datasets within your Lambda code.

Prior to attempting this assignment, be sure you have completed the readings and activities in week 5 and 6. These activities are foundational and required to be successful in completing this homework.

Please get started early as this assignment will take you longer than you think.

<ol>

 <li>Using your AWS Educate classroom environment, create an REST API with a Lambda backend service that provides the results of the last 5 games in a specific sport for a specific team entered by the user. Details regarding the implementation are as follows:</li>

</ol>




<ul>

 <li>The API should provide data for at least 3 different professional or college sports (e.g. Baseball, Football, Basketball)</li>

 <li>The API should provide data for at last 3 different teams for each of the 3 sports. This means you will have data from at least 9 different sporting teams.</li>

 <li>The data needs to be real and current. (Hint: all major sports have sites providing the most recent scores for all of their teams.) Note there will be some issues with current with the recent pandemic so recent might be relative.</li>

 <li>The API will use a Get Query String as input containing the Sports and Teams name. (e.g.</li>

</ul>

?sport=baseball&amp;team=astros). You decide the way you want to refer to a team and a sport.

For example Houston versus Astros, Baltimore versus Orioles.

<ul>

 <li>If a sport is not present in your dataset, just reply “Sport was not found”. Then return a list of all of your possible sports. For example,</li>

</ul>

“Soccer was not found. Please try one of these:

Basketball

Football

Hockey”

<ul>

 <li>If a team is not present in your dataset, just reply “Team was not found”. Then return a list of all of your possible team for the sport selected. For example,</li>

</ul>

“Packers was not found for the Football sport. Please try one of these:

Ravens

Patriots

Chargers”

<ul>

 <li>Upon successful entry of the Sport and the Team name, the API should return the last 4 games, if the team lost or won and the date of the game. For example, if Baseball and Astros were input, the API response might be the following:</li>

</ul>

“For the sport of baseball the Astros last 4 game results include:

Astros beat Rays 6-1 on Oct 10, 2019

Astros lose to Rays 1-4 on Oct 8, 2019

Astros lose to Rays 3-10 on Oct 7, 2019

Astros beat Rays 3-1 on Oct 5, 2019




Note the data should be real sports results representing the time you created the API. Feel free to word the results as you see fit to fulfil the requirements.




Following the previous requirements, the minimum data storage for events will be 3 sports times 3 teams times 4 events = <strong>36</strong>. Feel free to add more if desired.

<ul>

 <li>The Lambda function should be written in Python 3.X.</li>

 <li>The Lambda function should be modular where functions are used to maximize code reuse and efficiency</li>

 <li>Use data structures to store the datasets, <strong>or</strong> read the data in from an S3 or DynamoDB AWS resource. (The latter is more advanced but encouraged if you really want to demonstrate mastery of this material.)</li>

</ul>

<ol start="2">

 <li>(20 points) Describe the API including detailed descriptions and screen captures of your API Resources and Stage. Discuss how and show results of your testing the Lambda function and resulting API that uses the Lambda function backend. <strong>Include your API Endpoint URL </strong>to be run by the professor in your documentation.</li>

</ol>