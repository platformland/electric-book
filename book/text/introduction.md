# Introduction

If you walked into a government office, anywhere on the planet in the 20th Century, you would probably have found three things: a records department managing paper files, index cards or microfiche; administrative staff processing and validating information, either in person over-the-counter or in back-offices, executing the rules set out in different government policies; finally, you'd find forms. Lots and lots of forms.

On the outside of the building, you'd find a sign that contains a word like 'driving', 'passport' or 'tax'. That's because most government departments were, and still are, thematically organized, with responsibility for everything from the top to the bottom of an area of government.

As governments began to put more of their services online, this was the world they digitized. So, today, if you were to look at the technology stack of a typical government agency - let's say a motoring agency with responsibility for issuing driving and vehicle licences - you'd see something like this:

* A series of online transactions - apply for a driving licence, renew a licence, report a change of address - that would more or less map directly to the paper forms they replaced.

* There would be admin systems for things like managing payments or validating addresses - things that humans used to do manually, but these days are semi-automated. The business rules once written out in a policy document have been turned into code.

* Finally, there would be a series of databases - for our hypothetical driving agency, that might be a database of drivers and their cars, and some sort of case-management system for keeping track of applications.  These databases have (mostly) replaced the records departments and paper files that once took over whole floors of government buildings.

This is a pattern that is replicated across government - the pattern repeated in different agencies and at different layers of government. So, if you were to look at land registration, social security, or tax departments, in central government or local government, you'd probably see a similar pattern.

## Digitizing a world of paper

You might be asking, why is this a problem? Surely making paper processes work more efficiently is a good thing? There are several reasons why not.

When it comes to using data from one part of government in another part of government - maybe someone wants to be able to prove they own a car to the tax office - the prevailing practice is what is referred to euphemistically as 'data sharing'.  It's referred to as 'sharing', but it's actually closer to copying and pasting. Records in databases are not like pieces of paper in a file. 'Data sharing' often means multiple copies of the same data end up scattered across government, which has implications for accuracy, security and privacy.

As well as duplication of _data_ there is duplication of _effort_ too. Remember, our hypothetical driving agency? It probably has a payment processing system so people could pay for their driving licences. But other agencies also need to process payments, so public money ends up being spent on the multiple systems, all doing the same thing. The same is true for other commons tasks too - things like messaging or printing.

Thirdly (and most importantly), is the impact on the design of services that the public have to use. In computer science, there's an adage called 'Conway's law'.[^1] It's named after computer programmer Melvin Conway, and it says that:

> "organizations which design systems ... are constrained to produce designs which are copies of the communication structures of these organizations."

Government is this idea writ large - services tend to be designed around the organizational structure of government rather than the needs of people. This means a family looking to move house, someone recovering from an illness or someone looking to start a company, will have to deal separately with many government agencies. The end result is that people fall through the gaps. (You have to ask: what that does to people's trust in the state?).

This also leads to a monopoly of provision - a one to one mapping between department and services, which often means it's impossible for other parts of government, or companies and charities, to build complementary services. That’s because the data and the business logic are locked away inside these organizations.

## Platforms are changing governments

Looking around the world, we can see a different approach emerging. One of cross-government platforms that are beginning to break down government silos, save money and change the types of services that can be delivered to the public. 

For example, in the United States, the U.S. Veterans Administration has begun to buid its services around APIs. This allows veterans charities and other organizations (not just government) to build public-facing services.[^2] This work is part of a federated data effort across central and state governments to build APIs and exchange data to agreed formats.[^3]

In India, the Aadhaar identity platform has started to link together services from across different parts of government for a billion people.[^4] In the process, it's creating a national debate about privacy and digital rights. Aadhaar is part of IndiaStack, which the government refers to as “a set of APIs that allows governments, businesses, startups and developers to utilize an unique digital infrastructure to solve India’s hard problems towards presence-less, paperless, and cashless service delivery”.[^5]

Estonia is starting to design new services around 'life events', like having a child, that transcend the boundaries of government agencies. They can do this because of common cross-government data infrastructure they have developed over the past decade.[^6] And because neighbouring countries have adopted that infrastructure, it holds out the promise of simpler trade, and citizens accessing services across borders.[^7]

In the UK, Italy and Argentina shared components solve common problems for the whole of government. For example: sending a text message, hosting a web application or taking a payment. These components are run centrally, rather than by individual departments, helping civil servants to deliver faster and creating more consistent experiences for citizens.[^8][^9][^10]

## Government as a Platform

Taken together, what we are seeing is the realization of the world sketched out by Tim O'Reilly in his 2011 article 'Government as a Platform', where he posed the question: what if government was organized more like an operating system?[^11]

Government as a Platform holds out the promise of radically better services for the public. And to do so in a way that makes it simpler and faster for both civil servants and politicians, the private sector and non-profits, to meet people’s needs. A world of government reorganized around shared components, APIs, standards and canonical datasets.

[^1]:   Conway, Melvin E. (April 1968), "How do Committees Invent?", Datamation, 14 (5): 28–31

[^2]:   U.S. Department of Veterans Affairs, "Put VA Data to Work", [https://developer.va.gov](https://developer.va.gov). Retrieved 5th June 2019.

[^3]:   Julia Lindpaintner, "The U.S. Data Federation wants to make it easier to collect, combine, and exchange data across government", 5th March 2019, [https://18f.gsa.gov/2019/03/05/the-us-data-federation/](https://18f.gsa.gov/2019/03/05/the-us-data-federation/)

[^4]:   UIDAI, Addhaar Dashboard, [https://uidai.gov.in/aadhaar\_dashboard/index.php](https://uidai.gov.in/aadhaar_dashboard/index.php), Retrieved 5th June 2019

[^5]:   "What is India Stack?", [https://indiastack.org/about/](https://indiastack.org/about/). Retrieved 5th June 2019.

[^6]:   Sam Trendall, "We have only scratched the surface’ – Estonia’s CIO on what’s next for the world’s most celebrated digital nation", PublicTechnology.net, 18th February 2019, [https://publictechnology.net/articles/features/‘we-have-only-scratched-surface’-–-estonia’s-cio-what’s-next-world’s-most](https://publictechnology.net/articles/features/%E2%80%98we-have-only-scratched-surface%E2%80%99-%E2%80%93-estonia%E2%80%99s-cio-what%E2%80%99s-next-world%E2%80%99s-most)

[^7]:   Finnish Patent  "Estonian Ministry of Justice: The Ministry of Justice entered into an agreement with Finland for the exchange of business register data", [https://www.prh.fi/en/uutislistaus/2019/P\_17654.html](https://www.prh.fi/en/uutislistaus/2019/P_17654.html)

[^8]:   HM Government, “Design and build government services”, https://www.gov.uk/service-toolkit#gov-uk-services. Retrieved 30th April 2019,

[^9]:   Team Digitale, “Projects”, https://teamdigitale.governo.it/en/projects.htm. Retrieved 30th April 2019,

[^10]:  Mike Bracken, “Argentina just made driving licences digital”, Public Digital blog, 12th February 2019, https://public.digital/2019/02/12/argentina-just-made-driving-licences-digital/

[^11]:  Tim O'Reilly, "Government as a Platform", Innovations, Vol. 6, Issue. 1, Pages. 13-40, January 2011
