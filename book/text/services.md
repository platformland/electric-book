# Designing services on-top of platforms

The way services get created changes in a platform ecosystem. Rather than (mostly) being built from scratch, they are assembled from common components.

This characteristic, in combination with a service design approach means new types of service could become possible (or at least much simpler to create): services that allow people to interact with multiple parts of government at the same time; real-time services; and services from the public, private and third sector that overlap and complement each other.

## 1. Design services, not policies

With platforms, designing new services largely becomes a job of joining together existing systems. With this reduced effort and duplication comes the potential to save time and money. However, increased efficiency is not the most significant opportunity arising from Government as a Platform. The biggest opportunity is the potential for radically better public services. That's because it does not just become simpler and quicker to design services, it also becomes simpler to design new types of service that are designed around the needs of a user rather than the organizational structure of government.[^1]

Estonia is starting to design new services around 'life events', like having a child, that transcend the boundaries of government agencies. They can do this because of the common cross-government data infrastructure they have developed.[^2]
  
The UK government Service Standard (which all new government services must meet) includes the following requirement for teams designing services to work beyond the boundaries of an individual government agency:

> Work towards creating a service that solves one whole problem for users, collaborating across organizational boundaries where necessary.

The GOV.UK website is a single place to access government services, with the different steps needed to complete a task like 'employing someone' or 'learning to drive' organized in one place regardless of which government department a user needs to interact with.[^3]

Take advantage of the opportunity of platforms by rapidly prototyping and testing services to solve whole problems for people. Look for opportunities to make end-to-end service design part of official guidance and governance processes.

## 2. Think of services as built from many platforms

Just as platforms are part of many services, so services are made from many platforms.

A great example is the Christmas tree permitting service operated by the U.S. Forest Service that allows people to legally harvest a Christmas tree for their home from a national forest. The service is comprised of pay.gov top take payment, login.gov for authentication is hosted on cloud.gov, and uses a generic permits API built by 18F.[^4] [^5]. The user interface is built using the a variant of the U.S. Web Design system.[^6]

This approach means that the team designing the service can focus on the areas that are unique to the domain they are working in, and prototype a working service much faster. But it also means that the team will not have control over the entire user journey.  

Work in the open and maintain good communications with teams operating platforms, so you can ensure you understand any upcoming changes.

## 3. Allow for multiple, overlapping services, built on a common platform

Historically, policymakers have had a couple of clear, binary choices to make when it comes to the delivery of services to the public. Should this be delivered centrally or locally? Should this be done by the private sector or the public sector? A healthy platform ecosystem could start to turn those choices into false ones, allowing governments to follow both a wholesale and a retail approach to providing services.[^7]

Because platforms do the heavy lifting, it becomes possible to build multiple services on top of them. Services can (in theory) be provided by any layer of government, and by commercial or third sector organizations in such a way that is ok if they overlap, complement and duplicate each other. It could also become much simpler to interact with multiple layers of government at once in a single service.

One recent example is recreation.gov, which has a public facing website for finding and booking campsites and tours on federal land. It also has an API that is used by commercial websites to do the same thing.[^8] These services overlap and to some extent compete with each other, but that’s ok, so long as there are clear rules and standards that services follow.

## 4. Design real-time services (but be cautious of the risks)

One of the characteristics of modern commercial digital services is that they operate in real-time. If you want to buy something on Amazon, you see if it’s out-of-stock immediately. Pricing on Uber responds to demand in real-time. Teams operating those services benefit from real-time feedback loops so they can see where they are getting stuck and what’s not working as it should.

Registers, and shared APIs that expose the business logic of government should make these things possible for government services, so that, for example, users can track the exact point in the process their visa application is at.

Real-time services will come with new risks. For example, the Indian hotel chain Oyo plans to share guests check-in data with state governments in real-time (replacing an existing, manual process). The company's motivation is to reduce errors and make things faster for hoteliers and guests. But this has raised concerns from privacy campaigners about the affordances of such as system.[^9] [^10] [^11]

Real-time, programmatic, company formation and dissolution could also become a possibility, and the risks of that have (as yet) only been speculated about.[^12]

When designing real-time services, a key decision for services designers is going to be understanding where there needs to be a human in the loop.

## 5. Design event-driven services

