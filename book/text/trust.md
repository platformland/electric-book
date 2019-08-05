# Identity, trust and consent

When it comes to digital identity and the exchange of data between organizations, many of the requirements for the safe operation of a platform ecosystem, such as an effective and legal framework for privacy and digital rights, are beyond the gift of digital service teams. However, there are many things that you can do to minimize the risks to privacy and trust. As such, please do not read this section as anything approaching a complete list, instead, see it as a set of practical things that should be within your control.

## 1. Design for an identity ecosystem (not an identity system)

Digital identity is often thought of in terms of a singular system - a single digital identity system to join everything together. However, there are several risks with this approach.

It potentially creates a single point of failure and it risks joining together data sets that are best kept separate. The cost (both to privacy and financially) of a single system being compromised is higher.[^1]

It may also not reflect the reality that many countries have multiple de facto systems of ID - a country may operate different identity systems at a municipal and national level. For example, Sweden operates multiple identity systems, including IDs issued by banks accepted for certain government services.[^2] European countries are beginning to accept each other's digital IDs as part of the eIDAS program.[^3]

Finally, people may have legitimate reasons for wanting to keep different aspects of their lives separate through different identities (for example, keeping health information separate).

Understand these risks when thinking about implementing or utilizing a digital identity system.

## 2. Design for trust escalation (and failure)

There are many services for which proving an identity will not be necessary at all. There are also services, or stages of services, that demand different levels of trust. For example, applying and paying for a licence may require a lower level of trust than someone changing the bank their benefit payments are paid to.

Services should be able to establish enough trust (and only enough trust) to allow their users to achieve their desired outcome.

Inevitably, there will also be circumstances where people are unable to meet the level of trust online (or they may be unable to go online at all). As such, providing a real-world fall-back is important. In the UK, this idea has been explored through the use of a chain of high street stores for checking documents in person.[^4]

Avoid putting an identity verification step in services that don't need it. Map out the levels of trust needed for each stage of a service and integrate identity verification and authentication steps accordingly. Provide real-world fall-backs for when a process cannot be completed digitally.

## 3. Understand digital identity in context

In many contexts, digital identity systems have the opportunity to make services simpler by creating a consistent way for people to verify their identity to different institutions - be that government, or refugee agencies providing aid. They also have the potential to offer opportunities for marginalized and undocumented communities to access vital services, such as access to justice, and welfare.

However, centralized systems, and particularly systems which gather biometric data, also bring huge risks and challenges to the privacy and security of people whose data is collected. This is particularly the case when mechanisms for recourse or accountability in are absent or fall short.

