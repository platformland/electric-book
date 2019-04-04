---
title: "How to identify platforms"
---

# How to identify platforms

Platforms solve problems once and meet the common needs of different users, rather than addressing the same problem multiple times, in slightly different ways, for each type of user. Organziations will need to prioritize three things to help them identify where there is a genuine opportunity to do this, and where the opportunity is superficial:

1. The capability to identify common needs and duplication
2. Clear routes for 'point solutions' from specific products to develop into more general platforms
3. A culture where teams are encouraged to think about users beyond their own domain

## Common needs and duplication

In the UK GDS conducted 150 interviews with teams across government with the aim of understanding their common needs. It led GDS to understand they should prioritize a form building platform over one that, for example, accepted payments from the public, because more services needed it.

Other approaches include:

* Use [Wardley mapping](https://blog.gardeviance.org/2015/02/an-introduction-to-wardley-value-chain.html) to identify duplication
* Use governance processes, such as service assessments, to collect data about common needs
* Review legislation and guidance to identify where one service might benefit from API access to another
* Review code repositories to identify teams working on the same problem
* Organise a survey of service teams across government and beyond

Whichever approach your organization takes, make it someone's explicit job to spot common needs and duplication. Just leaving it to happen organically is unlikely to lead to results.

## From products to platforms

A less top-down approach is to provide clear routes and support for 'point solutions' from individual products to develop into shared platforms.

For example, the authentication platform, Login.gov, started life as a larger project called [MyUSA](https://web.archive.org/web/20130423114036/http://www.whitehouse.gov/innovationfellows/myusa), which aimed to provide a single account and todo list for interacting with government. The authentication part of the project was developed into login.gov by 18F and the United States Digital Service.

This is similar to the approach taken by many teams at Google and Amazon, where problems are first solved within product teams, but then supported with staff and funding to turn them into general solutions.

Other approaches include:

* Making it part of a governance process that teams building products and services should be able to explain potential how parts of their service might be reused
* Identifying under-utilised resources, such as empty offices or printing services and wrap them in an API to turn them into a generalized resource
* Ensuring code from different teams can be discovered and shared
* Speculatively creating public APIs that allow other teams to build on top of a product

Crucially though, product teams need to have permission and support to work in this way. There also needs to be a clear 'route to market'. For commercial services this is clear - an Amazon platform can ultimately appear in the AWS dashboard alongside the company's other offerings where developers can start to experiment with it. For government platforms, there needs to be an equivalent.

## Culture

Developing a culture where teams think about users beyond their domain is also important. Without that in place, any of the approaches above could just become a 'tick-box exercise' [^1].

[^1]: Tick-box exercise/culture is one where things are done for bureaucratic expediency rather than serving any actual purpose

## Platforms do one thing well

In the UK, the Ministry of Justice developed a service called 'Visit someone in Prison' which allows someone to book a slot to visit a prisoner. Initially, it was thought that might be a route to developing a more general 'booking platform'. However, the rules around prison visits were found to be too complex and domain specific. Also, it would have needed to integrate with different back-office calendar systems.

> Quote goes here
{:.box}

A good general rule is that: if a system encapsulates is trying to do multiple things, or is highly customizable, it probably isn't a platform. Platforms generally do one thing well.

## Actions

* Create a list of services from across government that can be used as a starting point for identifying teams to work with
* Run a Wardley Mapping workshop
* Review governence processes to identify new opportunities to collect 
data
* Encourage people to share their work in the open and talk about the potential for new platforms
* Create a single place to document government platforms (it can be as simple as a shared, public document to start with)