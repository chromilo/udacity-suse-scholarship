# udacity-suse-scholarship
These are my notes for the 6 month SUSE scholarship for the Cloud Native Application Architecture. nanodegree The format of the daily check-ins must follow this format:
1. What did I work on yesterday?
2. What will I work on today?
3. What issues are blocking my progress?

For the study teams, we post using this format:
1. What did your Study Team work on or participate in last week?
2. What are your plans for this coming week? 
3. Are you facing any challenges or blockers? 

---
Day 63:
1.  Yesterday and the days before, I submitted project 4 and passed on the second try. Yay.
2.  Today I submitted some of the projects from career services. Had my resume, Github, and LinkedIn reviewed and graded. I also graduated today and received my certificate. So proud of this one.  https://confirm.udacity.com/WCERFPLC
![CNAA-certificate](https://user-images.githubusercontent.com/75153964/143979576-e09e10cc-76fb-4f95-9cde-fcef48079017.JPG)  
3.  Busy with Georgia Tech final exam review for actual exam on Dec 9.
---
Day 62:
1.  Yesterday and the days before, I completed up to lessons 6.12.
2.  Today I completed all the lessons for Hardened Microservices Environment. Enjoyed this lesson more than the past two. Instructor was easy to understand and demos were systematic. Progressing along with project, fixed my issue running helm from SUSE vm. Working on docker-bench again and hardening the environment. Going at it hard on my own and hoping to submit it this weekend so I can concentrate on my Georgia Tech lessons starting Monday. Currentl behind 3 lessons there.
3.  Busy with Georgia Tech final exam review for actual exam on Dec 9.
---
Day 61:
1.  Yesterday and the days before, I completed lessons 4-5.25.
2.  Today I completed up to lesson 6.12. I had issues installing the falco driver. Knowledge shows some options so had to redo my RKE cluster to try a few things. It seems a little bit harder to do this on Windows 10 host. I believe my issue is with running the "helm install --kubeconfig kube_config_cluster.yml falco falcosecurity/falco --set falco.grpc.enabled=true --set falco.grpcOutput.enabled=true" command from inside the SUSE Linux vm as it is trying to "ssh root@192.168.50.101" which is not a valid IP when I'm on the vm itself. Still working on it.
3.  Busy with Georgia Tech final exam review for actual exam on Dec 9.
---
Day 60:
1.  Yesterday and the days before, I completed and passed project 3. Started with lessons 1-3 of Hardened Microservices Environment.
2.  Today I completed lessons 4 up to 5.25. Also finished design drawing, loaded RKE cluster, ran kube-bench out of box scan, ran docker-bench out of box scan, grype out of box and hardened scans. Seems easy so far. With 7 days left before end of term, anyone interested in partnering up for a last push on project 4? I'm available after 5pm Pacific for a one-hour session over Teams. 
3.  Busy with Georgia Tech final exam review for actual exam on Dec 9.
---
Day 59:
1.  Yesterday and the days before, I submitted my last Georgia Tech project with partner Luis. Many 2am sessions for this one.
2.  Today I completed the Observability project, submitted it twice for review by graders, and passed it on second try. Yay! Also today, I finished lessons 1-3 including reading about the project requirements for the Hardened Microservices Environment project. With only 8 days left before end of term on Dec 2, this will be tough. However, I see that we may have an automatic 4-week extension.  
![image](https://user-images.githubusercontent.com/75153964/143086343-afb6d5b2-4bac-4a30-9cbc-6b2f1da1ed21.png)  
3.  Busy with Georgia Tech final exam review for actual exam on Dec 9.
---
Day 58:
1.  Yesterday and the days before, I submitted my Udaconnect project and passed it after two attempts. Yay! I also placed top 8 in the Kubecon Cup 2021 battlesnake tournament and received $25 from CNCF.
![image](https://user-images.githubusercontent.com/75153964/140273011-ebea5e21-a37d-48cd-ba40-5c1cb1c2fd8a.png)  

2.  Today I completed the Observability prerequisites for the project. I am also now in lesson 4.1 of Tracing. Working to complete these TODO items below listed in README. Posted my updates to my GitHub repo.   
Create a Basic Dashboard - Describe SLO/SLI - Creating SLI metrics - Create a Dashboard to measure our SLIs - Tracing our Flask App - Jaeger in Dashboards - Report Error -Creating SLIs and SLOs - Building KPIs for our plan - Final Dashboard
3.  Busy with work and with Georgia Tech projects. 
---
Day 57:
1.  Yesterday and the days before, I loaded a bitnami kafka container.
2.  Today I attended KubeCon conference, joining I was eliminated in the first stage of the KubeCon Cup battlesnake challenge. I didn't write enough code to avoid hitting other snake. My entry is the one called "Kubecon Cup 2021" in [this video](https://drive.google.com/file/d/1tYvnpSZUqDE-Dof68sFTdY1QHWy1xn1d/view). Posted my updates to my GitHub repo.   
![image](https://user-images.githubusercontent.com/75153964/136861136-05d9a629-321a-4edf-929a-1ba9c637bff7.png)   
![image](https://user-images.githubusercontent.com/75153964/136886410-43a05ea6-9122-4e12-a7b0-f3933fc03d14.png)

3.  Tons of confusion on pods and networking. This is the error I am getting trying to launch my grpc client. It can't seem to connect to grpc server on port 5005 with below error:   
_Sending sample payload...
Traceback (most recent call last):
  File "producer.py", line 17, in <module>
    response = stub.Get(udaconnect_pb2.Empty())
  File "/usr/local/lib/python3.7/site-packages/grpc/_channel.py", line 946, in __call__
    return _end_unary_response_blocking(state, call, False, None)
  File "/usr/local/lib/python3.7/site-packages/grpc/_channel.py", line 849, in _end_unary_response_blocking
    raise _InactiveRpcError(state)
grpc._channel._InactiveRpcError: <_InactiveRpcError of RPC that terminated with:
status = StatusCode.UNAVAILABLE
details = "failed to connect to all addresses"
debug_error_string = "{"created":"@1634009125.663647500","description":"Failed to pick subchannel","file":"src/core/ext/filters/client_channel/client_channel.cc","file_line":3158,"referenced_errors":[{"created":"@1634009125.663646400","description":"failed to connect to all addresses","file":"src/core/lib/transport/error_utils.cc","file_line":147,"grpc_status":14}]}"_

---
Day 56:
1.  Yesterday and the days before, I finished the architecture diagram and started refactoring a branch.
2.  Today I finished loading two pods for two refactored microservices. I have posted below some of my answers to the lesson essay questions for lesson 5. Posted my updates to my GitHub repo. 
3.  Having problems with networking. I got vagrant working before to expose vm to my host via bridging but it doesn't work now.
---
Day 55:
1.  Yesterday and the days before, I got to lesson 5.4.
2.  Today I finished all of lesson 5 and including all the lesson reviews for the Udaconnect project. Will start on the project now. I have posted below some of my answers to the lesson essay questions for lesson 5. Posted my updates to my GitHub repo. 
3.  This is the last week to finish my other AWS ML Foundations challenge course, with last lesson estimated at 6 hours long. Omg.

**How was your experience with integrating a Flask REST API with a Kafka queue? How might integrating a REST API with a Kafka queue be useful in large production systems?**
-I found it very confusing setting up a listener for the broker and a listener for the consumer service on port 9202. The flask server itself was on port 5000 and submitting a POST was a bit confusing because of the multiple listeners involved. For a large production environment, I can see that the zookeeper and Kafka services have to be run as containers on kubernetes cluster. The producer and consumers also have to run as separate pods.

**How might you find OpenAPI useful in your RESTful API implementations? When would it not make sense to use OpenAPI?**
-I think this would work well for python. I don't know what libraries are available to help with inline documentation using OpenAPI if I used another language. It is very helpful for those that observe this practice but many organizations will likely bypass documentation altogether for speed in delivery.

**Once the new endpoints are set, what other parts of the code will we need to modify?**
-The method names also had to be changed after duplicating the endpoint. I appended v2 to the method name. This technical debt needs to be revisited after however, by removing the old endpoint and at that point, also rename the method name removing v2 from it. This seems wrong somehow.

**Choose at least two of the strategies discussed in this lesson and describe how using those strategies would have helped you on an earlier project.**
-I was working on SIEM integration using Kafka beat as a consumer of event logs from various sources. I could have used json to format the output of logs stored in a database table. I could have also used what I learned on OpenAPI using Swagger to see if I could read the format of the syslog input that the kafka beat consumer is expecting from the log sources acting as producers.

**We discussed situations in which these strategies can be useful. Can you think of situations when these strategies would not be useful and would add unnecessary complexity to your projects?**
-The versioning of APIs would double the size of the code if it was made in the same code by duplicating the endpoints. This would entail duplicating the method and renaming the copied method name so that it was unique and didn't conflict with the original method. After go-live, it would be dangerous to have to go back and cleanup the changes to remove the original API methods and rename the new method. To me, it would make more sense to make a version change on the code itself and replace the API version directly. If there were issues, roll back to the previous version of the code.

---
Day 54:
1.  Yesterday and the days before, I got to lesson 4.13.
2.  Today I finished lesson 5.4. I was able to complete the gRPC and Kafka exercises/demos using docker-compose container and vagrant. I had issues getting the readers/writers in a container so ran those from within the vm. Had some issues with installing the grpcio tools initially and issues running the kafka create shell script as it was missing partitions and replication-factor parameters. Fixed those. Do you need to complete lesson 5 prior to starting on the udaconnect project? Posted my updates to my GitHub repo. 
3.  Three lessons behind on my CS 6290 course and two more lesson to go on AWS MLE challenge then assessment quiz. Also trying to get my PHP environment setup for an internship. 
---
Day 53:
1.  Yesterday and the days before, I got to lesson 4.6 and finished Project:Udaconnect lesson 3.
2.  Today I finished lesson 4.13. Running the REST API exercises are harder on Windows, I had to spin up create docker containers for client and server. Also trying to get started on Kafka exercise. Posted my updates to my GitHub repo. 
3.  Spending a lot of time correcting some of the lesson mistakes Matthew G. mentioned. Also trying to spin up a separate linux vm for the Kafka and gRPC exercises.
---
Day 52:
1.  Yesterday and the days before, I got to lesson 4.3.
2.  Today I finished lesson 4.6. I also finished Project:Udaconnect lesson 3. I was able to get all the environment and tools setup ready for project as I am running out of time. I had tons of issues running the seeding script as I run Windows 10 OS. I had to scp the script and db folders to the vm guest and run each line of the run_db_command.sh file separately as the $CT_DB_USERNAME and $CT_DB_NAME environment variables did not get recognized inside the shell script. Got it working though. Posted my updates to my GitHub repo. 
3.  Two endpoints tested ok except for http://localhost:30001/api. 
---
Day 51:
1.  Yesterday and the days before, I got to lesson 3.3.4.
2.  Today I finished lesson 4.3. Posted my updates to my GitHub repo.  
3.  Busy studying for AWS MLE foundations lesson, and GT CS 6290 lesson.
---
Day 50:
1.  Yesterday and the days before, I got to lessone 3.2.14.
2.  Today I finished lesson 3.3.4. Posted my updates to my GitHub repo.  
3.  Busy studying for AWS recertification, AWS MLE foundations lesson, and GT CS 6290 lesson.
---
Day 49:
1.  Yesterday and the days before, I got to lessone 3.1.5.
2.  Today I finished lesson 3.2.14 (Straggler Pattern with Flask Starter code). Posted my updates to my GitHub repo.  
3.  Busy studying for AWS recertification, AWS MLE foundations lesson, and GT CS 6290 lesson.
---
Day 48:
1.  Yesterday and the days before, I started lesson 3 (Message Passing).
2.  Today I finished lesson 3.1.5. I also joined SUSE & Rancher community and signed up for welcome CNA Scholars meetup. Posted my updates to my GitHub repo.  
3.  Just submitted proj0 for my CS 6290 course. That is hard, trying to work with branch predictors.
---
Day 47:
1.  Yesterday and the days before, I finished all of techtrends project except for the second standout suggestion on customizing docker tags with the GitHub actions. I was also able to get a courtesy drop of CS 6300 course which is a big relief. I now still have to pass CS 6290 however.
2.  Today I figured out that I mispelled the tags variable in the GitHub actions workflow manifest. I submitted the techtrends project along with all 3 standout suggestions, and passed it successfully. Posted my updates to my GitHub repo.  
![image](https://user-images.githubusercontent.com/75153964/131765176-d9e66356-c332-4100-9a23-d6606aa582b4.png) 

3.  Catching up on AWS MLE, AWS solutions architect exam, and GT CS 6290 lectures.
---
Day 46:
1.  Yesterday and the days before, I took some time off in Victoria. 
2.  Today I completed UdaConnect project lesson 1.5. Posted my updates to my GitHub repo.
3.  I can't find the correct format for livenessProbe and readinessProbe in deploy.yaml file.
---
Day 45:
1.  Yesterday and the days before I was accepted into the full nanodegree. I also finished up to lesson 5 of the Techtrends project 1. 
![image](https://user-images.githubusercontent.com/75153964/130725382-4b2ff37a-4447-4e67-9f24-e8f76b17e15f.png)  
2.  Today I finished creating the Kubernetes declarative manifest yaml files for Techtrends lesson 6. Posted my updates to my GitHub repo.
3.  Travelling to Victoria all day will cause some delays in my studying.
---
Day 44:
1.  Yesterday I tried a few docker images that will run on Raspberry Pi 3. No luck. The pods on k3s keep erroring out and recycling. I create a MS Teams Together view of the #st_canada members who have profile headshots available. I also updated our final #st_canada meeting minutes document here.
![image](https://user-images.githubusercontent.com/75153964/127928646-81d631ae-8a0d-4ba6-b6b5-bf9c1ad5f631.png)

2.  Today I tried [balenalib/raspberry-pi-alpine-golang:latest image](https://hub.docker.com/r/balenalib/raspberry-pi-alpine-golang) and that worked. The pods are running yay! I must have tried over 5 different images before landing on this one. This isn't easy. Posted my updates to my GitHub repo.
3.  I can't seem to access the go-helloworld app via http://192.168.0.1:6112 from my host computer. Trying to run it locally on the RPi via http://127.0.0.1:6112 is exteremly slow and I fear it might be resource constrained.

---
Day 43:
1.  Yesterday I received my Okta Certified Professional badge from Credly.

[![image](https://user-images.githubusercontent.com/75153964/127759621-6ace7aef-ad75-4093-a44c-014ecdf8d4c3.png)](https://www.credly.com/badges/f496e755-b3be-4534-abe3-b91f9dd16135)

2.  Today I was a speaker at Conclave21 from 9:30am-10:30am Pacific where I covered AI for Robotics. Here is a [recording](https://drive.google.com/file/d/1SPVcu-00Vkhv-4wyn4JVjAdkcmokiUqV/view), many thanks to @RohitBhardwaj and team for organizing [Conclave21](https://sites.google.com/view/suse-conclave-21/). I also setup our final Study Buddy meetup with @Barry.Pratt who has now fully completed the course. Posted my updates to my GitHub repo.
3.  Got some help on a possible docker image type for golang alpine go-helloworld app on an RPi 3. Just need some time to try it out.
---
Day 42:
1.  Yesterday I studied for my Okta exam. I submitted the final tally of #st_canada members who completed the course.
2.  Today I took the Okta Certified Professional exam and passed. I'll get the total breakdown via email soon but I believe I was very close to not passing. Hate DOMC (Discrete Option Multiple Choice) style of question for exams. I attended the end party Zoom call and posted my updates to my GitHub repo.
3.  Got some help on a possible docker image type for golang alpine go-helloworld app on an RPi 3. Just need some time to try it out.

#reflect
1.  Looking back at your original motivation and goals, how did you do?  
I did fairly well. I saved my original motivation and goals on my Github blog so I can refer back to it. I said that I was all over the place with my plans wanting to finish my Udacity/Bertelsmann AI Program Manager nanodegree, study for the AWS ML phase 1 challenge, get AWS Solutions Architect recertified, and get Okta Certified Professional certified before fall 2021 semester starts at Georgia Tech. I was able to get my AI Program Manager certificate and just passed my Okta Certified Professional exam tonight.

2.  Were you on track for what you expected and hoped for? (If not, what would you want to try next time to get there?)  
It's already August next week and my classes at Georgia Tech start August 23, 2021 which leaves me with less than 3 weeks to finish the AWS ML phase 1 challenge and get my AWS Solutions Architect recertification. Slack definitely contributed to my procrastination and having too many tabs open on my browser. I'll try and have one app or tab open at one time to stay focused.

3.  What helped you succeed and stay motivated/succeed thus far? (Did anything surprise you about this process?)  
Nothing surprised me this time around as it is my second scholarship challenge. Although Slack was my downfall, it was also my saving grace as I used it along with LinkedIn messenger to stay in touch with current and past Udacity scholar to stay motivated. Socializing my successes and/or failures on Slack kept me honest and accountable, which helped me complete 3 out of 5 goals I wanted to complete at the start of this challenge.
---
Day 41:
1.  Yesterday I booked my Okta exam and lesson 11, skipped the Okta Udemy course. What a waste of $35 on a course, the trainer does not know how to teach. Instead of useless Udemy course I went through all the Okta materials and practiced on oktapreview.com tenant.
2.  Today I counted all members who have not completed the course and on the worst case, there are 40/64 who still have not finished. Continued studying for my Okta exam. Posted my updates to my GitHub repo.
3.  Got some help on a possible docker image type for golang alpine go-helloworld app on an RPi 3. Just need some time to try it out.
---
Day 40:
1.  Yesterday I finished lesson 11, skipping lesson 12 (python), finished lesson 13 of Okta Udemy course. I also took the free sample exam from the site. I started updating our tracking list to figure out who in #st_canada is done with Cloud native course by scouring through slack any updates from members.
2.  Today I will book my Okta exam and continue studying. I submitted an EasyPoll to #st_canada channel to get a sense of who has finished the course so we can win the highly coveted Study Team Competition award for this coming Wednesday July 28. Posted my updates to my GitHub repo.
3.  Still no help on finding correct docker image type for golang alpine app that will work on an RPi arm.
---
Day 39:
1.  Yesterday I finished lesson 3 fron the Okta course on Udemy.
2.  Today I finished lesson 9 from the Okta course. Posted my updates to My GitHub repo.
3.  Still no help on finding correct docker image type for golang alpine app that will work on an RPi arm.
---
Day 38:
1.  Yesterday I met with @Barry.Pratt for our Study Buddy meetup. I finished lesson in Users for the Okta course on Udemy.
2.  Today I continue on the Okta course. Posted my updates to My GitHub repo.
3.  Still no help on finding correct docker image type for golang alpine app that will work on an RPi arm.
---
Day 37:
1.  Yesterday I finished AWS ML lesson 2.5. Spent some time troubleshooting golang alpine images that will run on my RPi 3. I also participated in a 2 hour Okta Professional Certification Exam Prep webinar. Received a $50 voucher good until September.
2.  Today I purchased a Udemy course Okta from zero to hero course in preparation for exam. I also filled out form for a student-led initiative for next week. Posted my updates to My GitHub repo.
3.  None.  
![image](https://user-images.githubusercontent.com/75153964/126847601-a402ebb3-8467-4167-9643-57315d3e6ee9.png)
---
Day 36:
1.  Yesterday I finished AWS ML lesson 2.4 and started lesson 3 exercises again but on Raspberry Pi 3.
2.  Today I updated our #st_canada tracking spreadsheet. Fixed issue installing and running k3s on RPi. Posted my updates to My GitHub repo.
- modify /boot/cmdline.txt to add cgroup_enable=cpuset cgroup_enable=memory cgroup_memory=1
- reboot
- Load version 0.9.1 as that is compatible with RPi 3+, by running "curl -sfL https://get.k3s.io | INSTALL_K3S_VERSION=v0.9.1 sh"
3.  None.

#st_canada
1.  What did your Study Team work on or participate in last week?   
Our study team met for our weekly session July 16 at 3:30pm Pacific. Meeting minutes are here. We participated in Study Jam over the weekend (I recognized a few from our group there), and we completed an Easy poll showing that out of 13 who filled out the poll, three scholars are still in lesson 4 and four in lesson 5.
2.   What are your plans for this coming week?  
Tally up the scholars on sprint 2 walls. Our tracking spreadsheet is here. We found the following stats:
20/63 scholars are on the sprint 2 wall but have not filled out the sprint 2 completion form, most likely because they are not done with lessons yet.
15/63 scholars have submitted the sprint 2 completion form, most likely completed all lessons.
Meet with more members this Friday July 23 to get updated stats.
3.   Are you facing any challenges or blockers?  
28/63 scholars have NOT submitted the Sprint 2 completion forms yet.
---
Day 36:
1.  Yesterday I attended docker compose workshop by @badr.ibrahim. I finished AWS ML lesson 2.2
2.  Today I completed the sprint 2 completion form, filled out the Study Buddy form, filled out the Blogathon form, and I finished AWS ML lesson 2.4. Posted my updates to My GitHub repo.
3.  None.
---
Day 35:
1.  Yesterday I graduated from my AI Program Manager.
2.  Today I attended docker compose workshop by @badr.ibrahim. I finished AWS ML lesson 2.2. Posted my updates to My GitHub repo.
3.  None.
---
Day 34:
1.  Yesterday I resubmitted my AI capstone project.
2.  Today I graduated from my AI Program Manager nanodegree and received certificate that I worked hard to get close to 7 months.   
![image](https://user-images.githubusercontent.com/75153964/126076980-3ceaa06d-f797-43cd-9ee8-fbf98fe2d30a.png)  

Attended some events for Study Jam 1.0. Co-host Bingo Baker event with @Rohit.Roy.Chowdhury. Host Jackbox game night later today July 17, 2021 from 10-11pm Pacific in the #wellness channel. 

Bingo Baker  

![image](https://user-images.githubusercontent.com/75153964/126076865-e92bc9b1-feaa-4a7d-96bd-9c5ced5cbf8d.png)

Game Night  

![image](https://user-images.githubusercontent.com/75153964/126076882-967741df-758f-4095-b565-9caaced156fb.png)

Posted my updates to my Github blog.

3.  None.
---
Day 33:
1.  Yesterday I submitted submitted 3 quizzes with answers to @James for a quiz event.  
2.  Today I resubmitted my AI capstone project. We also met for our weekly meetup with #st_canada. Submitted my t-shirt logo to @ElizabethWotawa. Finalized and posted our Bingo Baker study jam event with @Rohit.Roy.Chowdhury. Posted my updates to my Github blog.
https://github.com/chromilo/udacity_suse_project_tshirt/blob/master/tshirt_designs/cicd-chromilo.amin.png
![image](https://user-images.githubusercontent.com/75153964/126076929-66779d92-d380-4b89-8061-e94fac813dc2.png)
3.  None.
--- 
Day 32:
1.  Yesterday I submitted my AI capstone project and got 7 wrong.
2.  Today I fixed 2/7. I submitted 3 quiz items to @James for our group #st_canada to get involved in a community quiz event. Posted my updates to my Github blog.
3.  A bit anxious with some reorganizations happening at work recently. Losing energy a bit.
---
Day 31:
1.  Yesterday I submitted all Udacity career services project perks.
2.  Today I submitted my AI capstone project and received feedback from Udacity mentors, with 7 points to revisit. Prepared poster for Game Night for study jam and other event I am co-hosting with @Rohit.Roy.Chowdhury. Posted my updates to my Github blog.
3.  None.
---
#st_canada
1.  What did your Study Team work on or participate in last week?  
Our study team met for our weekly session July 9 at 3:30pm Pacific. Meeting minutes are here. An additional meetup was scheduled over the weekend for a 1:1 help with lesson 5.12 exercise.
2.   What are your plans for this coming week? 
Tally up the scholars on sprint 1 and sprint 2 walls. Our tracking spreadsheet is here. We found the following stats: 26/54 have submitted Sprint 2 commitment form so far. 28/54 (51.8%) have NOT submitted the Sprint 2 commitment form. Meet with more members this Friday July 16 to get updated stats.
3.   Are you facing any challenges or blockers? 
18/54 scholars most likely still not done with lesson 3 yet. Encouraged our members to skip lesson 3 and keep moving to 4 and 5 if stuck. We can always go back to lesson 3. 
---
Day 30 (sprint 2):
1.  Yesterday I finished lesson 5. Yay!
2.  Today I submitted my cover letter career services projects. I submitted an event to host for SJ to organizers, waiting for approval. Posted my updates to my Github blog.
3.  None.
---
Day 29 (sprint 2):
1.  Yesterday I finished lesson 5.15.
2.  Today I completed all of lesson 5 and quickly went over all lessons to ensure I answered all quizzes. Posted my updates to my Github blog.
3.  I received an email alert from Gitguardian saying I may have exposed an RSA Private Key. I just deleted it from my repo. Do you use GitGuardian to watch your repos? Received some mentor feedback on my Github profile review so I have to incorporate some of those feedback. 
---
Day 28 (sprint 2):
1.  Yesterday I was at lesson 5.13.
2.  Today I finished lesson 5.15. Posted my updates to my Github blog.
3.  Procrastination by working on my cover letter project review.
---
Day 27 (sprint 2):
1.  Yesterday I started with lesson 5.12. I was getting sync error "field is immutable" with lesson 5.13.
2.  Today I fixed lesson 5.13 with help from @Rohinton.Kazak. I am now able to sync nginx-alpine app via ArgoCD. Posted my updates to my Github blog.
3.  Procrastination by submitting my GitHub project review to Udacity career services.
---
Day 26 (sprint 2):
1.  Yesterday I finished lesson 5.9.
2.  Today I completed lesson 5.12, at ArgoCD solution. Posted my updates to my Github blog.
3.  Unable to sync nginx-alpine app via ArgoCD. Getting sync error "field is immutable". Need help.
---
Day 25 (sprint 2):
1.  Yesterday I finished lesson 5.3.
2.  Today I completed lesson 5.9 on CD Fundamentals. Posted my updates to my Github blog.
3.  All over the place with other challenges and studies.
---
Day 24 (sprint 2):
1.  Yesterday I finished lesson 5.2.
2.  Today I started with lesson 5.3 videos. Posted my updates to my Github blog.
3.  Slack is such a great place to slack off unfortunately for me. 

#st_canada
1. What did your Study Team work on or participate in last week?  
Our study team met for our weekly session July 3 at 10:00am Pacific (rescheduled). Meeting minutes are here. A final poll was sent out asking for status on lessons. 
2. What are your plans for this coming week?   
This week we Updated the tracking spreadsheet matching team members to sprint 1 wall. We found that 17/52 did not fill out the sprint 1 commitment form; 14/35 have not filled in the sprint 1 completion form so they probably have not finished lesson 3; which means 21/35 or 60% have completed lesson 3.
3. Are you facing any challenges or blockers?   
@James has issues doing the Docker exercise because his laptop PC doesn't support virtualization technology. @moor and @Raphael also said they had some issues but haven't heard back.
---
Day 23 (sprint 2):
1.  Yesterday I finished all of lesson 4.
2.  Today I finished lesson 5.2. Posted my updates to my Github blog.
3.  Work is a little busy today.
  
#reflect
1. How are you doing so far in this course and community in relation to your original motivation?  
Since the start, I have been all over the place, excited to drink in all these scholarships and certifications (AI Program Manager ND, AWS ML challenge, AWS recertification, Okta certification) before fall 2021 semester starts. Nothing has changed, I am still all over the place, still excitedly drinking in all the learnings.

2. Are you on track/what you expected and hoped for? If not, what can you do to get there?  
Not where I wanted to be. Slack seems to contribute to my procrastination and don't know how to get around that. I need to do my own daily_scrum for the other items I am trying to complete outside of this foundations course but because I cannot post here, those are falling behind. With regards to this course, I am ahead of schedule.

3. What has helped you succeed and stay motivated/succeed thus far?  
My study team #st_canada has provided the hand-holding needed to get past demo exercises from lesson 3 and 4. Priceless to have such talented scholars there.
---
Day 22 (sprint 2):
1.  Yesterday I took some time off to procrastinate.
2.  Today I finished all of lesson 4, hurrah! Posted my updates to my Github blog.
3.  Spent a bit of time counting #st_canada scholars who are not in the #daily_scrum wall, or on the wall but without stars beside their names. I also spent some time working on career services project GitHub review. A lot of time spent outside of actual lessons.
---
Day 21:
1.  Yesterday I completed lesson 4.11.
2.  Today I took some time off from lessons to take my kids to their first vaccine shot. Posted my updates to my Github blog.
3.  Procrastination.
---
Day 20:
1.  Yesterday I completed lesson 4.9.
2.  Today I got to lesson 4.11 and was able to complete the demo exercise deploying python-helloworld to IBM Cloud Foundry. I also finished the SUSE survey and my Student Story. Posted my updates to my Github blog.
3.  I spent some time in AWS ML challenge, now at lesson 1. I also have to spend some time with Udemy ACloudGuru AWS course, and purchase Okta zero-to-hero course. More time vortex.
---
Day 19:
1.  Yesterday I celebrated Canada Day so skipped lessons.
2.  Today I was able to get to lesson 4.9 and signed up for an IBM Cloud Foundry account. Working on finishing the exercise and the demo. Posted my updates to my Github blog.
3.  Using IBM Cloud Foundry interface, I don't know how to create the python-helloworld application using public Github as shown in demo. Help!
---
Day 18:
1.  Yesterday I finished lesson 4.6.
2.  Today I celebrated Canada Day by going biking with family. Posted my updates to my Github blog. 
3.  Procrastination.
---
Day 17:
1.  Yesterday I finished lesson 4.5.
2.  Today I finished lesson 4.6 working on 4.7 still. Posted my updates to my Github blog. 
3.  SUSE Cloud Application Platform is deprecated so what can I use instead for the upcoming exercise?

#st_canada
1. What did your Study Team work on or participate in last week?  
A member posted a quiz to complete a couple of questions for group to answer. A few members met on Friday June 25 to help with lesson 3 blocks. Easypoll finished on Monday indicating 7/17 completion of lesson 3.  
2. What are your plans for this coming week???  
Meet again Friday July 2 at 3:30pm PST with members. Started new easypoll that ends Sunday. Resubmit study team competition form if poll improves on Sunday. Grab ideas from members via padlet or remind members of upcoming deadlines.  
3. Are you facing any challenges or blockers???  
17/52 completed poll so need more interaction. Slack does not notify members when meetings come up. No access to @channel or @here.  
---
Day 16:
1.  Yesterday I finished lesson 4.5.
2.  Today I finished lesson 4.7. Posted my updates to my Github blog. 
3.  Started looking at AWS ML classroom. Oh boy here we go.
---
Day 15:
1.  Yesterday I finished lesson 3.
2.  Today I made it to lesson 4.5 exercises. Submitted student team group competition form. Posted my updates to??my Github blog. 
3.  Orientation for AWS ML scholarship start on Tuesday June 29, 2021 so will figure out after that what my blockers are. Plus it is too hot to study right now.
---
Day 14:
1.  Yesterday it was too hot to do any work so I watched some EUFA Euro2020 soccer between France and Portugal. Great game.
2.  Today I finished lesson 3. I jnew taking some time at church mass for wellness would give me the drive to push through. Posted my updates to my blog.
3.  Classes for AWS ML scholarship start on Monday June 28, 2021 so don't know what to do here...
---
Day 13:
1.  Yesterday I made it to lesson 3.23. Held our weekly meetup with #st_canada. Meeting minutes are here.
2.  Today I took some time off. Updated my blog of daily scrum tasks.
3.  Received AWS ML scholarship starting on Monday June 28, 2021.
---
Day 12:
1.  Yesterday I made it to lesson 3.17. Also got the fever from my second moderna shot.
2.  Today I started with lesson 3.22. Working to finish lesson 3.23 exercise. Had our weekly meetup with #st_canada and they helped resolve my issue accessing port 6112 on VM from host. I just needed to add "--address 0.0.0.0" in my port-forward command to have container listen on all ports. Also keeping blog of my daily scrum tasks. 
3.  Received AWS ML scholarship starting on Monday June 28, 2021 so that will take some kung fu skills to manage along with this challenge.
---
Day 11:
1.  Yesterday I made it to lesson 3.16, spending tons of time troubleshooting networking between vm and host.
2.  Today I started with lesson 3.17. Working to finish the exercise. Also keeping blog of my daily scrum tasks
3.  I got sick with the fever after taking my second moderna shot. Hope to feel better tomorrow.
---
Day 10: 
1.  Yesterday I made it to lesson 3.12 KuberConfig walkthrough, working to install Kind cluster.
2.  Today I installed Kind cluster in Windows and K3s inside the VirtualBox VM running Linux, completing lesson 3.16. 
3.  I couldn't connect to my Linux VM from my Windows 10 host to be able to test launching the apps from browser. I bridged the VM network adapter and can ping the VM guest from my Windows 10 host but I am not able to get to ports 6111 or 6112 ports. I got it to work with Kind cluster installed to my Windows 10 computer so I can move forward.

#st_canada  
1. Our study team met for an icebreaker session June 18 at 3:30pm Pacific. Meeting minutes are here. A poll was sent out yesterday asking for status on lessons. This week a member started with weekly quiz challenges for the group.  
2. Update the tracking spreadsheet with everyone's updates and finish lesson 2 for everyone this week. Continue to locate a guest speaker with cloud native experience.
3. There are two scholars facing some issues with lesson 2 but haven't gotten any status back from them yet.
---
Day 9: 
1.  Yesterday I made it to lesson 3.8, publishing to DockerHub registry the two containers from the exercise. 
2.  Today I made it to lesson 3.12 KuberConfig walkthrough, working to install Kind cluster.
3.  I need to prioritize this challenge, an existing AI nanodegree, and two other certifications I need to pass before fall 2021 semester starts at Georgia Tech.
---
Day 8:
1.  Yesterday I did not get to look at lessons. 
2.  I completed submitting both exercises for lesson 3 to DockerHub, all the way to concept 8.
3.  I need to prioritize this challenge, an existing AI nanodegree, and two other certifications I need to pass before fall 2021 semester starts at Georgia Tech.
---
Day 7:
1. Yesterday I watched lessons 3 video.
2. Today I did not get to look at lessons.
3. I need to prioritize this challenge, an existing AI nanadegree, and two other certifications I need to pass before fall 2021 semester starts at Georgia Tech.
---
Day 6:
1. Yesterday I started on lesson 3. I also started with GitHub review lesson from udacity career services ND project.
2. Today I continued watching the lesson 3 videos.
3. Still trying to find a Udemy discount coupon so I can purchase a course currently at CAD$34.99
---
Day 5:
1. Yesterday I finished lesson 2, all concepts.
2. Today I started with lesson 3 concepts. Met with some members from #st_canada at 3:30pm PST. 
3. Still trying to find a Udemy discount coupon so I can purchase a course currently at CAD$34.99
---
Day 4:
1. Yesterday I finished lesson2, concept 10.
2. Today I will continue with lesson 2 concepts using Python Flask. Booked meeting tomorrow for 3:30pm PST for #st_canada . Promoted #st_pinoy_studious trying to get some scholars from Philippines der.
3. Still trying to find a Udemy discount coupon so I can purchase a course currently at CAD$34.99
---
Day 3:
1. Yesterday I finished lesson2, concept 7.
2. Today I will continue with lesson 2 concepts. I also asked st_canada as co-lead/co-organizer if Friday 3:30pm Pacific is a good meeting time this week for an icebreaker.
3. Still trying to find a Udemy discount coupon so I can purchase a course currently at CAD$34.99
---
Day 2 :
1. Yesterday I started with lesson 2 and finished the first quiz in Concept #5; I followed Katie Gamanji on LinkedIn; I joined st_asean,  st_pinoy_studious, st_san_diego_scholars, and st_canada study groups.
2. Today I will continue with lesson 2. I will schedule some time to meet with Barry to see where to help with st_canada as co-lead/co-organizer.
3. Trying to find a Udemy discount coupon so I can purchase a course currently at CAD$34.99
---
Day 1:
1. Yesterday I installed all the prerequisites except for Vagrant.
2. Today I upgraded Vagrant 2.2.9  incrementally, rebooting each time, until I got to the latest version 2.2.16.
3. No blockers.
