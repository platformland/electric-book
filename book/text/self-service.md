# Designing for self-service

For a platform to serve all its potential users it needs to be usable without direct support from your team. This means designing a service that actively helps different types of users to "self-serve". A platform that is designed for self-service is one that users can find, understand what it does and start using without your intervention.

## 1. Create landing pages for each platform

You can't know who all your potential users might be - they might be in another part of your organization, in another government agency or outside of government altogether (for example a startup developing a new product). So, firstly, your users need to be aware of the platform. Then, if they are aware of it, it is likely that many will ask the same questions, things like "where are you hosted?", "is it secure?", "is there a Python library?", "can I download a CSV of the data?".

Many digital service units are creating public landing pages for their platforms to help users discover them and understand how they work. Australia, Canada and France have public API stores that list APIs that are available to build on. [^1] [^2] [^3]  While units in the UK, USA, Italy and India have all created landing pages for their shared components, and the UK has landing pages for each register. [^4] [^5] [^6] [^7]

Create a public landing page for each component, API or register that lists key information about the platform. Ensure that registers are independently discoverable from components and shared APIs, and that open-data is available to download a bulk dataset. Keep a record of questions that people are regularly asking, such as average uptime, and aim to answer them on the landing page (not hidden elsewhere on an FAQ page).

## 2. Design good documentation

Well-written documentation is essential to help your users understand how to use your platform. But as with any good content, this takes time and an understanding of the needs of your users. Ensure your team has access to technical writers and tests content with users to ensure it meets their needs over time.

## 3. Go where your users are

Developers and designers who are building services using your platforms will have existing tools and workflows. By understanding which package managers, languages and tools that they use, you can make it quicker and simpler for them to get started.[^8]

For example, the U.S. Web Design System and the Australian Government Design System are published as Node.js packages that can be installed via the NPM package management system.[^9] [^10] This makes it simpler to use and to track updates.[^11]

Try and emulate a high-quality open-source vendor. Create and maintain packages in the languages your users use most, and publish code samples online.

## 4. Let users try it out

Commercial platforms like Twilio, Google's Cloud APIs and GoCardless let users try out the capability of their platforms. They do this by either allowing free access at low usage or providing a sandbox environment. They may also provide a manual interface to help users understand it's capabilities without writing any code.

The eSign component, which is part of IndiaStack and allows users to integrate digitally signed documents into their services, also includes links to sandboxes as part of their documentation.[^12] 

Consider creating a manual interface or sandbox so people can use or try it without writing any code and without exposing sensitive information (for example, by using fake data). Think carefully before requiring registration or anything else that might unnecessarily slow users down.

## 5. Understand the needs of procurement and finance

Designing for self-service is not just about meeting the needs of developers and designers. Working hard to make your platform easy to procure is also important.

The GOV.UK Notify team spent lots of time writing Memorandums of Understanding in plain English. They also calculated that they could offer the platform to 80% of users without charging.[^13]

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

[^1]:   Australian Government, "api.gov.au", https://api.gov.au. Retrieved 5th June 2019.

[^2]:   "api.gouv.fr", [https://api.gouv.fr](https://api.gouv.fr). Retrieved 9th march 2019.

[^3]:   Government of Canada, "API Store", [https://api.canada.ca/en/homepage](https://api.canada.ca/en/homepage). Retrieved 5th June 2019.

[^4]:   HM Government, "GOV.UK Service Toolkit", [https://www.gov.uk/service-toolkit#gov-uk-services](https://www.gov.uk/service-toolkit#gov-uk-services). Retrieved 5th June 2019.

[^5]:   18F, "cloud.gov", [https://cloud.gov](https://cloud.gov). Retrieved 5th June 2019.

[^6]:   Agenzia per ill'Italia digitale, "API - Il catalogo delle API REST italiane a disposizione degli sviluppatori", [https://developers.italia.it/it/api](https://developers.italia.it/it/api). Retrieved 23rd April 2019.

[^7]:   HM Government, "GOV.UK Registers", [https://www.registers.service.gov.uk](https://www.registers.service.gov.uk). Retrieved 17th June 2019.

[^8]:   Citation needed

[^9]:   "uswds (United States Web Design System)", npm, [https://www.npmjs.com/package/uswds](https://www.npmjs.com/package/uswds). Retrieved 5th June 2019.

[^10]:  "[uswds (United States Web Design System)](gov.au)", npm, [https://www.npmjs.com/org/gov.au](https://www.npmjs.com/org/gov.au). Retrieved 8th June 2019.

[^11]:  Citation needed

[^12]:  "About eSign API", [https://indiastack.org/esign/](https://indiastack.org/esign/). Retrieved 8th June 2019.

[^13]:  Citation needed
