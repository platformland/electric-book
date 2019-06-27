# Measuring and monitoring

Because the primary users of a platform tend not to be the public themselves, but rather the people who use them to create services for the public, platform teams need to understand both what _they_ need to measure to operate the platform, and what their _users_ need to provide services to the public. Ultimately, the success of a platform will be perceived by the success of those services, not the platform itself.

## 1. Understand what data your team needs

The team operating the platform will have clear a set of needs that relate to the operation and improvement of the platform. These may include some of the following:

* Are people self-serving? (For example what's the ratio of meetings to users?)
* Are people using the documentation?
* What code libraries are being used?
* Where are the users (central government, local government, private sector?)
* How many distinct services and organizations are using the platform?
* What is the service up-time?

If you are operating a platform, conduct user research with your team and understand what data they need to do their job effectively.

## 2. Understand what data your users need

Because platforms are component parts of services, the success of a platform will ultimately be perceived by the success of those services. As such, it is critical to understand what data your users will need access to as part of the operation of their service. Google, for example, maintains specific tools to help Android developers understand app performance.[^1]

Much of the data users need may be domain specific, so conduct user research with them to understand their needs.

## 3. Measure cost-per-use (even if you don't charge)

Measure cost-per-use and be transparent to users of the platform or register, even if they are using the platform or register for free. This is particularly important in case you need to pivot the funding model at some point in the future.

## 4. Publish performance data in the open

Italy's Team per la Trasformazione Digitale publish data about the rollout of the National Resident Population Register, including register size and the number of municipalities that have migrated to it.[^2] India's Aadhaar and Estonia's X-road both have public dashboards that show usage.[^3][^4] The UK's GOV.UK Pay publishes data about the organizations using it and the value of the payments that it has processed.[^5]

## 5. Prepare for unexpected user behaviour

It is in the nature of a 'true' platform that you don't know exactly how people will use your platform or when they will use it. If someone is going to do something new with your platform, they will likely not tell you in advance. This is especially true if you have designed for self-service. As such, you should also aim to understand the roadmaps of any large services making use of your platform so you can better anticipate their usage. You can also use analytics to understand emerging use-cases for the platform.

## 6. Create a public system status page

It is standard practice for commercial platforms to maintain a status page (often on a separate web domain) that detail the current status of the system.[^6] Many digital service units are following this practice with the UK, Australia and US (among others) maintaining status pages.[^7] [^8] [^9]

## 7. Publish incident reports

It is also standard practice for commercial platforms to publish public incident reports detailing any outages or security issues. [^10] 

## 8. Use the privileged position of the platform (respectfully)

Platform operators have the power to look across the platform and see how it is being used. e.g. looking for patterns in implementation that can be generalized into features or used to improve how other users use the platform.

With great power comes great responsibility - there may be legitimate cases for making this essentially technically impossible (e.g. GOV.UK Verify being blind to the services that someone was using)

> ## Example: Monitoring and tooling for Android
> 
> "Google maintains specific tools to help Android developers understand app performance and respond to issues."
> 
> "The dynamic is that whatever you do with your platform, you are perceived through the lens of the applications that run on it, so you need to provide tooling as well as APIs."
> 
> "We have a tonne of reporting that's built into the platform. If an application crashes, the system shows a dialogue: "Send report?" --- with user permission, it'll send back anonymized (non-personally identifiable) system information to the core team (so we can debug our platform) and it'll send it to the app developers so they are aware of issues. A bunch of energy is invested in Play Developer Console where we give developers a tonne of metrics & tools to help them improve their applications."
> 
> — Dr Adam Connors, Senior Google Engineering Manager
{:.box}

[^1]:   Google, "Google Play Console", [https://developer.android.com/distribute/console](https://developer.android.com/distribute/console). Retrieved 9th June 2019.

[^2]:   Team Digitale, "National Resident Population Register (ANPR) - Digital Transformation Team", [https://teamdigitale.governo.it/en/projects/anpr.htm](https://teamdigitale.governo.it/en/projects/anpr.htm). Retrieved 9th June 2019.

[^3]:   UIAI, "Aadhaar Dashboard", [https://uidai.gov.in/aadhaar\_dashboard/](https://uidai.gov.in/aadhaar_dashboard/). Retrieved 9th June 2019.

[^4]:   "X-TEE", [https://www.x-tee.ee/factsheets/EE/#eng](https://www.x-tee.ee/factsheets/EE/#eng). Retrieved 9th June 2019.

[^5]:   HM Government, "Dashboard, GOV.UK Pay,  GOV.UK", [https://www.gov.uk/performance/govuk-pay](https://www.gov.uk/performance/govuk-pay). Retrieved 9th June 2019.

[^6]:   For examples see: [https://status.twilio.com](https://status.twilio.com), [https://www.gocardless-status.com](https://www.gocardless-status.com), [https://status.aws.amazon.com](https://status.aws.amazon.com) and [https://status.stripe.com](https://status.stripe.com)

[^7]:   "GOV.UK Pay Status", [https://payments.statuspage.io](https://payments.statuspage.io). Retrieved 9th June 2019.

[^8]:   "cloud.gov.au Status", [https://status.cloud.gov.au](https://status.cloud.gov.au). Retrieved 9th June 2019.

[^9]:   "cloud.gov Status", [https://cloudgov.statuspage.io](https://cloudgov.statuspage.io). Retrieved 9th June 2019.

[^10]:  See [https://aws.amazon.com/message/41926/](https://aws.amazon.com/message/41926/) and [https://gocardless.com/blog/incident-review-api-and-dashboard-outage-on-10th-october/](https://gocardless.com/blog/incident-review-api-and-dashboard-outage-on-10th-october/) for examples "
