DroughtMonitor v2 requirements document
=======================================
This document will outline the requirements of a prototype personal drought monitor that could be used in conjunction with a media organization's effort to personalize a mass weather event like drought.


Product overview, use cases, user profiles
------------------------------------------
Media organizations covering large scale climate events, such as drought, often seek to personalize those events through personal stories of people impacted by those events. Those personalized stories -- by design -- live in the realm of anecdote, but often the media organization wishes they could go further. Through the use of inexpensive sensors, micro controllers and wireless technologies, those personal stories can be bolstered with data unique to that individual. That data can then be aggregated to paint a broader picture of the situation, melding the personal with the communal, the unique observations of a person with measurable and verifiable data from a sensor. 

**Use case**

A media organization wants to engage its readers and users to produce a more complete story about an event, in this case, a drought. The media organization would like this product to measure soil moisture conditions at an individual reader's location and report it back to the news organization in a centralized system. The news organization will then use the personal stories and data to create an interactive data visualization that melds personal narrative with personal data.

**User profiles**

1. A single man, aged 68, concerned for his local environment and the toll that drought is taking on it, and is a dedicated reader of the media organization. He wants to take part, but has no experience with electronics.
2. A family of four, with middle school aged children interested in the sciences. They have previous experience with the Arduino platform, and are interested in citizen science efforts.
3. An engineer who is active in her local Maker space. She has significant experience with electronics and is interested in getting others involved in the project through her Maker space.


Functional requirements
-----------------------
This project will seek to produce three prototypes. Those three prototypes will handle details of the implementation different. Details include how they are made, how a user reports data to the news organization and how the device is manufactured and distributed. Based on field testing, these prototypes will be narrowed to functional products that can be presented to a media organization. 

The operational requirements for the devices are as follows:

1. It must record soil moisture conditions at a location at least once a day.
2. It must record the time said conditions were recorded. 
3. It must be able to stay in the field for 30 days without requiring batteries to be changed.
4. It must be able to withstand various weather conditions, including high heat, direct sunlight and rain.

Aspirational but not operational requirements include:

1. Record temperature and relative humidity at the location at the same time soil moisture is recorded.
2. Solar power battery recharge.

Each individual prototype will now be described:

**Prototype 1**

Prototype 1 will be the most simple, will require the most intervention on the part of the user, and could be assembled by the media organization to be given to participants in the effort, or sold as a kit put together by the media organization. As such, it will need to be simple to manufacture. 

In addition to the above listed requirements, Prototype 1 will:

1. Record data to a microSD card and require the user to upload a text file to a website. It will have no wireless capabilities.
2. Require as few solders as possible. If possible, a zero solder model is desirable. 
3. Will cost less than $20 per unit to produce.

**Prototype 2**

Prototype 2 will be the most expensive and will likely require user intervention to set up. It too could be assembled by the media organization and be given to the participants in the effort, or sold as a kit. It will require a more significant documentation effort, particularly if the individual user has secured their home wifi. 

In addition to the above listed requirements, Prototype 2 will:

1. Report data directly to an online data store via API.
2. Record data to a microSD card as backup in case of wifi failure.
3. Contain significant documentation for individual users showing them how to set up their device.
4. Cost less than $40 per unit to produce.

**Prototype 3**

Prototype 3 will use wireless transmission, but not rely upon wifi for that transmission. This will limit issues with setup, but complicate matters with the addition of a base station to receive the data from the sensor. This too could be assembled by the media organization or sold as a kit.

In addition to the above listed requirements, Prototype 3 will:

1. Use a low power wireless transmission protocol such as Xbee to send data from the sensor in the field to a base station stored inside at the users home, where it will be connected to the internet. 
2. Record data to a microSD card as a backup in case of wireless failure. 
3. Contain significant documentation for individual users showing them how to set up their device. 
4. Cost less than $40 per unit to produce.


Usability requirements
----------------------

The significant usability issues inherent in an effort like this are the widely varying technical skills of the participants and unfamiliarity with electronics. In all facets of the development of the prototypes, developers should be mindful of the user profiles listed above. 

1. All prototypes should be easy to assemble to promote user adoption at all levels, and make potential manufacture more feasible.
2. All prototypes should be documented in a beginner-friendly way.
3. All prototypes should be open so more advanced users can hack their own versions.
4. All prototypes must be easy to manipulate -- for example, the microSD card must be easy to remove for all users.


Technical requirements
----------------------

For this project to work, the data must be verified and valid. 

1. Each prototype will be first internally tested in laboratory conditions to validate internally consistent results across devices.
2. Each prototype's data will be validated using industry standard methods to ensure the data coming from them is useful.
3. All uncertainty, error level or data significance will be documented and disclosed.
4. The software will be tested to ensure continued operation.


Timelines and milestones 
----------------------------------------

Prototypes will be completed by May 15. 

Individual timelines and milestones will be determined by each prototype team at the time of assignment. Those timelines and milestones will be spelled out through issue tracking. 
