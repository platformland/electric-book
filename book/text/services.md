# Designing services on-top of platforms

The way services get created changes in a platform ecosystem. Rather than being built from scratch, they are assembled from common components.

This characteristic, used in combination with a service design approach, means new types of service could become possible (or at least much simpler to create). These include services that allow people to interact with multiple parts of government at the same time, real-time services, and services from the public, private and third sector that overlap and complement each other.

## 1. Design services, not policies

In a platform ecosystem, designing new services largely becomes a job of joining together platforms. With this reduced effort and reduced duplication comes the potential to save time and money. However, increased efficiency is not the most significant opportunity.

The biggest opportunity is the potential for radically better public services. That's because it does not just become simpler and quicker to design services, it also becomes simpler to design new types of service that are designed around the needs of a user rather than the organizational structure of government.[^1] Looking around the world, we can begin to see that approach happening. 

Estonia is starting to design new services around 'life events', like having a child, that transcend the boundaries of government agencies. They can do this because of the common cross-government data infrastructure they have developed.[^2] Singapore's GovTech agency is following a similar approach and has developed a "Moments of Life" service.[^3]
  
The UK government Service Standard (which all new government services must meet) includes the following requirement for teams designing services to work beyond the boundaries of an individual government agency:

> "Work towards creating a service that solves one whole problem for users, collaborating across organizational boundaries where necessary"[^4]

Also in the UK, the different steps needed to complete a task like 'employing someone' or 'learning to drive' are organized in one place on the GOV.UK website, regardless of which government agency a user has to interact with.[^5]

Take advantage of the opportunity of platforms design services to solve _whole problems_ for people. Look for opportunities to make end-to-end service design part of official guidance and governance processes.

## 2. Think of services as built from many platforms

Just as platforms are part of many services, so services are made from many platforms. This means that a team designing the service can focus on the areas that are unique to the domain they are working in, and prototype a working service much faster.

A great example is the Christmas tree permitting service operated by the U.S. Forest Service that allows people to legally harvest a Christmas tree for their home from a national forest. The service uses pay.gov (to take payments), login.gov (for authentication), is hosted on cloud.gov, and uses a generic permits API.[^6] [^7]. The user interface is built using the U.S. Web Design system as a base.[^8]

The other implication of this one-to-many principle is that a service team will not have control over the entire user journey, and this may take some adjustment for teams used to controlling the totality of the user experience.

When designing services that use platforms, understand what existing platforms you could use to develop your service. Work in the open and maintain good communications with teams operating platforms so you can ensure you understand any upcoming changes.

## 3. Allow for multiple, overlapping services, built on a common platform

Historically, policymakers have had a couple of clear, choices to make when it comes to the delivery of a service to the public. Should it be delivered centrally or locally? Should it be done by the private sector or the public sector? A healthy platform ecosystem could start to turn those choices into false choices.

That's because it allows governments to follow both a retail approach to providing services (where government offers a public-facing service) **and** a wholesale one (where the charities and private companies also provide services).[^9]

Because platforms do the "heavy lifting", it becomes more feasible to build multiple services on top of them. These services could be provided by any layer of government, and by commercial or third sector organizations, in such a way that is ok if they overlap, complement or duplicate each other.

One recent example of this wholesale and retail approach is recreation.gov, which is a public-facing government service for finding and booking campsites and tours on federal land. It is built on an API that is also used by a commercial vacation website.[^10] These services overlap and to some extent compete with each other, but serve slightly different audiences.

It could also become much simpler to interact with multiple layers of government at once in a single service. Designing services that allow people to interact with central and local government within a single service.

## 4. Design real-time services (but be cautious of the risks)

One of the characteristics of modern digital services is that they operate in real-time. If you want to buy something on Amazon, you see if it’s out-of-stock immediately, and pricing on Uber responds to demand in real-time. The teams operating those services also benefit from real-time feedback loops so they can see where users are getting stuck and what’s not working as it should.

Registers, and shared APIs should make these things simpler for government services, so that, for example, users could track the exact point in the process their welfare application is at.

