# Transparency, accountability and governance

Transparency, accountability and governance processes are not an end in themselves. The aim should be to make sure things are working as they should be, and that people understand what "should be" looks like.

As with trust and consent systems, there are limits to what a digital service team can do in this area (many responsibilities will lay with elected representatives and empowered regulators).

## 1. Put accountability, recourse and transparency at the point of use

Governments have an obligation to help citizens understand the functioning of their democracy, and give them clear opportunities for recourse when things go wrong. A platform ecosystem in combination with services designed to 'just work' could obfuscate how government works. This is not supposed to suggest that people have a brilliant mental model of how government works today, but there is an obligation on teams designing platforms and services to ensure they make that understanding better, not worse. Taken as a whole, the system should actively educate people about how their government works, where power and accountability lie and how services are performing.

For each service linked to from the GOV.UK publishing platform, there is a corresponding page that explains some elements of the current performance of the service and an explanation of the underlying user need for the service.[^1] While the information is currently limited, it is easy to imagine it expanding to include data about both the real-world analytics, the data and the underlying legislation used to operate the service.

In New South Wales, Australia government services make use of a shared component, (in this case, a wrapper around a commercial CRM), for adding feedback to digital services.[^2]

Put information about performance and accountability at the point of use of services. Conduct user research to understand the information citizens, their representatives, or civil society organizations might need to understand how a service works and who is accountable for it.

## 2. Ensure platforms have owners and registers have custodians

Clear product ownership (one person who can direct the work of a team to meet the needs of users) is just as important for platforms as it is for public-facing services. Even in situations where some element of a platform is outsourced, you will still need to maintain the expertise in-house to monitor and audit.

The consequences of incorrect data in a platform ecosystem are potentially higher than in legacy systems (an incorrect data item in a register could affect many services). As such, data custodianship also needs to be clear (and this may be distinct from product ownership). A data custodian is accountable for the quality and accuracy of data.

Ensure that there is a product owner for each platform and service and that each register has a clear custodian.

## 3. Decide the 'rules of the road' for non-government services

For platforms that allow non-government services to be built on top of them, there may need to be clear rules about the type of services that can be built on top of them (for example, if they make use of sensitive data, or require users to understand a particular piece of information).

Consider the risks of government being disintermediated and of data misuse. Understand which parts of the user experience government will always need to control.

## 4. Put users in control of the data about them

Put users in control of their data. Millions of engaged curators are the best protection government has against fraud, and that citizens have against misuse. Users should be able to see what services have access to their data and what access has been made.

By default, Estonian citizens have the right to see _all_ data held about them, unless explicitly restricted.[^3] In India, holders of an Aadhaar identity can view the history of how it has been used.[^4]

Design ways for people to access and understand how data about them is being used.
 
## 5. Expose the rules and design for monitoring

Digital systems encode the law in software. This raises the question of how people (or more likely their representatives) know if a system is working as it should be. Open-source code and associated software tests can help third parties understand how government systems work and better hold them to account.

Another approach to consider is if there are opportunities to expose data that helps third parties monitor the quality of information. In the US, the Web Integrity Project is independent of government and automatically monitors for changes to federal government websites.[^5] Currently, it does this by crawling government websites, but this could be made much easier by exposing content changes via APIs.

## 6. Maintain an archive of user interface changes

Small design choices can have big impacts on how people access and understand services.[^6] Seeking out screen-shots of government software is also increasingly becoming a human rights monitoring activity - recent studies of China's Social Credit System and Saudi Arabia's 'Absher' have both made use of screen-shots to understand the impact on people's rights.

Maintain a public archive of any changes to the user-interfaces of services (and platforms that have public-facing elements).

## 7. Design for verifiable use of data

Numerous examples around the world show that access rules and legal frameworks are not enough to limit the misuse of data. There are emerging approaches that allow for the verifiable use of data through recording access in immutable databases such as Trillian or Amazon QLDB. [^7][^8][^9][^10]

Estonia's X-Road data exchange uses this approach to create a tamper-proof log of data accessed across the system. (Contrary to reports, X-Road does not use blockchain).[^11]

Don't just rely on access controls to limit the use of data.

