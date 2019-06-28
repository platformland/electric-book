# Trust and consent

When it comes to digital identity and the exchange of data many of the requirements for the safe operation of a platform ecosystem, such as an effective and legal framework for privacy and digital rights, are beyond the gift of digital service teams. As such, do not read this section as anything approaching a complete list. Instead, see it as a set of practical things that should be within your control.

## 1. Design for an identity ecosystem (not an identity system)

Digital identity is often thought of in terms of a singular system - a single digital identity system to join everything together. There are risks with this approach. It potentially creates a single point of failure.[^1] It risks joining together data that are best kept separate. It also may not reflect the reality that many countries have multiple systems of ID that can be made interoperable.

Countries may operate different identity systems at a municipal and national level and people may have legitimate reasons for wanting to keep different aspects of their lives separate through different identities (for example, keeping health information separate).

For example, Sweden operates multiple identity systems, including IDs issued by banks accepted for certain government services.[^2] European countries are beginning to accept each other's digital IDs as part of the eIDAS program.[^3]

## 2. Design for trust escalation (and failure)

Services should be able to establish enough trust (and only enough trust) to allow their users to achieve a desired outcome.  There are many services for which proving an identity is not needed at all. There are also services, or stages of services, that need different levels of trust. For example, applying and paying for a licence may require a lower level of trust than someone changing the bank their benefit payments are paid to.

Inevitably, there will be circumstances where people are unable to meet the level of trust online (or they may be unable to go online at all). As such, providing a real-world fall-back is important. In the UK, this idea has been explored through the use of a chain of high street stores for verifying paper documents.[^4]

Avoid putting an identity verification step in services that don't need it. Map out the levels of trust needed for each stage of a service and integrate identity verifications accordingly. Provide real-world fall-backs and backups for when a process cannot be completed digitally.
## 3. Ask people for less data

Collecting data to personalize a platform or service comes at a cost to a users time and privacy. The more data collected and held, the greater the security and privacy risk. Collect only the minimum data needed to operate a platform or service.

## 4. Understand where data lies on the open-shared-closed spectrum

Registers should be made as open as possible, but understanding of what 'as possible' means requires a deliberate decision about where data lies on the spectrum of open-shared-closed.[^5] This should be informed by data impact and privacy assessments, security and ethical considerations.

Understand where data held by a register or shared API sits on this spectrum. Use that knowledge to design an appropriate data access model and governance process for the data.

## 5. Make some data harder to join together

To avoid unintended consequences, some data should be harder to join together than others. A clear example of why this is important comes from the UK National Health Service.

In November 2018, the UK National Health Service finally pulled out of a controversial "memorandum of understanding" with the Home Office (which is responsible for immigration enforcement). It had granted Home Office immigration officers access to data about patients to help them trace people breaking immigration rules.[^6] The withdrawal followed objections from Public Health England and the House of Commons Health and Social Care Committee that people not seeking medical attention, or deliberately missing vaccinations for fear of data about them being shared, posed a risk to public health.[^7][^8]

While this may be an extreme example, making it clear to users how and when data is being joined together is important. There are many different design patterns available for informing users about data use, or asking for explicit consent.[^9]

## 6. Create APIs that answer questions

When designing your APIs, look for opportunities to limit the amount of information that is revealed. Rather than sharing a full database record, design APIs that answer specific questions. For example, "does this car have a permit to park in this area ?— yes or no?", "Is this person entitled to work in this country — yes or no?"

This allows services to find the information needed to operate that service, without all the negatives that come with traditional approaches to ‘data-sharing’ in government.

## 7. Use digital proofs to join services together

Digital proofs offer the opportunity to keep some of the good things about paper certificates while removing some of the risks. They allow people to prove things to whomever they like and however they like: the designers of a service don’t need to guess upfront all the different situations that someone might experience.

For example, someone can prove to one part of government that another part of government agrees a certain fact about them  -  for example, that they own a property  - without the need for duplicating and sharing entire datasets between organizations. It’s up to the organization or individual receiving the proof to decide if they trust it or not, which allows for flexibility.

One example is Digilocker, part of the IndiaStack project. It is a personal data store for cryptographically signed government documents. Among other things, people can use it to store a digital representation of their driving licence, or a university certificate signed by the organization that issued it.[^10]

Another example is the approach used by the GOV.UK ‘Share driving licence’ service. It lets users create a one-use code that a third party (for example a car-rental company) can use to check the details of a licence.[^11] This has the advantage that it clearly puts the user in control of how and when they share data about themselves.

Digital proofs, in combination with apps like DigiLocker for storing and managing digital proofs, are an evolving area, with the Android platform and the W3C both actively developing approaches.[^12][^13] The important thing to consider however, is not the technology, but where the principle of putting verifiable facts in the hands of the public would be most beneficial.

## 9. Make understanding risks part of the design process 

Governance can't just be something that happens in the realm of policy documents. Ensuring that design and development processes make space for an understanding of risks is also important.

