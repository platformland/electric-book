# Users

It is one of the tenets of user centred design that services should be designed around the needs of users. But, platforms are building blocks, used to create many different public-facing services, so the primary users of a platform tend not to be the public themselves (the end-users of services), but rather the people and organizations who use them to _create services_ for the public. A platform might have users across different tiers of government and non-government organizations.

## 1. Think of platforms as part of many services

If successful, a platform will be part of many public facing services, for example, an API for validating and geocoding addresses might be used in services that let people tax their car, find a hospital, or apply for benefits. As such, a team developing a platform may have only a limited relationship with the end-users of those services, and the public will experience the platform as part of a wider service, not in isolation.

This 'one-to-many' nature of platforms also means that any changes you make to them will affect many different types of user and many different services. This comes with a responsibility to understand the likely impacts of any changes you make and to work in an open way. The teams using your platform need to be able to anticipate changes early and ensure they work for users of their service.  

Conduct joint user research with teams using your platform, so that you can understand how your platform manifests itself in different services. Work in the open and maintain good communications with your users, so you understand how they are using the platform and ensure they understand any upcoming changes.

## 2. Understand _who_ your users are

Because shared components, APIs, registers and identity systems are building blocks of public-facing services, it's important to understand the users of a platform are often not the public (at least not directly). Designing a good platform will require an understanding of their needs, but first you need to identify who they might be. Some important user types to understand include:

* **Developers** wanting to integrate with your platforms quickly and simply.
* **Designers** of a public-facing service who may need to understand how your platform will fit into the broader design of a service, or include it in prototypes they are testing.
* **Procurement managers** who need to understand any contractual or financial arrangements.
* **Administrators** who need to manage the use of the platform, view usage reports or changing their settings.
* **The team developing the platform** who will need to understand how other users are using the platform.
* **The general public** and their representatives who want to understand how you are spending their money and managing public data.
* **Politicians or senior officials** who might have statutory responsibility for your platform or the services using it.

You should identify people and organizations who might use your platform, and understand their needs (remembering that they may not work in government at all and may work in non-technical roles such as procurement).

## 3. Understand _where_ your users are

Looking around the world, government platforms tend to have users in one of three groups:

1. Limited to a single tier of government - for example used by a single state in a federal system, or only by central government.
2. Government-wide - used across central, municipal and regional government.
3. Society-wide - for example, in addition to use in government, a platform is also used in banking, or by third sector organizations and commercial companies.

We can see this if we look at the identity and authentication platforms from the US, UK and India.

Login.gov provides a way to add single-sign-on to digital services, but is limited to US federal agencies.[^1] GOV.UK Verify provides a similar service (albeit with additional levels of identity verification and multiple identity providers) for central government in the UK, but there have also been trials to use it in local government too.[^2] [^3] While in India, the Aadhaar identity platform is used well beyond government services for people to open bank accounts (and not without controversy). [^4]

It is important not to take away from this that ‘the broader the usage the better the platform'. There may be very good reasons for focusing on a subset of institutions early on. There may also be circumstances where a single society-wide platform has too many significant risks associated with it. (Identity is indeed one area where a single, centralized system might be undesirable!)

The key thing to understand is that this is a strategic decision that can be made, and one that can change over time. Who your users are will change too.

> ### Example: Identifying users of Government as a Platform in the UK
> 
> **In the UK, much of the early work of the Government Digital Service had been focused on projects with significant public-facing elements. As the organization began to focus more explicitly on platforms, it had to change how it thought about users:**
> 
> "Many of us joined the Government Digital Service to work directly on things which matter to users. We realized that, organizationally, our job had shifted to meeting the needs of other civil servants, so that they can meet the needs of their users and, as a consequence of that, public services improve and the quality of people's experience of the state is transformed."
> 
> "Citizens are not the only valid users – even GOV.UK itself has a huge number of civil servant users who are using it as a publishing tool."
> 
> "We needed to start thinking about our users as being service teams around government. Shifting from thinking about making services for citizens to making products for service teams was a tough shift for GDS."
> 
> "To identify the needs of our users, we did 150 interviews with service teams across government. We identified those teams from service assessments, the GOV.UK performance platform and also the 4,000+ PDF forms that are hosted on GOV.UK. We asked them things like: Tell us about your users? Tell us about the needs you are meeting? Tell us about the needs you can't meet but would love to meet?"
> 
> — Ben Welby & Will Myddelton - Government as a Platform programme 2013 - 2018 (UK)
{:.box}

[^1]:   login.gov describes it's aim as to make "federal benefits, services and applications easier and more secure". U.S. General Services Administration, "login.gov", [https://login.gov](https://login.gov). Retrieved 5th June 2019.

[^2]:   Joanne Southern, "Guest post: working with GDS on transforming local services", GOV.UK Verify Blog, 22nd March 2017, [https://identityassurance.blog.gov.uk/2017/03/22/guest-post-working-with-gds-on-transforming-local-services/](https://identityassurance.blog.gov.uk/2017/03/22/guest-post-working-with-gds-on-transforming-local-services/)

[^3]:   Angelica Mari, "London council trials Verify-based digital ID scheme for vulnerable citizens", Computer Weekly, 20th May 2019, [https://www.computerweekly.com/news/252463658/London-council-trials-Verify-based-digital-ID-scheme-for-vulnerable-citizens](https://www.computerweekly.com/news/252463658/London-council-trials-Verify-based-digital-ID-scheme-for-vulnerable-citizens)

[^4]:   "Banks can use Aadhaar for KYC with customer's consent: RBI", The Economic Times, 29th may 2019, [https://economictimes.indiatimes.com/industry/banking/finance/banking/banks-can-use-aadhaar-for-kyc-with-customers-consent-rbi/articleshow/69568435.cms](https://economictimes.indiatimes.com/industry/banking/finance/banking/banks-can-use-aadhaar-for-kyc-with-customers-consent-rbi/articleshow/69568435.cms)