Lots of government services require their people to report when things in their life change. This places a lot of responsibility on the user - they need a good mental model of the service to know what to report when they should do it and how. (The UK's Universal Credit benefits system requires people to internalize over 30 types of change-of-circumstance.)[^13]

A different approach is to design services that both respond to events, and make use of data held elsewhere. Trust and identity systems, along with shared APIs and registers could make it simpler to design services that forgo the need for lots of secondary digital transactions (Things like 'update this', 'report that', 'change this', 're-apply for that'.)

[^1]:   See this blog post by former UK Head of Design for Government for a fuller exploration of this idea. Lou Downe, "Better services with patterns and standards", Government Digital Service Blog, 6th August 2015, [https://gds.blog.gov.uk/2015/08/06/better-services-with-patterns-and-standards/](https://gds.blog.gov.uk/2015/08/06/better-services-with-patterns-and-standards/)

[^2]:   Sam Trendall, "We have only scratched the surface’ – Estonia’s CIO on what’s next for the world’s most celebrated digital nation", PublicTechnology.net, 18th February 2019, [https://publictechnology.net/articles/features/‘we-have-only-scratched-surface’-–-estonia’s-cio-what’s-next-world’s-most](https://publictechnology.net/articles/features/%E2%80%98we-have-only-scratched-surface%E2%80%99-%E2%80%93-estonia%E2%80%99s-cio-what%E2%80%99s-next-world%E2%80%99s-most)

[^3]:   Sam Dub and Gabrielle Acosta, "Building a better GOV.UK, step by step", Government Digital Service Blog, 17th October 2018, [https://gds.blog.gov.uk/2018/10/17/building-a-better-gov-uk-step-by-step/](https://gds.blog.gov.uk/2018/10/17/building-a-better-gov-uk-step-by-step/)

[^4]:   18F, "18F/fs-open-forest Wiki", GitHub,[https://github.com/18F/fs-open-forest/wiki](https://github.com/18F/fs-open-forest/wiki). Retrieved 5th June 2019.

[^5]:   18F, "Ongoing site architecture 18F/fs-open-forest Wiki", GitHub, [https://github.com/18F/fs-open-forest/wiki/Ongoing-site-architecture](https://github.com/18F/fs-open-forest/wiki/Ongoing-site-architecture). Retrieved 5th June 2019.

[^6]:   18F, "18F/fs-fork-uswds: The Forest Service fork of U.S. Web Design System is a design system for building fast, accessible, mobile-friendly Forest Service websites.", GitHub, [https://github.com/18F/fs-fork-uswds](https://github.com/18F/fs-fork-uswds). Retrieved 5th June 2019.

[^7]:   Aneesh Chopra and Nick Sinai, "Wholesale Government: Open Data and APIs", Medium, 9th April 2015, [https://medium.com/@ShorensteinCtr/wholesale-government-open-data-and-apis-7d5502f9e2be](https://medium.com/@ShorensteinCtr/wholesale-government-open-data-and-apis-7d5502f9e2be)

[^8]:   A recent example is recreation.gov, which has a public facing website for finding and booking campsites and tours on federal land. It also has an API that is used by commercial websites to do the same thing. (I think this article is a bit unfair on the government run website). Lindsey Smith, "Booking campsites on Recreation.gov is a mess. Here’s the solution", San Francisco Chronicle, 4th march 2019, [https://www.sfchronicle.com/travel/article/Recreation-gov-is-a-mess-Here-s-the-solution-13655884.php](https://www.sfchronicle.com/travel/article/Recreation-gov-is-a-mess-Here-s-the-solution-13655884.php)

[^9]:   "Oyo to share customers' arrival, departure details with authorities", Business Today, 15th January 2019, [https://www.businesstoday.in/buzztop/buzztop-corporate/oyo-to-share-customers-arrival-departure-details-with-authorities/story/310152.html](https://www.businesstoday.in/buzztop/buzztop-corporate/oyo-to-share-customers-arrival-departure-details-with-authorities/story/310152.html)

[^10]:  "Oyo Rooms wants to share digital record of your check-ins with government", India Today, 15th January 2019, [https://www.indiatoday.in/technology/news/story/oyo-rooms-wants-to-share-digital-record-of-your-check-ins-with-government-1431439-2019-01-15](https://www.indiatoday.in/technology/news/story/oyo-rooms-wants-to-share-digital-record-of-your-check-ins-with-government-1431439-2019-01-15)

[^11]:  @internetfreedom /  Internet Freedom Foundation (IFF), "Everyday we loose more of our privacy. This also means a live update the next time you check into a hotel room. Without a warrant or a legal request, instantaneous. Scalable, deeper, richer and in real time.", 15th January 2019, [https://mobile.twitter.com/internetfreedom/status/1085169410799751168](https://mobile.twitter.com/internetfreedom/status/1085169410799751168)

[^12]:  OpenCorperates, "Fireflies and algorithms — the coming explosion of companies", Medium, 24th October 2018, [https://medium.com/@opencorporates/fireflies-and-algorithms-the-coming-explosion-of-companies-9d53cdb8738f](https://medium.com/@opencorporates/fireflies-and-algorithms-the-coming-explosion-of-companies-9d53cdb8738f)

[^13]:  Citizens Advice, "Check if a change affects your Universal Credit", [https://www.citizensadvice.org.uk/benefits/universal-credit/what-youll-need-to-do-on-universal-credit/check-if-a-change-affects-your-universal-credit/](https://www.citizensadvice.org.uk/benefits/universal-credit/what-youll-need-to-do-on-universal-credit/check-if-a-change-affects-your-universal-credit/). Retrieved 5th June 2019.