> ### Example: The Web Integrity Project
> 
> The Web Integrity Project systematically monitors changes to 30,000 federal agency webpages using software that crawls URLs every few days and alerts us when a change has been made. A team of analysts review the changes, and the Web Integrity Project extensively reviews and vet and changes we decide to report on. The regular monitoring of websites forms the basis of our efforts to hold the federal government accountable by revealing shifts in information and public access to resources. We work with journalists to make our findings public, and we produce policy analyses to evaluate and recommend changes to web governance practices and help ensure access to valuable Web resources.
> 
> Many of the changes we find are minor or routine. Others reflect stated shifts in policy. Some reveal the removal of large amounts of useful information or data from public view.  And sometimes we see alterations to websites that are more like spoilers: they foreshadow changes in policy that will come later after a much longer, more open rulemaking process or a public announcement of the policy shift.
> 
> A government API that included data on content changes, the creation and removal of pages, and usage statistics would be of immense use in our work. We could build a more automated and efficient workflow with access to information on which pages were changed, removed, or added and exactly when.
> 
> — Dr Sarah John, Director, Web Integrity Project 
{:.box}

[^1]:   For an example see [https://www.gov.uk/info/jobsearch](https://www.gov.uk/info/jobsearch)

[^2]:   NSW Government, "Feedback Assist", [https://www.digital.nsw.gov.au/digital-design-system/components/reusable-components/feedback-assist](https://www.digital.nsw.gov.au/digital-design-system/components/reusable-components/feedback-assist). Retrieved 25th June 2019.

[^3]:   Riigikantselei, "Public Information Act", Section 43-8, [https://www.riigiteataja.ee/en/eli/518012016001/consolide](https://www.riigiteataja.ee/en/eli/518012016001/consolide)

[^4]:   Unique Identification Authority of India, "Aadhaar Authentication History", [https://uidai.gov.in/305-faqs/aadhaar-online-services/aadhaar-authentication-history.html](https://uidai.gov.in/305-faqs/aadhaar-online-services/aadhaar-authentication-history.html). Retrieved 25th June 2019.

[^5]:   "Web Integrity Project", [https://sunlightfoundation.com/web-integrity-project/](https://sunlightfoundation.com/web-integrity-project/). Retrieved 26th June 2019.

[^6]:   As immigration solicitor, Jonathan Kingham, notes in this article on the digitization of Brexit era immigration systems in the UK:
  "Unlike with Rules and legislation changes, there was little opportunity to scrutinise the detail of what are in fact significant changes to the immigration system prior to their coming into force (bar selective ‘user testing’, which is rarely transparent to all). And, as with so many tech developments, as the process or ‘app’ itself increasingly takes centre stage over the content (in this case the law) that underpins it, there are risks." 8th January 2019, "“Computer says no”: facing up to the full implications of a digitised immigration system", [https://www.freemovement.org.uk/computer-says-no-digitised-immigration-system/](https://www.freemovement.org.uk/computer-says-no-digitised-immigration-system/)

[^7]:   Open Data Institute / Register Dynamics, "Putting the trust in data trusts", 14th April 2019, [https://www.register-dynamics.co.uk/data-trusts/index.html](https://www.register-dynamics.co.uk/data-trusts/index.html)

[^8]:   Emily Mattiussi, "Monitoring cloud data with Trillian", IF Journal, 3rd April 2019, [https://www.projectsbyif.com/blog/monitoring-cloud-data-with-trillian/](https://www.projectsbyif.com/blog/monitoring-cloud-data-with-trillian/)

[^9]:   "google/trillian", GitHub, [https://github.com/google/trillian](https://github.com/google/trillian). Retrieved 25th June 2019.

[^10]:  "Amazon Quantum Ledger Database (QLDB)", [https://aws.amazon.com/qldb/](https://aws.amazon.com/qldb/). Retrieved 25th June 2019.

[^11]:  Petteri Kivimäki, "There is no blockchain technology in the X-Road", Nordic Institute for Interoperability Solutions blog, 26th April 2019,  [https://www.niis.org/blog/2018/4/26/there-is-no-blockchain-technology-in-the-x-road](https://www.niis.org/blog/2018/4/26/there-is-no-blockchain-technology-in-the-x-road)
