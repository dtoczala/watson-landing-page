# Welcome to Watson
Cognitive computing can be complex, but we're here to help you make sense of it.  This is a technically focused set of pages that will allow you to explore the technology, see the latest best practices, and help you master cognitive application development.
# Contents
- **[Introduction](https://github.com/dtoczala/watson-landing-page#introduction---getting-started)**
- **[Watson Services and APIs](https://github.com/dtoczala/watson-landing-page#watson-services-and-apis)**
  - [Conversation](https://github.com/dtoczala/watson-landing-page#conversation)
  - [Discovery](https://github.com/dtoczala/watson-landing-page#discovery)
  - [Alchemy API](https://github.com/dtoczala/watson-landing-page#alchemy-api)
  - [Natural Language Understanding (NLU)](https://github.com/dtoczala/watson-landing-page#natural-language-understanding-nlu)
  - [Personality Insights](https://github.com/dtoczala/watson-landing-page#personality-insights)
  - [Speech to Text and Text to Speech (STT/TTS)](https://github.com/dtoczala/watson-landing-page#speech-to-text-and-text-to-speech-stttts)
  - [Tone Analyzer](https://github.com/dtoczala/watson-landing-page#tone-analyzer)
  - [Tradeoff Analytics](https://github.com/dtoczala/watson-landing-page#tradeoff-analytics)
  - [Visual Recognition](https://github.com/dtoczala/watson-landing-page#visual-recognition)
- **[Common Use Cases](https://github.com/dtoczala/watson-landing-page#common-use-cases)**
  - [Chatbots](https://github.com/dtoczala/watson-landing-page#chatbots)
- **[Cognitive Development Topics](https://github.com/dtoczala/watson-landing-page#cognitive-development-topics)**
  - [The Importance of Data](https://github.com/dtoczala/watson-landing-page#the-importance-of-data)
  - [DevOps with Cognitive on Bluemix](https://github.com/dtoczala/watson-landing-page#devops-with-cognitive-on-bluemix)
  - [Testing Approaches and Methods](https://github.com/dtoczala/watson-landing-page#testing-approaches-and-methods)
  - [Watson/Bluemix Security Concerns](https://github.com/dtoczala/watson-landing-page/blob/master/README.md#watsonbluemix-security-concerns)
- **[Common Tips and Tricks](https://github.com/dtoczala/watson-landing-page#common-tips-and-tricks)**
  - [Bluemix Tips and Tricks](docs/bluemix_tipstricks.md)

---
# Introduction - Getting Started

## The Watson Developer Cloud
The Watson Developer Cloud (WDC) is a collection of cogntive services hosted on the [IBM Bluemix](https://console.ng.bluemix.net/) platform.  They are available as cloud based services.  These services include:
- **[Watson Conversation service](https://console.ng.bluemix.net/catalog/services/conversation/)** - which is used to drive conversations with end users.  Some of the more common use cases include customer care scenarios and chatbots.  Also check out the various Application Starter Kits which uses Watson Conversation to build a chatbot.
- **[Watson Discovery Service](https://console.ng.bluemix.net/catalog/services/discovery/)** - which is used to answer "long tail" questions, catalog knowledge and information, and retrieve relevant documents.  

### References for Further Reading
- [Bluemix tutorial](https://console.ng.bluemix.net/docs/admin/adminpublic.html) - A simple getting started tutorial
- [Cloud Architecture Center](https://www.ibm.com/devops/method/category/architectures?cm_mc_uid=59482719098114889125842&cm_mc_sid_50200000=1488912584) - basic architecture concepts and patterns for Cloud and Cognitive development.
- [Watson Cognitive Developer Certification Study Guide](https://github.com/havasnewyork/IBM-Watson-Developer-Certification-Study-Guide) - a nice guide on GitHub with a nice background on core cognitive principles and concepts.
- [Watson Developer Blog](https://developer.ibm.com/watson/blog/) - don't be fooled by the title, most of the blog entries here are more along the lines of announcements of new capabilities available with Watson.  Some technical content here, but it's good to follow this to remain aware of the new things coming.
- [Building With Watson](https://www.ibm.com/watson/building-with-watson-webinar.html) - source for a series of technical webcasts on a variety of different Watson and cognitive computing topics.

---
# Watson Services and APIs
The following section will focus on the various Watson services and API's, providing links to high quality technical content focused specifically on these services.

## Conversation
The Conversation service allows you to add a natural language interface to your application, to automate interactions with your end users. Common applications include virtual agents and chat bots that can integrate and communicate on any channel or device.  The [text message chatbot](https://www.ibm.com/watson/developercloud/starter-kits.html#text-message-chatbot) on the [Application Starter Kits (ASKs) page](https://www.ibm.com/watson/developercloud/starter-kits.html) is an excellent example of a chatbot application, with code and instructions on how to implement this on [IBM Bluemix](https://console.ng.bluemix.net/).

The tooling used to "develop" the Conversation service consists of three parts.  The first part deals with user intents.  The purpose of intents is to map “what a user says” to “what a user means”. Because of the wide variety of utterances users say to mean the same intent, Watson Conversation leverages deep learning technology to extract intents from utterances. You, as the app developer, have complete control in defining what intents are relevant to your application. Once you’ve defined your list of intents, you need to teach Watson how to recognize these intents by providing it with sample utterances and how they map to these intents. Probably the most common question we get from developers is “how many sample utterances do I need to provide”. While the tool requires a minimum of five sample utterances, the general guideline is “the more the better”. We’ve typically seen good results with 20-30 sample utterances per intent. The key observation is to try and capture real end-user input utterances and then map those to the intents you’ve defined for your application.

The second part handles Entities.  Entities provide specific information that your bot can leverage to provide most relevant response. For example, if the user’s utterance is “I would like to book a flight to Paris”, then the intent is “book_flight” and the entity is “Paris”. You, as the app developer, define the entities that are relevant for your application by providing a list of entity names and for each entity, a list of values and for each value a corresponding list of synonyms.

Once intents and entities are defined in the Conversation service, it is the third part, called Dialog, that actually orchestrates the conversation based on extracted intents and entities, as well as context provided by the application. Context is an extremely important concept as it is the bridge that links the conversation service to your bot (or application). Any information communicated back and forth between the Conversation service and the bot goes across through the context variables. Dialog consists of a number of user defined nodes where each node executes based on whether its condition is true. Think of each node as an “if” condition where the condition checked is based on a combination of intents, entities, and context variables (or any derived variables). If the condition is true, then the node executes; if not, the flow continues to the next node in the dialog. Please note that the order of the nodes is important as the flow executes top to bottom, left to right.

### References for Further Reading
- [Conversation with Alchemy Entity Extraction](https://kozhayasite.wordpress.com/2016/08/27/watson-conversation-with-alchemy-entity-extraction/) - great overview of Conversation concepts, and how to integrate with other Watson capabilities.  Complete with a GitHub repo with sample code.

**Intents**
- [Compund Questions](https://sodoherty.ai/2017/02/06/compound-questions/) - Nice article on a technique for detecting compound questions.
- [Watson in the White and Black Room](https://sodoherty.ai/2017/02/10/watson-in-the-black-and-white-room/) - Quick article on understanding Watson cofidence scores.

**Entities**
- [Improving Your Intents with Entities](https://sodoherty.ai/2017/01/16/improving-your-intents-with-entities/) - an exploration of how intents and entities work together.

**Dialog**
- [Recursive Questions with Conversations](https://ollycox.me/2016/10/21/recursive-questions-with-ibm-watson-conversations/) - a quick post showing how to disambiguate user utterances, without driving the end user crazy.
- [Pattern for Gathering Information with Conversation](https://ollycox.me/2016/11/18/pattern-for-gathering-information-in-ibm-watson-conversations/) - an example (with code) of gathering multiple pieces of information in a Conversation flow.

## Discovery
xxx

### References for Further Reading
None

## Alchemy API
The Alchemy API is being deprecated, and will not be available for the creation of new Alchemy instances on April 7, 2017.  Existing Alchemy API instances will remain functional until March 7, 2018.

Users who utilized Alchemy Language in the past are now encouraged to use the [Natural Language Understanding (NLU)](https://github.com/dtoczala/watson-landing-page#natural-language-understanding-nlu) service.

Users who utilized Alchemy Data News in the past are now encouraged to use the Watson [Discovery](https://github.com/dtoczala/watson-landing-page#discovery) service.

### References for Further Reading
- [How to Migrate from Alchemy Lanaguage to NLU](http://wdc-watson-master.stage1.mybluemix.net/doc/natural-language-understanding/migrating.html) - the official guide for migrating to the NLU service.
- [How to Migrate from Alchemy Data News to Discovery](https://www.ibm.com/watson/developercloud/doc/discovery/migrate-adn.html) - the official guide for migrating to the Watson Discovery service.

## Natural Language Understanding (NLU)
xxx

### References for Further Reading
None

## Personality Insights
xxx

### References for Further Reading
None

## Speech to Text and Text to Speech (STT/TTS)
xxx

### References for Further Reading
None

## Tone Analyzer
xxx

### References for Further Reading
None

## Tradeoff Analytics
xxx

### References for Further Reading
None

## Visual Recognition
The Visual Recognition API is used for vision services.

Often when doing analysis of pictures, it is useful to "tile" the image, and break it down into smaller chunks.  See the link to the Visual Recognition Tile Localization tool, which is a KEY component for segmenting larger images into bite size pieces for Visual Recognition.

### References for Further Reading
- [Visual Recognition Tile Localization](https://github.com/IBM-Bluemix/Visual-Recognition-Tile-Localization) - complete source code for visualizing localized results for a single class, within a single custom classifier using image preprocessing (tiling) techniques, and will run on Bluemix as-is.

---
# Common Use Cases
This section will cover some of the basic patterns and cognitive use cases that are implemented using the Watson services.

## Chatbots

Chatbots are popular right now, and they can help serve a real purpose.  Many customers use them for customer care and customer support scenarios.  They have been integrated into a number of different communications channels, and they can often do the repetitive work associated with common customer questions and requests.

### References for Further Reading
- [Build a Wikipedia Factoid Bot](https://medium.com/@biosopher/wikipedia-factoid-bot-1-of-6-intro-and-configure-demo-code-884d6c2ac35e\#.zex5raoru) - a six part series taking you through building a factoid bot based on [Wikipedia](https://www.wikipedia.org/), which also shows an integration with the Watson Alchemy service.
- [Build a Chatbot That Cares](https://medium.com/ibm-watson-developer-cloud/build-a-chatbot-that-cares-part-1-d1c273e17a63\#.h9ahlfoh1) - nice series on building an IOT chatbot using the Coversation, Tone Analyzer, Speech-to-Text and Text-to-Speech services.
- [Build a Chatbot with Watson and Spoontacular](https://medium.com/ibm-watson-developer-cloud/how-to-build-a-recipe-slack-bot-using-watson-conversation-and-spoonacular-api-487eacaf01d4\#.xxt6vwknl) - another chatbot tutorial that builds a chatbot using Watson Conversation and the Spoontacular API.

---
# Cognitive Development Topics

## The Importance of Data
Data is the lifeblood of any cognitive solution.  You need to be aware of the 

### References for Further Reading
- [Data Considerations When Building a Cognitive Solution](https://kozhayasite.wordpress.com/2016/07/31/data-considerations-when-building-a-cognitive-solution/) - an overview of data considerations when working with Watson services.
- [Data Scientists and App Develpment](https://medium.com/cognitive-resonance/data-scientists-and-app-development-fde50ebb54de#.nz70d9ke0) - Anthony discusses the importance of data science in the building of cognitive applications, and he shares some ways to learn more about data science.

## DevOps with Cognitive on Bluemix
xxx

### References for Further Reading
- [Full Cycle Cognitive Development (4 part series)](https://dtoczala.wordpress.com/2017/02/02/full-cycle-cognitive-development-part-1-business-concepts/) - A series by D. Toczala on the concerns, tools, and strategies for doing Cognitive development, from ideation through build and maintenance.

## Testing Approaches and Methods
When looking at testing Cognitive systems, we run into issues that are new to software developers.  Cognitive systems are _trained_, and they may be non-deterministic.  So we have to apply some different principles and techniques when we test cognitive systems.

### References for Further Reading
- [Andrew Freed Blogs](https://developer.ibm.com/watson/blog/author/afreed/) - Andrew has done some thinking about cognitive testing, his blog posts will give you some insight into solid testing approaches.
- [Cognitive Quality Assurance \- An Introduction](https://brainsteam.co.uk/2016/03/29/cognitive-quality-assurance-an-introduction/) and [Cognitive Quality Assurance \- Performance Metrics](https://brainsteam.co.uk/2016/05/29/cognitive-quality-assurance-pt-2-performance-metrics/) - both authored by James Ravenscroft, with some good advice and introduction to the concepts of accuracy, precision, recall, and confusion matrices.

## Watson/Bluemix Security Concerns
There are some very real security implications that you will have to consider when developing applications and systems that use the IBM Cloud, and the Watson services hosted on that cloud.
- **Question:** How do Watson Developer Cloud services handle PII and PHI data?
  - **Answer:** PHI (Personal Health Information) data should NOT be handled by Watson Developer Cloud services. PII (Personally Identifiable Information), on the other hand may be okay to send to Watson Developer Cloud services. WDC services do not save any data if the user opts-out. If that is NOT sufficient, then the customer has the responsibility of any required de-identifying before sending the data to the Watson services. In certain emergency scenarios, deletion of PII data may be done by IBM team but this is handled on a case-by-case basis (contact Watson Security for any such needs).

### References for Further Reading
- **[WDC Security Overview](https://www.ibm.com/watson/assets/pdfs/Watson_Developer_Cloud_Security_Overview_October-2016.pdf)** - a PDF with a general overview of security topics when using Watson services (published October 2016)

---
# Common Tips and Tricks
This section will cover some of the common tips and tricks used by cognitive develpment professionals, and covers some of those things that are not addressed in the documentation.

- [Bluemix Tips and Tricks](docs/bluemix_tipstricks.md)



