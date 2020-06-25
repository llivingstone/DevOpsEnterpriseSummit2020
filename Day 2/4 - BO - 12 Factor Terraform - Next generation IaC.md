#### 12 Factor Terraform: Next Generation Infrastructure As Code

Richard Vodden - Head of Cloud Engineering, Babylon Health

---

Slides: TBC

Video: TBC

---

##### Introduction

Babylon’s mission is to put an accessible and affordable health service in the hands of every person on earth. In order to do this, we need to be able to deploy quickly, effectively, and with total confidence in success. The 12 Factor App is old news as far as software development is concerned, and countless firms have achieved great success in applying its principles. At Babylon we’ve gone a step further and have applied 12-factor principles to our IaC pipeline, and extended the concept of a microservice down to the infrastructure layer. This means that our delivery teams are empowered to deploy their own infrastructure and innovate around it, whilst maintaining our confidence that we can allocate cost correctly, that we remain compliant with our internal and external standards, and that we are delivering as fast as we possibly can.

---

##### Notes

* Terraform isn't special, it's just another programming language
* What are we trying to solve?
  * Remove bottlenecks
  * Increase Pace
  * Ensure Consistency
  * Enforce Compliance
* Big challenges running terraform in 12 pillars format
  * Seperate build, release and run
  * Factor shared code into libraries which can be included through the dependency manager
  * Explicity declare and isolate dependencies
  * Store configuration in the environment
* Versioning terraform modules/librarys
* Four layer hierarchy
  * Environement 
  * Service 
  * Component
  * Module
* Testing
  * Environment = Production testing, runscope api testing, regularly run a plan
  * Service = End to End Test: deploy the infra and the app and run the app test suite
  * Component = Integration tests: Can i get the creds for the db out of vault? etc
  * Module = Unit tests: Does th resourse deploy, does it have the correct tasgging, have the opinions we had about it be applied?
* 

---

##### Takeaways

* Beroku - Dependancy manager for terraform
