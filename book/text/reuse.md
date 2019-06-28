# Reuse

Not everything needs to be built from scratch.
Reusing existing platforms from other governments can reduce development time. And putting wrappers around commercial commodity services can allow for the use of commercial offerings with less risk of lock-in or loss of control.

## 1. Borrow from other governments (and celebrate it)

While government platforms are a relatively new thing, there are some opportunities to reuse the work of other governments. This includes reusing entire platforms, learnings from user research, guidance and standards.[^1]

One example of this is the Digital Transformation Agency in Australia reusing the UK's GOV.UK Notify messaging platform.[^2] Because the code was open-source, developers were able to quickly evaluate and set up their own implementation.[^3] Another example is the reuse of analytics.gov by city and state governments across the US.[^4]  

(Increasingly there are projects and organizations being created with the explicit aim of fostering more of this kind of sharing, these include the MOSIP identity project, and the Nordic Institute of Interoperability Solutions.)

During the discovery phase of a platform project, understand what other governments might have approached this problem before. Try contacting the teams and asking for advice.

## 2. Put wrappers around commercial, commodity components

In some instances, there may be commercial components available on the market that could be used as part of a platform ecosystem - for example, cloud hosting or digital payment providers. Creating thin wrappers around these can minimize the risk of lock-in, maintain control over the user experience and enforced standards.

In the US, Cloud.gov is built on top of Amazon Web Services, and meets the standards set by FedRAMP (a standard approach to security governance across the US federal government).[^5]

This approach may also open up new opportunities to manage demand and build robustness into the system. In the UK, GOV.UK Pay supports multiple payment providers and GOV.UK Notify awards contracts to multiple SMS gateways.[^6][^7]

This is approach is unlikely to work if the components are not true commodities. Use Wardley Mapping to help understand if potential components are commodities or not.[^8]

[^1]:   See [https://www.platformland.org/mapping/](https://www.platformland.org/mapping/) for lists of platforms, standards and design systems.

[^2]:   DTA, "govau/notify", GitHub, [https://github.com/govau/notify](https://github.com/govau/notify). Retrieved 25th June 2019.

[^3]:   Interview

[^4]:   Melody Kramer, "Tips for adapting analytics.usa.gov from Tennessee, Boulder, and Philadelphia", 18F Blog, 6th January 2016, [https://18f.gsa.gov/2016/01/06/tips-for-adapting-analytics-usa-gov/](https://18f.gsa.gov/2016/01/06/tips-for-adapting-analytics-usa-gov/)

[^5]:   "What is cloud.gov?", [https://cloud.gov/overview/overview/what-is-cloudgov/](https://cloud.gov/overview/overview/what-is-cloudgov/). Retrieved 24th June 2019.

[^6]:   HM Government, "GOV.UK Pay’s Payment Service Provider", [https://www.payments.service.gov.uk/payment-service-provider/](https://www.payments.service.gov.uk/payment-service-provider/). Retrieved 24th June 2019.

[^7]:   Mark Say, "GDS awards SMS firms GOV.UK Notify contracts", UKAuthority, 30th January 2019, [https://www.ukauthority.com/articles/gds-awards-sms-firms-govuk-notify-contracts/](https://www.ukauthority.com/articles/gds-awards-sms-firms-govuk-notify-contracts/)

[^8]:   Simon Wardley, "How commodity is something?", Bits of Pieces?, 15th September 2015,  [https://blog.gardeviance.org/2015/09/how-commodity-is-something.html](https://blog.gardeviance.org/2015/09/how-commodity-is-something.html)