This is true both of platforms (what might the unintended consequences be of collecting, modelling or using data in a particular way?) and the services built on top of them (who benefits and who might lose?). 

There are a few emerging approaches to this, including 'consequence scanning' and 'data ethics canvases'.[^14][^15] Adopting a human rights review of key digital infrastructure has also been suggested.[^16]

[^1]:   e.g. South Korea had to reissue government IDs at huge cost after a data breach. Iain Thompson, "South Korea faces $1bn bill after hackers raid national ID database", The Register 14th October 2014, [https://www.theregister.co.uk/2014/10/14/south\_korea\_national\_identity\_system\_hacked/](https://www.theregister.co.uk/2014/10/14/south_korea_national_identity_system_hacked/)

[^2]:   BankID, [https://www.bankid.com/en/](https://www.bankid.com/en/). Retrieved 8th February 2019.

[^3]:   "Trust Services and Electronic identification (eID)", [https://ec.europa.eu/digital-single-market/en/trust-services-and-eid](https://ec.europa.eu/digital-single-market/en/trust-services-and-eid). Retrieved 26th June 2019.

[^4]:   Open Identity Exchange, "Face-to-face identity proofing to help people obtain an assured digital identity", [https://oixuk.org/wp-content/uploads/2017/01/F2F-white-paper-final.pdf](https://oixuk.org/wp-content/uploads/2017/01/F2F-white-paper-final.pdf)

[^5]:   Open Data Institute, "The Data Spectrum helps you understand the language of data", [https://theodi.org/about-the-odi/the-data-spectrum/](https://theodi.org/about-the-odi/the-data-spectrum/). Retrieved 26th June 2019.

[^6]:   Jasmin Gray, “NHS Pulls Out Of Data-Sharing Deal With Home Office Immigration Enforcers”, Huffington Post, 12th November 2018, [https://www.huffingtonpost.co.uk/entry/nhs-data-sharing-home-office_uk_5be97198e4b0e843889a1b5d](https://www.huffingtonpost.co.uk/entry/nhs-data-sharing-home-office_uk_5be97198e4b0e843889a1b5d)

[^7]:   Denis Campbell, “NHS will no longer have to share immigrants’ data with Home Office”, Guardian, 9th May 2018, [https://www.theguardian.com/society/2018/may/09/government-to-stop-forcing-nhs-to-share-patients-data-with-home-office](https://www.theguardian.com/society/2018/may/09/government-to-stop-forcing-nhs-to-share-patients-data-with-home-office)

[^8]:   Alan Travis, “NHS chiefs urged to stop giving patient data to immigration officials”, Guardian, 31st January 2018, https://[www.theguardian.com/society/2018/jan/31/nhs-chiefs-stop-patient-data-immigration-officials](www.theguardian.com/society/2018/jan/31/nhs-chiefs-stop-patient-data-immigration-officials)

[^9]:   IF, "data Permissions Catalogue", [https://catalogue.projectsbyif.com](https://catalogue.projectsbyif.com). Retrieved 26th June 2019.

[^10]:  National eGovernance Division
  Ministry of Electronics & Information Technology (MeitY), "About DigiLocker", [https://digilocker.gov.in/about.php](https://digilocker.gov.in/about.php). Retrieved 5th April 2019.

[^11]:  Sally Meecham, "A new way to view your driving licence info online", Government Digital Service Blog, 7th October 2014, [https://gds.blog.gov.uk/2014/10/07/a-new-way-to-view-your-driving-licence-info-online/](https://gds.blog.gov.uk/2014/10/07/a-new-way-to-view-your-driving-licence-info-online/)

[^12]:  Mishaal Rahman, "Google is working on securely storing Digital Driver’s Licenses in Android", XDA Developers, 5th March 2019, [https://www.xda-developers.com/google-android-digital-drivers-license/](https://www.xda-developers.com/google-android-digital-drivers-license/)

[^13]:  W3C, "Verifiable Credentials Data Model 1.0", 28th March 2019, [https://www.w3.org/TR/verifiable-claims-data-model/](https://www.w3.org/TR/verifiable-claims-data-model/)

[^14]:  Open Data Institute, "What is the Data Ethics Canvas?", 5th April 2017, [https://theodi.org/article/data-ethics-canvas/](https://theodi.org/article/data-ethics-canvas/)

[^15]:  Doteveryone, "Consequence Scanning", [https://doteveryone.org.uk/project/consequence-scanning/](https://doteveryone.org.uk/project/consequence-scanning/). Retrieved 25th June 2019.

[^16]:  Beatrice Martini, "What is at stake for human rights in the design of Internet protocols?", Kennedy School Review, 13th May 2019, [http://ksr.hkspublications.org/2019/05/13/what-is-at-stake-for-human-rights-in-the-design-of-internet-protocols/](http://ksr.hkspublications.org/2019/05/13/what-is-at-stake-for-human-rights-in-the-design-of-internet-protocols/)
