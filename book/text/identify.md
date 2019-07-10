# Identifying platforms

Platforms solve problems once, meeting the _common_ needs of users, rather than addressing the same problem multiple times, and in slightly different ways. Those users might be elsewhere in government, in a different tier of government or outside government altogether (for example, a private company or charity).

Your organization will need to prioritize three things to help it identify where there is a genuine opportunity to do this, and where the opportunity is purely superficial:

1. The capability to identify common needs and duplication.
2. Creating clear routes for 'point solutions' from specific products to develop into more general platforms.
3. An understanding of what the right level of abstraction is for a platform  (good platforms do one thing well).

## 1. Identify common needs and duplication

Chances are you are already aware of lots of duplication. It might be multiple services all using different payment systems or address lookups. It might be developers from different teams creating their own login system or hosting setup. In fact, this seems to be the normal state of most organizations developing digital services.

However, just hoping that shared APIs, components and registers will emerge organically from this is unlikely to lead to results. For example, no shared components, APIs or registers emerged from the UK Government Digital Service's _Exemplar_ programme (which saw teams setup across government to redesign digital services).

There is no single approach to doing this, but approaches you might like to consider include:

* Conducting interviews and surveys to understand where common needs might exist.[^1]
* Using [Wardley Mapping](#) to identify duplication.[^2]
* Use governance processes, such as service standard assessments, to collect data about common needs.[^3]
* Review legislation and guidance to identify where one service might benefit from API access to another.
* Review code repositories to identify teams working on the same problem.
* Create a service map or user-journey map and use it to identify common needs.[^4]
* Create a map of the data ecosystem and use it to identify common needs, and datasets that can be adapted into common registers.[^5]

Regardless of approach, all these activities take some time and effort, and will be competing against other priorities. So, make it clear where responsibility to spot common needs and duplication across teams lies.

## 2. Provide a path from products to platforms

A less top-down approach than identifying common needs and duplication is to ensure there are clear routes for 'point solutions' from individual products to develop into shared platforms. A point solution is something that has been developed as part of a single service, that might be useful as a more general platform for multiple services.

For example, the authentication platform, Login.gov, started life as a larger project called [MyUSA](#), which aimed to provide a single account and to do list for interacting with government. The authentication part of the project was developed into login.gov by 18F and the United States Digital Service.[^6]

Another example is the letter printing feature of the GOV.UK Notify messaging platform. It makes use of the spare printing capacity at the UK driving licence agency's secure printing facility that was created when printed 'tax discs' were abolished.[^7]

This approach is similar to that taken by many teams at commercial platform companies, where problems are first solved within product teams, but then supported with staff and funding to turn them into more general solutions.

Within Google, setting up a new team is often off the back of what is already happening organically. Google tends to create a set of core, high-level values while allowing space to innovate. Things that are mandated are really high-level, rather than day-to-day - everything rolls-up to a higher objective.[^8]

For commercial services, the 'route to market' is potentially clearer - for example, an Amazon platform can ultimately appear in the AWS dashboard alongside the company's other offerings where developers can use (and pay) for it. For the approach to be a success, teams working in government will need to be supported to generalize their point-solutions into platforms.

## 3. Identify real-world platforms

Platforms normally get talked about in terms of shared digital capabilities – things like hosting, identity or payments. As the GOV.UK Notify printing example above and commercial platforms like Grab (a broker for motorbike taxis in South East Asia) and JustPark (a broker for car parking spaces in the UK) show, it is possible to put platform-like capabilities around physical goods and services.

Most governments operate some public-facing offices – places like tax offices or labour exchanges. As with many digital services, these only tend to offer the services related to the part of government that owns them: you can’t get help filling out a passport application at a tax office. What if local offices were seen as a shared capability for any government service that needs to talk to people face-to-face? Or a place to take cash payments for people without bank accounts?

Understand where there might be opportunities to build a platform around fragmented, real-world capabilities.

## 4. Get the level of abstraction right

Developing a collective understanding of what makes a good platform is important. A general rule is that if a system is trying to do multiple things, or is highly customizable, it probably isn't a good platform. Platforms generally do one thing well - for example send a message, check the status of an application, verify a fact or geocode an address - small pieces loosely joined, rather than monoliths that try to handle every edge-case or be too smart.

It's worth noting how many of the platforms on the Amazon Web Services Dashboard start with the word 'simple', and generally how the services offered by AWS, Google Cloud and Twillio and other commercial platform providers are focused on a clear task.

Simple platforms are easier for developers to use because it is clear exactly what they do. Simple platforms also create less hard dependencies, making it easier for developers to replace them at a later date.

> ### Example: Prison visits and the potential for a booking platform, UK
> 
> **In the UK, the Ministry of Justice developed a service called ‘Visit someone in Prison’ which allows someone to book a slot to visit a prisoner. Initially, the team thought there might be a route to developing a more general ‘booking platform’, but this turned out to be the wrong level of abstraction.**
> 
> "Good platforms abstract away a clearly-defined problem. We found that ‘Bookings’ weren’t a clearly-defined thing and, typically, their definition was coupled to the nature of the wider process or organization they’re part of."
> 
> "That means that any 'booking platform' has to be able to be configured to handle those organizations’ processes and systems, which could be as simple as meeting room bookings (one person can book a meeting room at a time, and they specify the duration) or as complex as booking prison visits (each prison specifies its visit slots and their capacities, visitors may not be allowed to be present with prisoners who aren’t the person they’re visiting, and more)."
> 
> "Often, the back-ends that handle these bookings are also already tightly integrated into other parts of the organization, so they can’t simply be replaced with a new platform. Not only that, but this complexity also dramatically changes the interface that the user needs to see."
> 
> "Once we came to realize all of the factors that play into bookings, we concluded a single ‘booking platform’ wasn’t really something that could exist."
> 
> — Steve Marshall, Head of Hosting and Digital Operations, Ministry of Justice (UK)
{:.box}

[^1]:   In the UK, the Government Digital Service conducted 150 interviews with teams across government with the aim of understanding their common needs. It led GDS to understand they should prioritize a form building platform over one that, for example, accepted payments from the public, because more services needed it. Richard Pope, "Interview with Will Myddelton – UK Government as a Platform programme", 29th October 2018, [https://medium.com/platform-land/interview-with-will-myddelton-government-as-a-platform-3aff4ebcb3e8](https://medium.com/platform-land/interview-with-will-myddelton-government-as-a-platform-3aff4ebcb3e8)

[^2]:   Wardley Mapping is an approach to visualising the components required to deliver a service. Simon Wardley, "An introduction to Wardley (Value Chain) Mapping", bits or pieces?, 2nd February 2015, [https://blog.gardeviance.org/2015/02/an-introduction-to-wardley-value-chain.html](https://blog.gardeviance.org/2015/02/an-introduction-to-wardley-value-chain.html)

[^3]:   The Government Digital Service identified potential teams to work with  to help identify platforms from 'service assessments', which are a step in the governance process for all new digital services. Richard Pope, "Interview with Will Myddelton – UK Government as a Platform programme", 29th October 2018, [https://medium.com/platform-land/interview-with-will-myddelton-government-as-a-platform-3aff4ebcb3e8](https://medium.com/platform-land/interview-with-will-myddelton-government-as-a-platform-3aff4ebcb3e8)

[^4]:   The UK Ministry of Justice created a visual map of all the activities that take place in the justice system, agnostic from the organizations who run them. Mike Bracken, "Mapping new ideas for the digital justice system", Government Digital Service Blog, 18th August 2015, [https://gds.blog.gov.uk/2015/08/18/mapping-new-ideas-for-the-digital-justice-system-2/](https://gds.blog.gov.uk/2015/08/18/mapping-new-ideas-for-the-digital-justice-system-2/)

[^5]:   The Open Data Institute have developed a process for documenting and mapping data ecosystems. Open Data Institute, "Mapping data ecosystems", 23rd March 2018,[https://theodi.org/article/mapping-data-ecosystems/](https://theodi.org/article/mapping-data-ecosystems/)

[^6]:   18F, "18F/myusa", [https://github.com/18F/myusa](https://github.com/18F/myusa). Retrieved 26th June 2019.

[^7]:   @yahoo_pete (Pete Herlihy), "One of the coolest things about this, is that we made a deal with the DVLA to use their secure, modern on-site print facilities for our letter fulfilment. Having stopped printing tax discs etc a few years back, they had capacity. And we could maximise the savings to taxpayers.", 16th April 2019, [https://twitter.com/yahoo\_pete/status/1118245112482598912?s=12](https://twitter.com/yahoo_pete/status/1118245112482598912?s=12)

[^8]:   Interview, Dr Adam Connors, Senior Google Engineering Manager
