#### DevOps Journey at Adidas

Fernado Cornago - VP, Platform Engineering - Adidas

Daniel Eichten - VP, Enterprise Architecture, Adidas

---

Slides: TBC

Video: [DevOps Journey at Adidas](https://vimeo.com/showcase/7273701/video/431737448)

---

##### Introduction

Team adidas comes back this year to describe the consolidation or DevOps and SRE practices across the whole IT Department, being now renamed as Technology.

Fernando Cornago, who has taken more responsibility and whose scope is extending towards Cloud and Connectivity, brings this year Daniel Eichten. Heading up Enterprise Architecture, Daniel will talk about adidas’ Cloud and Data Strategy.

Last but least, gamification is always a topic at adidas, we’ll see how this gets implemented all over business and tech.

---

##### Notes

* 400 million lines of code at Adidas
* Product led organization at heart
* Three different tech product types
  * Experience product (Customer journey etc)
  * Core Products (Pricing, Payment, Fulfillment, Order Management)
  * Platform products & services
* Platform engagement model (Enabling, Collaborating & as a service)
* Platform as a product
* Changed the name of the team from IT to Technology
* Doubled down on ecom - 4.7bn - 30%-40% yoy due to COVID-19
  * Increased demand causes system outages 
  * Lost around 1 million in revenue per month directly related to P1 outages
* Beyond SLOs
  * Mean time to restore from DR
  * Mean time to detect to DR 
  * Revenue Loss
  * Count of Service Interruptions
* Secret key to avoid vendor lock in
  * Pick lock ins "that we love"
    * Sometimes push standards
    * Knowledge is widely avaliable
  * Exit strategy (Bolt cutters)
    * i.e move away from a lock-in by just rewriting it in the other provides
* Cloud providers they use (multi-cloud)
  * AWS
  * Azure
  * GCP
  * Also run their own DC for data they can't put on the cloud due to governance
* Access 
  * GitOps for users on AWS
    * "Bitbucket is integrated into Azure AD for SSO. And then a linked account request is basically one file. Yaml/Json depending on your preference. If you wanna change you only change the file. PR goes in and the guys sitting on top of aws review. Rest is then automated filling terraform templates or CDK scripts."
  * GCP + Azure all keys to the castle, but has a watchdog!
    * [Cloud Infrastructure Security, AWS Security Monitoring - Dome9](https://dome9.com/) - Watchdog

---

##### Takeaways

* The Platform engagement model could be useful if for things split between two teams to define ownership across teams
* "You don't want to be the bottleneck"
* [GitHub - adidas/adidas-devops-maturity-framework: The DevOps maturity framework was created by adidas as a guide for the first DevOps cup to support the teams on their DevOps transformation journey.](https://github.com/adidas/adidas-devops-maturity-framework)
* [Cloud Infrastructure Security, AWS Security Monitoring - Dome9](https://dome9.com/)
* On how they manage access to AWS
  * "Bitbucket is integrated into Azure AD for SSO. And then a linked account request is basically one file. Yaml/Json depending on your preference. If you wanna change you only change the file. PR goes in and the guys sitting on top of aws review. Rest is then automated filling terraform templates or CDK scripts."
