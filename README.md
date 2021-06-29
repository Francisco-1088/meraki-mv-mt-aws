<!-- Copy and paste the converted output. -->

<!-----
NEW: Check the "Suppress top comment" option to remove this info from the output.

Conversion time: 15.699 seconds.


Using this Markdown file:

1. Paste this output into your source file.
2. See the notes and action items below regarding this conversion run.
3. Check the rendered output (headings, lists, code blocks, tables) for proper
   formatting and use a linkchecker before you publish this page.

Conversion notes:

* Docs to Markdown version 1.0β29
* Tue Jun 29 2021 16:34:46 GMT-0700 (PDT)
* Source doc: Meraki AWS MT MV Integration
* This is a partial selection. Check to make sure intra-doc links work.
* This document has images: check for >>>>>  gd2md-html alert:  inline image link in generated source and store images to your server. NOTE: Images in exported zip file from Google Docs may not appear in  the same order as they do in your doc. Please check the images!

----->


<p style="color: red; font-weight: bold">>>>>>  gd2md-html alert:  ERRORs: 0; WARNINGs: 0; ALERTS: 59.</p>
<ul style="color: red; font-weight: bold"><li>See top comment block for details on ERRORs and WARNINGs. <li>In the converted Markdown or HTML, search for inline alerts that start with >>>>>  gd2md-html alert:  for specific instances that need correction.</ul>

<p style="color: red; font-weight: bold">Links to alert messages:</p><a href="#gdcalert1">alert1</a>
<a href="#gdcalert2">alert2</a>
<a href="#gdcalert3">alert3</a>
<a href="#gdcalert4">alert4</a>
<a href="#gdcalert5">alert5</a>
<a href="#gdcalert6">alert6</a>
<a href="#gdcalert7">alert7</a>
<a href="#gdcalert8">alert8</a>
<a href="#gdcalert9">alert9</a>
<a href="#gdcalert10">alert10</a>
<a href="#gdcalert11">alert11</a>
<a href="#gdcalert12">alert12</a>
<a href="#gdcalert13">alert13</a>
<a href="#gdcalert14">alert14</a>
<a href="#gdcalert15">alert15</a>
<a href="#gdcalert16">alert16</a>
<a href="#gdcalert17">alert17</a>
<a href="#gdcalert18">alert18</a>
<a href="#gdcalert19">alert19</a>
<a href="#gdcalert20">alert20</a>
<a href="#gdcalert21">alert21</a>
<a href="#gdcalert22">alert22</a>
<a href="#gdcalert23">alert23</a>
<a href="#gdcalert24">alert24</a>
<a href="#gdcalert25">alert25</a>
<a href="#gdcalert26">alert26</a>
<a href="#gdcalert27">alert27</a>
<a href="#gdcalert28">alert28</a>
<a href="#gdcalert29">alert29</a>
<a href="#gdcalert30">alert30</a>
<a href="#gdcalert31">alert31</a>
<a href="#gdcalert32">alert32</a>
<a href="#gdcalert33">alert33</a>
<a href="#gdcalert34">alert34</a>
<a href="#gdcalert35">alert35</a>
<a href="#gdcalert36">alert36</a>
<a href="#gdcalert37">alert37</a>
<a href="#gdcalert38">alert38</a>
<a href="#gdcalert39">alert39</a>
<a href="#gdcalert40">alert40</a>
<a href="#gdcalert41">alert41</a>
<a href="#gdcalert42">alert42</a>
<a href="#gdcalert43">alert43</a>
<a href="#gdcalert44">alert44</a>
<a href="#gdcalert45">alert45</a>
<a href="#gdcalert46">alert46</a>
<a href="#gdcalert47">alert47</a>
<a href="#gdcalert48">alert48</a>
<a href="#gdcalert49">alert49</a>
<a href="#gdcalert50">alert50</a>
<a href="#gdcalert51">alert51</a>
<a href="#gdcalert52">alert52</a>
<a href="#gdcalert53">alert53</a>
<a href="#gdcalert54">alert54</a>
<a href="#gdcalert55">alert55</a>
<a href="#gdcalert56">alert56</a>
<a href="#gdcalert57">alert57</a>
<a href="#gdcalert58">alert58</a>
<a href="#gdcalert59">alert59</a>

