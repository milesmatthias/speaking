%title: rails_app_to_api
%author: milesmatthias.com / equityeats.com
%date: 2015-05-10

# About Me

* CTO @EquityEats
* Full stack web and mobile dev
* Rails / JS / iOS / Android 
* miles@equityeats.com / miles.matthias@gmail.com
* @miles_matthias

---

# The proof of concept

* Before I was hired...
* Rails 4.1.8
* Devise
* AWS Elastic Beanstalk
  * (EC2 + ELB + S3 + RDS + deploy script)
  * Auto scaling
* See diagram
* Pros: time to launch, time to dev.
* Cons: scalability & new challenges
  * network traffic costs us money, even random word press scanners.
  * multiple domains (AWS Auto Scaling won't let you add more ELBs to the group after creation)
  * mobile apps

---

# The new architecture

* 


