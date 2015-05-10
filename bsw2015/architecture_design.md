%title: rails_app_to_api
%author: milesmatthias.com / equityeats.com
%date: 2015-05-10

# About Me

* CTO @EquityEats
* Dev track organizer @bldrstartupweek
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

---

# Weigh the pros and cons

* Pros: time to launch, time to dev.
* Cons: scalability & new challenges
  * network traffic costs us money, even random word press scanners.
  * multiple domains (AWS Auto Scaling won't let you add more ELBs to the group after creation)
  * mobile apps

---

# The new architecture

* Rails as just an API
* Thick JS client
* See diagram

---

# Rails as an API
## Authentication

* Override Devise authentication controller
* JWT
* Look at some code.

---

# Rails as an API
## Resources to Endpoints

* Render JSON, not HTML
* Rails resources -> API Endpoints
  * no new, edit, etc.
* Look at old jobs page to identify what the endpoint needs to provide.
* Look at the new jobs page to see it in action.

---

# New Hosting Infrastructure

* EC2 + ELB + RDS
* No auto scaling.
  * Manually monitor usage scaling.
  * Usage scaling will be slow and predictable.
* CloudFront.
  * Handles traffic scaling.
  * Handles annoying scanning.
  * Reduces legitimate API traffic.

---

# Other concerns

* SEO
* Error reporting
* Browser support
  * SSL (SNI / IE on XP)
  * CORS
  * Graceful fallback for unsupported browsers (js & noscript)

---

# Questions?

Feel free to contact me at __miles@equityeats.com__ or __@miles_matthias__