<p style="color: red; font-weight: bold">>>>>> PLEASE check and correct alert issues and delete this message and the inline alerts.<hr></p>



## Table of Contents

[Introduction](https://github.com/Francisco-1088/mt-webexteams/blob/master/README.md#intro)

[Webex, MS Teams and Slack MT Alerts with Camera Snapshots and a Flask Server](https://github.com/Francisco-1088/mt-webexteams/blob/master/README.md#flasksnapshots)

[Webex, MS Teams and Slack Alerts with Composite Camera images](https://github.com/Francisco-1088/mt-webexteams/blob/master/README.md#motionrecap)

[Appendix: Adaptive Cards for Webex and MS Teams and Message Blocks for Slack](https://github.com/Francisco-1088/mt-webexteams/blob/master/README.md#appendix)


## Appendix: Reporting with DynamoDB and Cloudwatch


## Introduction

In this project we explore the integration between Meraki MT20 Door Sensor and Meraki MV Cameras, as well as collaboration applications such as Webex and MS Teams using Amazon Web Services.



1. Webex and MS Teams MT Alerts with Camera Snapshots and AWS
2. Webex and MS Teams Alerts with Composite Camera images and AWS

Components:



*   Meraki MV cameras and MT sensors: Provide intelligence on facilities usage through smart cameras with motion and object detection capabilities, and smart intrusion and door sensors.
*   Meraki Dashboard: Configure sensors and define alerting schedules and conditions, as well as provide continuous monitoring and API integrations.
*   Amazon API Gateway: Front door into AWS environments for Webhook events fired from the Meraki Dashboard.
*   AWS Lambda: Serverless environment for running applications, that will receive calls from the API gateway and glue together all other AWS solutions.
*   Amazon DynamoDB: NoSQL database for storing event data in real time, providing alert de-duplication and day 2 reporting and analytics on events.
*   AWS Secrets Manager: Handle API Keys and tokens securely for interacting with the Meraki Dashboard and Cisco Webex.
*   Amazon CloudWatch: Log all events and errors in the system.


## MT Alerts with Camera Snapshots and AWS



<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image1.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image1.png "image_tooltip")


With this integration, you will be able to produce notifications for Webex and MS Teams like in the following example:



<p id="gdcalert2" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image2.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert3">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image2.png "image_tooltip")


The notification will contain:



*   Network Name
*   Sensor Name and Model
*   Timestamp of event
*   A link to the generated camera snapshot
*   A link to the video feed at the specified timestamp

The event workflow is as follows:



1. A person opens a door
2. The door’s MT20 triggers an alert which is sent to the Meraki cloud
3. The Meraki cloud sends a Webhook to a an Amazon API Gateway
4. Amazon API Gateway sends the event to AWS Lambda for processing
5. AWS Lambda queries DynamoDB for the Alert ID, and then discards any duplicate alerts, and processes new ones generating a new entry in DynamoDB
6. The Lambda application retrieves the Meraki Dashboard API Key and Webex Access Token securely from AWS Secrets Manager
7. AWS Lambda requests a snapshot from the camera specified in the sensor tag in the received alert
8. The Meraki Dashboard requests a Snapshot from the specified camera
9. The camera responds to the Meraki cloud
10. The Meraki cloud sends the response to AWS Lambda
11. AWS Lambda sends an Open Door adaptive card from the retrieved snapshot and event to Webex and/or MS Teams
12. AWS Lambda updates the alert entry in DynamoDB with metadata including
    1. Alert ID
    2. Alert Type (Sensor change or motion event)
    3. Network Name
    4. Sensor Name
    5. Sensor Link
    6. Snapshot Link
    7. Video Link
    8. Timestamp

All events and the results of their processing is logged in CloudWatch, and past alerts may be reported on in DynamoDB.


### Webex Setup

If you do not have a Webex developer account, go ahead and create one [here](https://developer.webex.com/). Also, download your Webex app [here](https://www.webex.com/downloads.html).

Log in to the Webex Developer [site](https://developer.webex.com/my-apps), click on your profile at the top right and select My Apps. Create a new App (or if you already have a Webex chatbot, you may reuse).

Choose Create a Bot, give it an easy to remember name and choose an icon for it and a description, and then take note of the Bot access token that appears when you hit Create Bot. This access token won’t be shown again, but you could regenerate it in the future.

Look up your chatbot in Webex and send it a message, doesn’t matter what you type.



<p id="gdcalert3" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image3.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert4">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image3.png "image_tooltip")




<p id="gdcalert4" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image4.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert5">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image4.png "image_tooltip")



### MS Teams Setup

[Sign up](https://products.office.com/en-us/microsoft-teams) free for an MS Teams account, or use your Microsoft account if you have one. Download the MS Teams [client application and install](https://www.microsoft.com/en-us/microsoft-teams/download-app).

Open your MS Teams Client and click on "Teams" on the left side:



<p id="gdcalert5" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image5.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert6">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image5.png "image_tooltip")


Click on Join or create a team at the bottom, choose From scratch and it can be either Public, Org-wide or Private. Once your team is created, click on Apps at the bottom left, and search for Incoming Webhook, and add the Webhook to your previously created team.



<p id="gdcalert6" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image6.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert7">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image6.png "image_tooltip")




<p id="gdcalert7" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image7.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert8">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image7.png "image_tooltip")


Click on Set up a Connector, and give your Webhook a Name, and optionally upload an image to it.



<p id="gdcalert8" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image8.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert9">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image8.png "image_tooltip")


Click on Create and then take note of the Webhook URL for use later.



<p id="gdcalert9" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image9.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert10">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image9.png "image_tooltip")



### Setting up your AWS Environment - Automated



<p id="gdcalert10" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image10.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert11">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image10.png "image_tooltip")


The setup of your AWS environment can be performed in automated fashion using CloudFormation. The current template only supports being deployed in the US-West-1, US-West-2, US-East-1 and US-East-2 regions.

Simply download the cloudformation-mv-mt.yaml file [from the repository](https://github.com/Francisco-1088/meraki-mv-mt-aws) and log into your AWS account (or create a new [AWS Free account](https://aws.amazon.com/free/?all-free-tier.sort-by=item.additionalFields.SortRank&all-free-tier.sort-order=asc&awsf.Free%20Tier%20Types=*all&awsf.Free%20Tier%20Categories=*all)):



1. Type CloudFormation in the search box
2. In the top right, click Create stack with new resources

<p id="gdcalert11" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image11.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert12">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image11.png "image_tooltip")

3. Under Prerequisite select **Template is ready** and under Specify template select **Upload a template file**, and upload the cloudformation-mv-mt.yaml file, and click Next

<p id="gdcalert12" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image12.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert13">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image12.png "image_tooltip")

4. Under specify stack details, fill out the form as in the example, using your environment’s parameters

<p id="gdcalert13" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image13.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert14">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image13.png "image_tooltip")

5. Click Next twice, and scroll down to the bottom, tick the checkbox that says “I acknowledge that AWS CloudFormation might create IAM resources” and click Create Stack



<p id="gdcalert14" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image14.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert15">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image14.png "image_tooltip")


Wait for a minute, and your stack should be created and you’re ready to move on to the Meraki Dashboard configuration.


### Setting up your AWS Environment - Manual

If you deployed your AWS environment via CloudFormation, you can skip this section and go directly to the Meraki Dashboard configuration.

Download the Lambda deployment package  from the Github Repo: [https://github.com/Francisco-1088/meraki-mv-mt-aws](https://github.com/Francisco-1088/meraki-mv-mt-aws)

Log into your AWS account (or create a new [AWS Free account](https://aws.amazon.com/free/?all-free-tier.sort-by=item.additionalFields.SortRank&all-free-tier.sort-order=asc&awsf.Free%20Tier%20Types=*all&awsf.Free%20Tier%20Categories=*all)), and in the Console’s search bar look for AWS Lambda.



<p id="gdcalert15" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image15.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert16">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image15.png "image_tooltip")


Select Create function, choose Author from scratch, give it a name, and select Python 3.7 as your runtime.



<p id="gdcalert16" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image16.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert17">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image16.png "image_tooltip")


Scroll down to Code and on the right, select Upload from .zip file



<p id="gdcalert17" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image17.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert18">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image17.png "image_tooltip")




<p id="gdcalert18" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image18.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert19">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image18.png "image_tooltip")


Click Configuration, and select General configuration - Edit, assigning 256MB of memory, a timeout of 3 minutes and using the existing Role, and then Save.



<p id="gdcalert19" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image19.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert20">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image19.png "image_tooltip")


Back in Configuration, select the Environment variables option, Edit, and fill out the following parameters:



<p id="gdcalert20" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image20.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert21">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image20.png "image_tooltip")




*   MERAKI_BASEURL: Insert the API baseurl you’re using. Normally, [https://api.meraki.com/api/v1](https://api.meraki.com/api/v1)
*   MS_TEAMS_URL (OPTIONAL): Insert your MS Teams Webhook URL from the previous section
*   REGION_NAME: Enter the name of the AWS Region your working on (can check by clicking the option next to Support in your navigation bar, see picture below for reference)



<p id="gdcalert21" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image21.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert22">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image21.png "image_tooltip")


Search for API Gateway in the search box and click on it.



<p id="gdcalert22" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image22.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert23">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image22.png "image_tooltip")


Click Create API and select REST API, clicking on Build.



<p id="gdcalert23" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image23.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert24">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image23.png "image_tooltip")


Give it a name and select Regional type Endpoint.



<p id="gdcalert24" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image24.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert25">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image24.png "image_tooltip")


Click on Actions, Create Methods and select POST



<p id="gdcalert25" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image25.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert26">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image25.png "image_tooltip")


Select Lambda Function as your integration type, and select your region and Lambda function from the list.



<p id="gdcalert26" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image26.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert27">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image26.png "image_tooltip")


Again, click on Actions, select Deploy API, select New Stage and give it a name:



<p id="gdcalert27" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image27.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert28">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image27.png "image_tooltip")


Go to Stages, select your newly created Stage and take note of the Invoke URL up top:



<p id="gdcalert28" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image28.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert29">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image28.png "image_tooltip")


Go back to your Lambda function, and you should be seeing something like this:



<p id="gdcalert29" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image29.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert30">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image29.png "image_tooltip")


In the search bar, type DynamoDB and select it:



<p id="gdcalert30" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image30.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert31">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image30.png "image_tooltip")


Click Create table and give it a name, and specify a primary Key of alertId with the type string and click Create:



<p id="gdcalert31" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image31.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert32">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image31.png "image_tooltip")


Go back to your Function, click Configuration and add a new Environment variable with the name of your DynamoDB table.



<p id="gdcalert32" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image32.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert33">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image32.png "image_tooltip")


In the search box, type Secrets Manager:



<p id="gdcalert33" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image33.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert34">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image33.png "image_tooltip")


Click Store a New Secret, select Other type of secrets and in the left box enter X-Cisco-Meraki-API-Key, and in the right box enter your Dashboard API Key



<p id="gdcalert34" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image34.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert35">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image34.png "image_tooltip")


If you haven’t generated a Meraki Dashboard API Key, just log in to your Dashboard, click on your email address in the top right, select My Profile, scroll down and generate a new API Key, storing the value safely (for example in AWS Secrets Manager).



<p id="gdcalert35" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image35.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert36">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image35.png "image_tooltip")


Give your secret the name X-Cisco-Meraki-API-Key, click Next, select Disable automatic rotation, click Next, review and then Store.

Repeat the previous steps, but now instead of calling it X-Cisco-Meraki-API-Key, call it Webex-Access-Token, and store the value of the Access token you generated in the previous section.



<p id="gdcalert36" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image36.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert37">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image36.png "image_tooltip")


Now, it’s time to give your Lambda Function some permissions. You will first need to obtain the ARN (Amazon Resource Names) for your DynamoDB table, and your two Secrets. To do this go to DynamoDB, select your Table and then scroll all the way down and copy the Amazon Resource Name:



<p id="gdcalert37" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image37.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert38">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image37.png "image_tooltip")


For your secrets, go to Secrets Manager, and click on each of them, and copy the Secret ARN for each of them.



<p id="gdcalert38" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image38.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert39">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image38.png "image_tooltip")


Go back to your function, Click Configuration and then Permissions.

Click on your Execution Role name at the top.



<p id="gdcalert39" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image39.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert40">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image39.png "image_tooltip")


Under permissions, click Add inline policy, we will create permissions for 5 actions your function must perform:



1. Allow Lambda to get your Meraki API Key from Secrets Manager
2. Allow Lambda to get your Webex Access Token from Secrets Manager
3. Allow Lambda to read items in your DynamoDB table
4. Allow Lambda to create items in your DynamoDB table
5. Allow Lambda to update items in your DynamoDB table

For the Secrets:



1. Select Add inline policy
2. Select Secrets Manager under service
3. Select Read Actions, and pick GetSecretValue
4. Under Resources, select specific and add each of the two ARNs for your Secrets
5. Review policy and create



<p id="gdcalert40" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image40.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert41">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image40.png "image_tooltip")


For the DynamoDB permissions:



1. Select Add inline policy
2. Select DynamoDB under service
3. Pick GetItem from Read, and UpdateItem and PutItem from Write
4. Under Resources, select specific and add the ARN for your Table
5. Review policy and create



<p id="gdcalert41" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image41.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert42">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image41.png "image_tooltip")


Go back to your Function Code, and make sure all changes have been Deployed by clicking Deploy.

Meraki Dashboard Configuration

Tag your MTs and MVs in pairs, with the MT having a tag of the format **mv-SERIAL**, where SERIAL is its paired MV camera’s serial, and the MV having a tag of the format **mt-SERIAL**, where SERIAL is its paired MT sensor’s serial. See the example below.



<p id="gdcalert42" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image42.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert43">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image42.png "image_tooltip")


<p id="gdcalert43" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image43.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert44">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image43.png "image_tooltip")


**_Paired MV and MT, where they each reference each other’s serial number in the tag._**

You may also add a tag of **delay-SECONDS** to your MT20 sensor. This tag delays the timestamp used for retrieval of the snapshot from the associated camera by the amount of seconds specified. For example, delay-3, retrieves a snapshot 3 seconds later from the actual opening of the MT20 sensor. This allows for some degree of fine tuning, as fetching the snapshot immediately after the door opens, can result in not capturing the exact moment when the person opening the door is visible.

You can modify this tag even while your receiver is already running.



<p id="gdcalert44" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image44.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert45">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image44.png "image_tooltip")


**_Here the delay-3 tag will make the script fetch snapshots 3 seconds after the door open events._**

Apply a Door Open alert profile to your MT20s and add your Webhook created in the previous section to it. Optionally, if you only want to receive alerts if the door is open for a set amount of time, check the box “Alert only when open for more than…” and choose your preferred amount of time.



<p id="gdcalert45" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image45.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert46">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image45.png "image_tooltip")




<p id="gdcalert46" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image46.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert47">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image46.png "image_tooltip")


If you haven’t, generate an API Key under My Profile, and ask a Meraki SE or NSE to enable MT APIs in your organization.



<p id="gdcalert47" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image47.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert48">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image47.png "image_tooltip")



## Webex, MS Teams and Slack Alerts with Motion Recap images



<p id="gdcalert48" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image48.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert49">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image48.png "image_tooltip")


NOTE: For this section to work, ask your Meraki SE to enable MT APIs in your network.

It’s also possible to receive composite images in your alerts if you’ve set up the Motion Recap functionality as in part I. This part of the code will wait to receive a Motion detected alert, and then the code proceeds to verify the status of the door sensor associated with the camera that sent the alert (via the Tags you set before). If the door status is open, then the Image URL will be downloaded, and a new image will be crafted like the ones below.

Make sure you have tagged your cameras and sensors as described in the previous section. Then, for every camera that you want motion recap events for, enable Motion alerts with the schedule and sensitivity of your preference. Make sure to enable the Motion Recap image within the alert option, and to avoid noisiness define an Area of Interest around the door you’re monitoring.



<p id="gdcalert49" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image49.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert50">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image49.png "image_tooltip")




<p id="gdcalert50" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image50.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert51">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image50.png "image_tooltip")


After this, go into your Network alerts, and add your Webhooks receiver as a custom recipient for Camera motion alerts.



<p id="gdcalert51" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image51.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert52">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image51.png "image_tooltip")


The event workflow is as follows:



1. A person opens a door
2. The camera near the door triggers a motion alert which is sent to the Meraki cloud
3. The Meraki cloud sends a Webhook to a an Amazon API Gateway
4. Amazon API Gateway sends the event to AWS Lambda for processing
5. AWS Lambda queries DynamoDB for the Alert ID, and then discards any duplicate alerts, and processes new ones generating a new entry in DynamoDB
6. The Lambda application retrieves the Meraki Dashboard API Key and Webex Access Token securely from AWS Secrets Manager
7. AWS Lambda requests the state of the sensor specified in the camera tag in the received alert
8. The Meraki Dashboard requests the state of the specified sensor
9. The sensor responds to the Meraki cloud
10. The Meraki cloud sends the response to AWS Lambda
11. If the sensor state is open, AWS Lambda sends a Motion Recap adaptive card from the retrieved Sensor and motion recap image to Webex and/or MS Teams
12. AWS Lambda updates the alert entry in DynamoDB with metadata including
    1. Alert ID
    2. Alert Type (Sensor change or motion event)
    3. Network Name
    4. Camera Name
    5. Camera Link
    6. Snapshot Link
    7. Video Link
    8. Timestamp



<p id="gdcalert52" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image52.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert53">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image52.png "image_tooltip")


The notification will contain:



*   Network Name
*   Camera Name and Model
*   Timestamp of event
*   A link to the video feed at the specified timestamp
*   A link to the associated sensor


## Appendix: Adaptive Cards for Webex and MS Teams

In the previous sections, for Webex and MS Teams you’ve been sending messages to these clients using a specialized format which is called Adaptive Card. This is a specification created by Microsoft, but which is compatible across several messaging platforms. This allows the creation of interactive messages and very visually appealing notifications. You may have seen them before in the Meraki Demo API Platform.

If you want to customize your cards to say something different or display different images, you may do so tweaking the adaptive_cards.py file, where a function has been created for each type of Adaptive Card (Door Open, Snapshot, Door Open for too Long and Motion Recap).

If you want to experiment with creating your own adaptive cards from scratch, you may use the following tools as guidance:



*   [Buttons and Cards](https://developer.webex.com/docs/api/guides/cards)
*   [Buttons and Cards Designer](https://developer.webex.com/buttons-and-cards-designer)


## Appendix: Reporting with DynamoDB and Cloudwatch

You can find all of the Motion and Open door events stored in your DynamoDB table and report on them. Go to DynamoDB and select your Table.

Click on the Items menu, and add filters with the attribute names of alertId, alertType, cameraLink, cameraName, isoTs, networkName, snapshotLink and videoLink, for example:



<p id="gdcalert53" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image53.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert54">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image53.png "image_tooltip")


For troubleshooting your function, you can go to Lambda, choose your function, click Monitor and then in the Logs section you’ll see all of your function invocations. If you click on any of the LogStreams, you can look at the execution of the function



<p id="gdcalert54" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image54.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert55">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image54.png "image_tooltip")




<p id="gdcalert55" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image55.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert56">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image55.png "image_tooltip")


It’s also useful if you record successful invocation events by clicking on the event and copying all of it



<p id="gdcalert56" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image56.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert57">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image56.png "image_tooltip")


You can then go back to your Function code, click on the down arrow next to Test and configure new Test events:



<p id="gdcalert57" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image57.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert58">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image57.png "image_tooltip")


Paste your event into the box, and make sure to find and replace all instances of single quotes with double quotes to make it a valid JSON object.



<p id="gdcalert58" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image58.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert59">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image58.png "image_tooltip")


Also, make sure to convert any **True** values to **“True”**, again to convert it to a valid JSON document. Once it checks out, save it and you can use these test events in the future for any changes you implement in your code. Just make sure to vary the alertId by changing one or two numbers, otherwise you will get the duplicate alert message.



<p id="gdcalert59" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image59.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert60">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image59.png "image_tooltip")

