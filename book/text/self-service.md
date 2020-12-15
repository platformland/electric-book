# Designing for self-service

For a platform to serve all its potential users it needs to be usable without direct support. This means designing a service that actively helps different types of users to "self-serve". A platform that is designed for self-service is one that users can find, understand what it does and start using without intervention.

## 1. Create landing pages for each platform

You can't know who all your potential users might be - they might be in another part of your organization, in another government agency or outside of government altogether (for example a startup developing a new product). So, firstly, your users need to be aware of the platform. Then, if they are aware of it, it is likely that many will ask the same questions, things like "where are you hosted?", "is it secure?", "is there a Python library?", "can I download a CSV of the data?".

Many digital service units are creating public landing pages for their platforms to help users discover them and understand how they work. Australia, Canada and France have public API stores that list APIs that are available to build on. [^1] [^2] [^3]  While units in the UK, USA, Italy and India have all created landing pages for their shared components, and the UK has landing pages for each register. [^4] [^5] [^6] [^7]

Create a public landing page for each component, API and register that lists key information about the each platform. Ensure that registers are independently discoverable from shared APIs and components. For registers containing open-data it should also be easy to identify how to download a bulk dataset from the landing page.

Keep a record of questions that people are regularly asking, such as average uptime, and aim to answer them on the landing page (not hidden elsewhere on an FAQ page).

## 2. Design good documentation

Well-written documentation is essential to help your users understand how to use your platform.[^8] Github's 2017 Open Source Survey found that incomplete or confusing documentation was the biggest problem encountered by developers.[^9]

As with any good content, developing good documentation takes time and an understanding of the needs of your users. The UK Government Digital Service maintain a template for different teams to publish technical documentation, which has users across government.[^10] Adoption of that template increased when it was itself, well documented.[^11]

Ensure your team has access to technical writers and tests content with users to ensure it continues to meets their needs over time. Use automated tools such as Swagger to help keep documentation up to date.[^12][^13]

## 3. Go where your users are

Developers and designers who are building services using your platforms will have existing tools and workflows. By understanding which package managers, languages and tools they use, you can make it quicker and simpler for them to get started.

For example, the U.S. Web Design System and the Australian Government Design System are published as Node.js packages that can be installed via the NPM package management system.[^14] [^15] This makes them simpler to use and to track updates.

Try and emulate a high-quality open-source vendor. Create and maintain packages in the languages your users use most, and publish code samples online.

## 4. Let users try it out

Commercial platforms like Twilio, Google's Cloud APIs and GoCardless let users try out the capability of their platforms. They do this by either allowing free access at low usage or providing a sandbox environment.

The eSign component, which is part of IndiaStack and allows users to integrate digitally signed documents into their services, includes links to sandboxes as part of their documentation.[^16] 

Create ways for people to try your platform quickly and without exposing sensitive information (for example, by using fake data). Think carefully before requiring registration or anything else that might unnecessarily slow users down.

## 5. Understand the needs of procurement and finance

Designing for self-service is not just about meeting the needs of developers and designers. Working hard to make your platform easy to procure is also important.

The GOV.UK Notify team spent lots of time writing Memorandums of Understanding in plain English. They also calculated that they could offer the platform to many users without charging.[^17]

When planning your user research, make sure to include people responsible for procurement and finance. Map out procurement 'pain-points' and prioritise addressing them.

> ### Example: Designing GOV.UK Notify for self-service
> 
> **The GOV.UK Notify team aimed to build for self-service from day one. They discovered that it was an effective way of increasing adoption for the shared component.**
> 
> "From day one of GOV.UK Notify, our hypothesis was that we needed to build something that was highly scalable. That meant we needed to do what everyone else on the web was doing: design for self-service. Jeff Bezos doesn't come around your house if you need to spin-up a new EC2 instance."
> 
> "If you have a government email address, you can create a trial account. We also got really rich feedback by saying to people, "rather than a meeting or a phone call, have a go first, and then come back to us if you get stuck". This was a bold step when we only had a few users but got easier as adoption grew, and the insight gained was invaluable."
> 
> "This approach also allowed us to sell what we were doing through our presentations and blog posts etc. where the call-to-action wasn't "get in touch", it was "go and try it". Within the team we called this 'permission to play'."
> 
> — Pete Herlihy - Lead Product Manager, Government Digital Service
{:.box}

[^1]:   Australian Government, "api.gov.au", [https://api.gov.au](https://api.gov.au). Retrieved 5th June 2019.

[^2]:   "api.gouv.fr", [https://api.gouv.fr](https://api.gouv.fr). Retrieved 9th march 2019.

[^3]:   Government of Canada, "API Store", [https://api.canada.ca/en/homepage](https://api.canada.ca/en/homepage). Retrieved 5th June 2019.

[^4]:   HM Government, "GOV.UK Service Toolkit", [https://www.gov.uk/service-toolkit#gov-uk-services](https://www.gov.uk/service-toolkit#gov-uk-services). Retrieved 5th June 2019.

[^5]:   18F, "cloud.gov", [https://cloud.gov](https://cloud.gov). Retrieved 5th June 2019.

[^6]:   Agenzia per ill'Italia digitale, "API - Il catalogo delle API REST italiane a disposizione degli sviluppatori", [https://developers.italia.it/it/api](https://developers.italia.it/it/api). Retrieved 23rd April 2019.

[^7]:   HM Government, "GOV.UK Registers", [https://www.registers.service.gov.uk](https://www.registers.service.gov.uk). Retrieved 17th June 2019.

[^8]:   HM Government, "How to document APIs", [https://www.gov.uk/guidance/writing-api-reference-documentation](https://www.gov.uk/guidance/writing-api-reference-documentation), GOV.UK 15th February 2019

[^9]:   GitHub, "Open Source Survey", [https://opensourcesurvey.org/2017/](https://opensourcesurvey.org/2017/). Retrieved 30th June 2019.

[^10]:  alphagov/tech-docs-template, "alphagov/tech-docs-template: A template for building technical documentation with a GOV.UK style", [https://github.com/alphagov/tech-docs-template](https://github.com/alphagov/tech-docs-template). Retrieved 30th June 2019.

[^11]:  Interview, Rosalie Marshall, Lead Technology Advisor &
  Head of Data and API Standards, Government Digital Service

[^12]:  "Create Great API Documentation", [https://swagger.io/solutions/api-documentation/](https://swagger.io/solutions/api-documentation/). Retrieved 30th June 2019.

[^13]:  HM Government, "Writing API reference documentation", GOV.UK, 15th February 2019, [https://www.gov.uk/guidance/writing-api-reference-documentation#generating-api-reference-from-code](https://www.gov.uk/guidance/writing-api-reference-documentation#generating-api-reference-from-code)

[^14]:  "uswds (United States Web Design System)", npm, [https://www.npmjs.com/package/uswds](https://www.npmjs.com/package/uswds). Retrieved 5th June 2019.

[^15]:  "[uswds (United States Web Design System)](gov.au)", npm, [https://www.npmjs.com/org/gov.au](https://www.npmjs.com/org/gov.au). Retrieved 8th June 2019.

[^16]:  "About eSign API", [https://indiastack.org/esign/](https://indiastack.org/esign/). Retrieved 8th June 2019.

[^17]:  HM Government, "Pricing", [https://www.notifications.service.gov.uk/pricing](https://www.notifications.service.gov.uk/pricing). Retrieved 26th June 2019.