The way data that is collected and stored against someone's identity also affects how those people's rights can be exercised. For example are there are options for people to represent themselves as they see themselves (for example, non-binary genders, people from countries that aren't recognized by government institutions).

These risks and benefits will affect different groups in different ways (for example, by gender).[^5] Also, as new datasets (such as healthcare or immigration status) are joined together through a digital identity, those risks will change.

Understand the implications of how data is associated with a digital identity for different groups. Provide clear routes to address mistakes or unintended consequences.

## 4. Ask people for less data

Collecting and retaining data to personalize a platform or service comes at a cost to a users time and privacy. The more data collected and held, the greater the security and privacy risk.

Collect only the minimum data needed to operate a platform or service.

## 5. Understand where data lies on the open-shared-closed spectrum

Registers should be made as open as possible, but understanding of what 'as possible' means requires a deliberate decision about where data lies on the spectrum of "open-shared-closed".[^6] This should be informed by data impact and privacy assessments, security and ethical considerations.

Understand where data held by a register or shared API sits on the open-data spectrum. Use this knowledge to design an appropriate data access model and governance process for the data.

## 6. Make some data harder to join together

There can be unintended consequences when data is joined together.
A clear example this is important comes from the UK health and immigration services. 

In November 2018, the UK National Health Service finally pulled out of a controversial "memorandum of understanding" with the Home Office (which is responsible for immigration enforcement). It had granted Home Office immigration officers access to data about patients to help them trace people breaking immigration rules.[^7] The withdrawal followed objections from Public Health England and the House of Commons Health and Social Care Committee that people not seeking medical attention, or deliberately missing vaccinations for fear of data about them being shared, posed a risk to public health.[^8] [^9]

While this may be an extreme example, understanding such risks is critical. It is also important to be transparent to the public about when and how data is being joined together or exchanged. (There are many different design patterns available for informing users about data use, or asking for explicit consent.) [^10]

Understand the risks of joining together different datasets. Be transparent to the public about data use.

## 7. Create APIs that answer questions

When designing APIs, rather than sharing full database records, create endpoints answer specific questions. For example, "does this car have a permit to park in this area ?— yes or no?", "Is this person entitled to work in this country — yes or no?" This allows services to find the information needed to operate that service, without all the negatives that come with traditional approaches to ‘data-sharing’ in government.

Look for opportunities to limit the amount of information that is exposed via APIs.

## 8. Use digital proofs to join services together

Digital proofs offer the opportunity to keep some of the good things about paper certificates while removing some of the risks. They also allow people to prove things to whomever they like and however they like.

This means the designers of a service don’t need to guess upfront all the different situations that someone might experience. For example, someone can prove to one part of government that another part of government agrees a certain fact about them  -  for example, that they own a property  - without the need for duplicating and sharing entire datasets between organizations. It’s up to the organization or individual receiving the proof to decide if they trust it or not, which allows for flexibility.

One example is Digilocker, part of the IndiaStack project. Digilocker is a personal data store for cryptographically signed government documents. Among other things, people can use it to store a digital representation of their driving licence, or a university certificate signed by the organization that issued it.[^11]

Another example is the approach used by the GOV.UK ‘Share driving licence’ service. It lets users create a one-use code that a third party (for example a car-rental company) can use to check the details of a licence.[^12] This has the advantage that it clearly puts the user in control of how and when they share data about themselves.

Digital proofs, in combination with apps like DigiLocker for storing and managing digital proofs, are an evolving area, with the Android platform and the W3C both actively developing approaches.[^13] [^14] The important thing to consider however, is not the technology, but where the principle of putting verifiable facts in the hands of the public would be most beneficial.

[^1]:   e.g. South Korea had to reissue government IDs at huge cost after a data breach. Iain Thompson, "South Korea faces $1bn bill after hackers raid national ID database", The Register 14th October 2014, [https://www.theregister.co.uk/2014/10/14/south\_korea\_national\_identity\_system\_hacked/](https://www.theregister.co.uk/2014/10/14/south_korea_national_identity_system_hacked/)

[^2]:   BankID, [https://www.bankid.com/en/](https://www.bankid.com/en/). Retrieved 8th February 2019.

[^3]:   "Trust Services and Electronic identification (eID)", [https://ec.europa.eu/digital-single-market/en/trust-services-and-eid](https://ec.europa.eu/digital-single-market/en/trust-services-and-eid). Retrieved 26th June 2019.

[^4]:   Open Identity Exchange, "Face-to-face identity proofing to help people obtain an assured digital identity", [https://oixuk.org/wp-content/uploads/2017/01/F2F-white-paper-final.pdf](https://oixuk.org/wp-content/uploads/2017/01/F2F-white-paper-final.pdf)

[^5]:   Zara Rahman, "Digital ID: why it matters, and what we're doing about it", 13th September 2018, [https://www.theengineroom.org/digital-id-why-it-matters/](https://www.theengineroom.org/digital-id-why-it-matters/)

[^6]:   Open Data Institute, "The Data Spectrum helps you understand the language of data", [https://theodi.org/about-the-odi/the-data-spectrum/](https://theodi.org/about-the-odi/the-data-spectrum/). Retrieved 26th June 2019.

[^7]:   Jasmin Gray, “NHS Pulls Out Of Data-Sharing Deal With Home Office Immigration Enforcers”, Huffington Post, 12th November 2018, [https://www.huffingtonpost.co.uk/entry/nhs-data-sharing-home-office_uk_5be97198e4b0e843889a1b5d](https://www.huffingtonpost.co.uk/entry/nhs-data-sharing-home-office_uk_5be97198e4b0e843889a1b5d)

[^8]:   Denis Campbell, “NHS will no longer have to share immigrants’ data with Home Office”, Guardian, 9th May 2018, [https://www.theguardian.com/society/2018/may/09/government-to-stop-forcing-nhs-to-share-patients-data-with-home-office](https://www.theguardian.com/society/2018/may/09/government-to-stop-forcing-nhs-to-share-patients-data-with-home-office)

[^9]:   Alan Travis, “NHS chiefs urged to stop giving patient data to immigration officials”, Guardian, 31st January 2018, https://[www.theguardian.com/society/2018/jan/31/nhs-chiefs-stop-patient-data-immigration-officials](www.theguardian.com/society/2018/jan/31/nhs-chiefs-stop-patient-data-immigration-officials)

[^10]:  IF, "Data Permissions Catalogue", [https://catalogue.projectsbyif.com](https://catalogue.projectsbyif.com). Retrieved 26th June 2019.

[^11]:  National eGovernance Division Ministry of Electronics & Information Technology (MeitY), "About DigiLocker", [https://digilocker.gov.in/about.php](https://digilocker.gov.in/about.php). Retrieved 5th April 2019.

[^12]:  Sally Meecham, "A new way to view your driving licence info online", Government Digital Service Blog, 7th October 2014, [https://gds.blog.gov.uk/2014/10/07/a-new-way-to-view-your-driving-licence-info-online/](https://gds.blog.gov.uk/2014/10/07/a-new-way-to-view-your-driving-licence-info-online/)

[^13]:  Mishaal Rahman, "Google is working on securely storing Digital Driver’s Licenses in Android", XDA Developers, 5th March 2019, [https://www.xda-developers.com/google-android-digital-drivers-license/](https://www.xda-developers.com/google-android-digital-drivers-license/)

[^14]:  W3C, "Verifiable Credentials Data Model 1.0", 28th March 2019, [https://www.w3.org/TR/verifiable-claims-data-model/](https://www.w3.org/TR/verifiable-claims-data-model/)
