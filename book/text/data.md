# Data infrastructure, APIs and open standards

WIth legacy systems, data gets shared and duplicated. In a platform ecosystem data is accessed as needed, via APIs using agreed open-standards. Data, rather than being held in multiple places and multiple formats, is stored in canonical registers.

## 1. Create canonical registers of data and manage them on behalf of multiple services

The development and maintenance of canonical data registers -  agreed lists of facts like addresses, refuse collection days,  or the location of health facilities is critical for enabling other services. Registers need to be managed for the broader ecosystem of public-facing services, rather than tied to a single, specific service. Your aim should be to maximize the benefit the data can provide.

For example, adresse.data.gouv.fr is the French register of addresses and is operated by the Etalab, the government unit responsible for open data. The data is made available via an API under an open licence so that it is free and reusable by anyone.[^1]

Identify and actively develop registers, ensuring that they have clear custodianship, appropriate licensing and are designed for self-service.

## 2. Use open, emergent processes to agree open-standards

Open standards (with stable identifiers) mean that different teams can be confident that they are speaking the same language, and the designers of public facing services can build on top of reliable, predictable data.

The process of agreeing standards need not be onerous. 
Large-scale, standardization efforts outside of government show what is possible, from OpenStreetMap to the Fast Healthcare Interoperability Resource specification, and Internet Engineering Task Force. Each effort favours progress, working implementations, public evolution and concrete use cases over perfection and completeness.

In the UK, the Cabinet Office solicits suggestions for the adoption of existing open standards via GitHub.[^2] Businesses, citizens or civil servants can suggest areas that may benefit from the adoption of standards. There is then an open process for the suggestion and adoption of open standards.

## 3. Build on APIs and create new APIs

Developing a platform ecosystem requires both canonical data registers, and the business processes of government (for example, the status of a visa application) to be exposed as APIs. i.e. the data can be accessed programatically and in real-time.

This will not happen by itself. It requires APIs to be prioritized by teams developing services and for space to be made for the development of shared data infrastructure.

When Argentina was developing it's new digital driving licence, rather than build a single system, the National Road Safety Agency provided an API, that API was then integrated into the miArgentina app where the digital driving licence service is housed. [^3]  And when 18F developed the cross-government  FOIA.gov for managing freedom of information requests, they also provided an API for the public and agencies to use it programatically.[^4]

So, if you are developing a public facing service, ask yourself "what APIs could we expose? What registers should exist to run this service? What registers and shared APIs exist that we should be using?"

## 4. Provide bulk downloads in addition to APIs

For open-data, provide the ability to download bulk datasets in addition to APIs. Work to understand the needs of non-developers (for example statisticians, academics and data scientists).

> ### Example: Digital driving licences in Argentina
> 
**As already noted, when Argentina was developing it's new digital driving licence, rather than build a single system, it started with an API.**
> 
> "The agency still has the data but pushes miArgentina an image with QR code and digital signature via an API. Eventually, we want every agency to be an API. The next areas we are looking at are car insurance, vehicle ownership and disability certificates."
> 
> "The future of government digital services is transforming government into a public API where companies and citizens can build, connect and interact. That’s building government as a platform, or better, as a service"
> 
> — Daniel Abadie - Subsecretario de Gobierno Digital, Secretaría de Gobierno de Modernización (Argentina)
{:.box}

[^1]:   Etalab, "Foire aux questions - adresse.data.gouv.fr", [https://adresse.data.gouv.fr/faq](https://adresse.data.gouv.fr/faq). Retrieved 8th June 2019.

[^2]:   "alphagov/open-standards", GitHub, [https://github.com/alphagov/open-standards](https://github.com/alphagov/open-standards). Retrieved 5th June 2019.

[^3]:   Mike Bracken, “Argentina just made driving licences digital”, Public Digital blog, 12th February 2019, [https://public.digital/2019/02/12/argentina-just-made-driving-licences-digital/](https://public.digital/2019/02/12/argentina-just-made-driving-licences-digital/)

[^4]:   U.S. Department of Justice, "Developer resources", [https://www.foia.gov/developer/](https://www.foia.gov/developer/). Retrieved 8th June 2019.