Real-time services will also come with new risks. For example, the Indian hotel chain Oyo plans to share guests check-in data with state governments in real-time (replacing an existing, manual process). The company's motivation is to reduce errors and make things faster for hoteliers and guests. But it has also raised concerns from privacy campaigners about the affordances and unintended consequences of such as system.[^11] [^12] [^13]

When designing real-time services, a key decision for services designers is going to be where there should be a human in the loop.

Design services that take advantage of the real-time nature of platforms, but consider negative consequences as well as opportunities.

## 5. Design event-driven services

Lots of government services require people to report when things in their life change, and this places a lot of responsibility on the user - they need a good mental model of the service to know what to report when and how. (The UK's Universal Credit benefits system requires people to internalize over 30 types of change-of-circumstance!)[^14]

A different approach is to design services that both respond to events, and make use of data held elsewhere. Trust and identity systems, along with shared APIs and registers could make it simpler to design services that forgo the need for lots of secondary digital transactions (things like 'update this', 'report that', 'change this', 're-apply for that'.)

Rather than placing the burden on users, look for opportunities to use APIs and registers to design services that proactively meet the needs of users based on events.

> ### Example: Building U.S. Forest Service Christmas tree permits service on-top of platforms
> 
> The Christmas tree permitting service operated by the U.S. Forest Service lets people to legally harvest a Christmas tree for their home from a national forest. It's built on top off several platforms, including pay.gov and cloud.gov.
> 
> "Before Open Forest, there was no online purchasing option for these permits, limiting the public to buying permits at mostly remote USFS district offices or sometimes from local vendors during weekday business hours. From launch to the the end of the holiday season, Open Forest sold nearly 5,000 permits across the four pilot forests."
> 
> "Though 18F has delivered many products to production since its founding in 2014, this is our first product to include payment functionality. Purchasers can use their credit card, debit card, or bank account number to pay for a permit through the U.S. Department of the Treasury’s Pay.gov. Leveraging this existing service helped us implement a modular approach; our product team focused on the unique Christmas tree sale process, rather than reinventing how to make a secure payment. For the Forest Service staff in the district offices, it minimized the administrative burden of processing large sums of cash."
> 
> "Why did we design and build a print-at-home solution rather than a mobile one? With limited cellular service and temperatures dropping below freezing that can quickly drain a mobile phone battery, a digital solution might not be that durable."
> — Laura Gerhardt, 18F (extract from a blog post) [^15]
{:.box}

[^1]:   See this blog post by former UK Head of Design for Government for a fuller exploration of this idea. Lou Downe, "Better services with patterns and standards", Government Digital Service Blog, 6th August 2015, [https://gds.blog.gov.uk/2015/08/06/better-services-with-patterns-and-standards/](https://gds.blog.gov.uk/2015/08/06/better-services-with-patterns-and-standards/)

[^2]:   Sam Trendall, "We have only scratched the surface’ – Estonia’s CIO on what’s next for the world’s most celebrated digital nation", PublicTechnology.net, 18th February 2019, [https://publictechnology.net/articles/features/‘we-have-only-scratched-surface’-–-estonia’s-cio-what’s-next-world’s-most](https://publictechnology.net/articles/features/%E2%80%98we-have-only-scratched-surface%E2%80%99-%E2%80%93-estonia%E2%80%99s-cio-what%E2%80%99s-next-world%E2%80%99s-most)

[^3]:   GovTech Singapore, "The Tech Behind The Moments Of Life (Families) App", [https://www.tech.gov.sg/media/technews/the-tech-behind-the-moments-of-life](https://www.tech.gov.sg/media/technews/the-tech-behind-the-moments-of-life). Retrieved 13th June 2019.

[^4]:   HM Government, "Service Standard", [https://www.gov.uk/service-manual/service-standard](https://www.gov.uk/service-manual/service-standard). Retrieved 5th June 2019.

[^5]:   Sam Dub and Gabrielle Acosta, "Building a better GOV.UK, step by step", Government Digital Service Blog, 17th October 2018, [https://gds.blog.gov.uk/2018/10/17/building-a-better-gov-uk-step-by-step/](https://gds.blog.gov.uk/2018/10/17/building-a-better-gov-uk-step-by-step/)

[^6]:   18F, "18F/fs-open-forest Wiki", GitHub,[https://github.com/18F/fs-open-forest/wiki](https://github.com/18F/fs-open-forest/wiki). Retrieved 5th June 2019.

[^7]:   18F, "Ongoing site architecture 18F/fs-open-forest Wiki", GitHub, [https://github.com/18F/fs-open-forest/wiki/Ongoing-site-architecture](https://github.com/18F/fs-open-forest/wiki/Ongoing-site-architecture). Retrieved 5th June 2019.

[^8]:   18F, "18F/fs-fork-uswds: The Forest Service fork of U.S. Web Design System is a design system for building fast, accessible, mobile-friendly Forest Service websites.", GitHub, [https://github.com/18F/fs-fork-uswds](https://github.com/18F/fs-fork-uswds). Retrieved 5th June 2019.

[^9]:   Aneesh Chopra and Nick Sinai, "Wholesale Government: Open Data and APIs", Medium, 9th April 2015, [https://medium.com/@ShorensteinCtr/wholesale-government-open-data-and-apis-7d5502f9e2be](https://medium.com/@ShorensteinCtr/wholesale-government-open-data-and-apis-7d5502f9e2be)

[^10]:  A recent example is recreation.gov, which has a public facing website for finding and booking campsites and tours on federal land. It also has an API that is used by commercial websites to do the same thing. (I think this article is a bit unfair on the government run website). Lindsey Smith, "Booking campsites on Recreation.gov is a mess. Here’s the solution", San Francisco Chronicle, 4th march 2019, [https://www.sfchronicle.com/travel/article/Recreation-gov-is-a-mess-Here-s-the-solution-13655884.php](https://www.sfchronicle.com/travel/article/Recreation-gov-is-a-mess-Here-s-the-solution-13655884.php)

[^11]:  "Oyo to share customers' arrival, departure details with authorities", Business Today, 15th January 2019, [https://www.businesstoday.in/buzztop/buzztop-corporate/oyo-to-share-customers-arrival-departure-details-with-authorities/story/310152.html](https://www.businesstoday.in/buzztop/buzztop-corporate/oyo-to-share-customers-arrival-departure-details-with-authorities/story/310152.html)

[^12]:  "Oyo Rooms wants to share digital record of your check-ins with government", India Today, 15th January 2019, [https://www.indiatoday.in/technology/news/story/oyo-rooms-wants-to-share-digital-record-of-your-check-ins-with-government-1431439-2019-01-15](https://www.indiatoday.in/technology/news/story/oyo-rooms-wants-to-share-digital-record-of-your-check-ins-with-government-1431439-2019-01-15)

[^13]:  @internetfreedom /  Internet Freedom Foundation (IFF), "Everyday we loose more of our privacy. This also means a live update the next time you check into a hotel room. Without a warrant or a legal request, instantaneous. Scalable, deeper, richer and in real time.", 15th January 2019, [https://mobile.twitter.com/internetfreedom/status/1085169410799751168](https://mobile.twitter.com/internetfreedom/status/1085169410799751168)

[^14]:  Citizens Advice, "Check if a change affects your Universal Credit", [https://www.citizensadvice.org.uk/benefits/universal-credit/what-youll-need-to-do-on-universal-credit/check-if-a-change-affects-your-universal-credit/](https://www.citizensadvice.org.uk/benefits/universal-credit/what-youll-need-to-do-on-universal-credit/check-if-a-change-affects-your-universal-credit/). Retrieved 5th June 2019.

[^15]:  Extract from a blog post published by Laura Gerhardt published after the launch of the service. Laura Gerhardt, "Buying Christmas tree permits online with Open Forest", 18F Blog, 12th February 2019, [https://18f.gsa.gov/2019/02/12/open-forest-launch-post/](https://18f.gsa.gov/2019/02/12/open-forest-launch-post/)
