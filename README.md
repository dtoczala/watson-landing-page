# Welcome to Watson
Cognitive computing can be complex, but we're here to help you make sense of it.  This is a technically focused set of pages that will allow you to explore the technology, see the latest best practices, and help you master cognitive application development.
# Contents
- **[Introduction](https://github.com/dtoczala/watson-landing-page#introduction---getting-started)**
- **[Watson Services and APIs](https://github.com/dtoczala/watson-landing-page#watson-services-and-apis)**
  - [Conversation](https://github.com/dtoczala/watson-landing-page#conversation)
  - [Discovery](https://github.com/dtoczala/watson-landing-page#discovery)
  - [Alchemy API](https://github.com/dtoczala/watson-landing-page#alchemy-api)
  - [Retrieve and Rank](https://github.com/dtoczala/watson-landing-page#retrieve-and-rank)
  - [Natural Language Understanding (NLU)](https://github.com/dtoczala/watson-landing-page#natural-language-understanding-nlu)
  - [Natural Language Classifier (NLC)](https://github.com/dtoczala/watson-landing-page#natural-language-classifier-nlc)
  - [Personality Insights](https://github.com/dtoczala/watson-landing-page#personality-insights)
  - [Speech to Text and Text to Speech (STT/TTS)](https://github.com/dtoczala/watson-landing-page#speech-to-text-and-text-to-speech-stttts)
  - [Tone Analyzer](https://github.com/dtoczala/watson-landing-page#tone-analyzer)
  - [Tradeoff Analytics](https://github.com/dtoczala/watson-landing-page#tradeoff-analytics)
  - [Visual Recognition](https://github.com/dtoczala/watson-landing-page#visual-recognition)
- **[Common Use Cases](https://github.com/dtoczala/watson-landing-page#common-use-cases)**
  - [Chatbots](https://github.com/dtoczala/watson-landing-page#chatbots)
  - [Customer Care](https://github.com/dtoczala/watson-landing-page#customer-care)
  - [Visual Inspection](https://github.com/dtoczala/watson-landing-page#visual-inspection)
- **[Cognitive Development Topics](https://github.com/dtoczala/watson-landing-page#cognitive-development-topics)**
  - [General Cognitive Development Information](https://github.com/dtoczala/watson-landing-page#general-cognitive-development-information)
  - [Cognitive Architectures](https://github.com/dtoczala/watson-landing-page#cognitive-architectures)
  - [The Importance of Data](https://github.com/dtoczala/watson-landing-page#the-importance-of-data)
  - [DevOps with Cognitive on Bluemix](https://github.com/dtoczala/watson-landing-page#devops-with-cognitive-on-bluemix)
  - [Testing Approaches and Methods](https://github.com/dtoczala/watson-landing-page#testing-approaches-and-methods)
  - [Watson/Bluemix Security Concerns](https://github.com/dtoczala/watson-landing-page/blob/master/README.md#watsonbluemix-security-concerns)
- **[Code Development Resources and GitHub Repositories](https://github.com/dtoczala/watson-landing-page/blob/master/README.md#code-development-resources-and-github-repositories)**
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
- [Watson Developer Handbook](https://ibm.ent.box.com/file/51752480029) - A PDF with links to important materials.
- [Building With Watson](https://www.ibm.com/watson/building-with-watson-webinar.html) - source for a series of technical webcasts on a variety of different Watson and cognitive computing topics.
- [IBM Watson - Where Do I Start?](https://joshicohen.wordpress.com/2016/11/08/ibm-watson-wdis/) - a quick blog post with links to good places to get started on your exploration of the Watson services and technology.

**Tools**
- [Bluemix Console Tool](http://myconsole.mybluemix.net/\#/dashboard) - Cool tool deployed on Bluemix that will show you all of your Bluemix services, spaces, applications, and organizations.

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

**Integration**
- [Example of Conversation and Discovery Integration](https://www.youtube.com/watch?v=SasXUqBE-38&feature=youtu.be) - This YouTube video shows an example of a Java application that integrates the Conversation and Discovery services. 

**Code**
- [Simple Conversation App](https://github.com/watson-developer-cloud/conversation-simple) - A simple sample Node.js app that uses conversation to power to car dashboard.

## Discovery
xxx

### References for Further Reading
None

**Integration**
- [Example of Conversation and Discovery Integration](https://www.youtube.com/watch?v=SasXUqBE-38&feature=youtu.be) - This YouTube video shows an example of a Java application that integrates the Conversation and Discovery services. 

## Alchemy API
The Alchemy API is being deprecated, and will not be available for the creation of new Alchemy instances on April 7, 2017.  Existing Alchemy API instances will remain functional until March 7, 2018.  Because of this, we strongly suggest starting new development with NLU or Discovery.  We will not be actively maintaining links to resources in this area.

Users who utilized Alchemy Language in the past are now encouraged to use the [Natural Language Understanding (NLU)](https://github.com/dtoczala/watson-landing-page#natural-language-understanding-nlu) service.

Users who utilized Alchemy Data News in the past are now encouraged to use the Watson [Discovery](https://github.com/dtoczala/watson-landing-page#discovery) service.

### References for Further Reading
- [How to Migrate from Alchemy Lanaguage to NLU](http://wdc-watson-master.stage1.mybluemix.net/doc/natural-language-understanding/migrating.html) - the official guide for migrating to the NLU service.
- [How to Migrate from Alchemy Data News to Discovery](https://www.ibm.com/watson/developercloud/doc/discovery/migrate-adn.html) - the official guide for migrating to the Watson Discovery service.

## Retrieve and Rank
The Retrieve and Rank service allows you to build a corpus of information, and then search that corpus to retrieve documents based on a trained ranker that evaluates the appropriateness of the document to the question being asked.

### References for Further Reading
- [R\&R Handbook](https://ibm.ent.box.com/file/53750516365) - A PDF with guidance, links to materials and code, and best practices for Retrieve and Rank.
- [Developing with Retrieve and Rank](https://medium.com/machine-learning-with-ibm-watson/developing-with-ibm-watson-retrieve-and-rank-part-1-solr-configuration-29c18e52966f\#.8hzg11tqp) - a three part series onhow to use Retrieve and Rank. [Part 1 covers SOLR configuration](https://medium.com/machine-learning-with-ibm-watson/developing-with-ibm-watson-retrieve-and-rank-part-1-solr-configuration-29c18e52966f\#.8hzg11tqp), [Part 2 covers training and configuration](https://medium.com/machine-learning-with-ibm-watson/developing-with-ibm-watson-retrieve-and-rank-part-2-training-and-evaluation-fda57efff5c8\#.h2wwsnail), and [Part 3 covers custom features](https://medium.com/machine-learning-with-ibm-watson/developing-with-ibm-watson-retrieve-and-rank-part-3-custom-features-826fe88a5c63\#.bc4h7k5oi).

## Natural Language Understanding (NLU)
xxx

### References for Further Reading
None

## Natural Language Classifier (NLC)
xxx

### References for Further Reading
- [NLC Handbook](https://ibm.ent.box.com/file/53025315153) - A PDF with guidance, links to materials and code, and best practices for Natural Language Classifier.

## Personality Insights
xxx

### References for Further Reading
- [Personality Insights Handbook](https://ibm.ent.box.com/file/51752480029) - A PDF with guidance, links to materials and code, and best practices for Personality Insights.
- [User Segmentation with Jungian Archetypes](https://ibm.ent.box.com/s/jtnlgbvszf9bn1pakn6fvsiwvas4x8fq) - a slide deck showing how use of Jungian archetypes can help in market segmentation, effectively segmenting users into categories to target communications based on user personality.
- [Leveraging PI to Predict Consumption Preferences](https://www.ibm.com/blogs/watson/2016/10/leveraging-personality-predict-consumption-preferences/) - a paper describing how Personality Insights can be used to help predict what people will choose to consume, based on their personality.

**Code**
- [Personality Insights with Twitter](https://github.com/watson-developer-cloud/personality-insights-twitter-python) - This sample shows how to get Twitter data using the Twitter REST API (via the python-twitter client library) and submit it to the Personality Insights Service.

## Speech to Text and Text to Speech (STT/TTS)
xxx

### References for Further Reading
- [IBM STT Model Hits New Milestone](https://www.ibm.com/blogs/watson/2017/03/reaching-new-records-in-speech-recognition/) - no technical information here, but an overview of how STT is done, and how IBM continues to improve it's speech recognition models.
- [Introducing Diarization](https://www.ibm.com/blogs/watson/2016/12/look-whos-talking-ibm-debuts-watson-speech-text-speaker-diarization-beta/) - announcement of the "diarization" capability in STT that allows you to differentiate between different speakers in an audio passage.

**Code**
- [Simple Node.js STT App](https://github.com/watson-developer-cloud/speech-to-text-nodejs) - A simple starter app in Node.js that utilizes the Speech to Text service.
- [Simple Python/WebSockets STT App](https://github.com/watson-developer-cloud/speech-to-text-websockets-python) - A simple starter app in Python, using WebSockets, that utilizes the Speech to Text service.

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

Often when doing analysis of pictures, it is useful to "tile" the image, and break it down into smaller chunks.  See the link to the [Visual Recognition Tile Localization](https://github.com/IBM-Bluemix/Visual-Recognition-Tile-Localization) tool, which is a KEY component for segmenting larger images into bite size pieces for Visual Recognition.

### References for Further Reading
- [Visual Recognition Command Line Interface](https://developer.ibm.com/dwblog/2017/command-line-tools-watson-visual-recognition/) - doing training and classification can be easier from the command line.
- [Sharpen Watson Visual Recognition Results](https://www.ibm.com/blogs/bluemix/2017/03/sharpen-watson-visual-recognition-results/) - Great blog by Andy Trice, his blog explains how to use "tile localization" to help your classifiers find details in images, and includes [the code for doing this](https://github.com/IBM-Bluemix/Visual-Recognition-Tile-Localization) on GitHub, which will run on Bluemix as-is.
- [Best Practice for Training Custom Classifiers](https://www.ibm.com/blogs/bluemix/2016/10/watson-visual-recognition-training-best-practices/) - article outlining some good approaches and best practices for custom classifiers.
- [Guidelines for Training Custom Classifiers](https://www.ibm.com/watson/developercloud/doc/visual-recognition/customizing.html) - some basic guidance on training custom classifiers from the online documentation.

**Code**
- [Visual Recgnition with ASP.NET](https://github.com/watson-developer-cloud/visual-recognition-aspnet) - Simple starter application in ASP.NET which uses the IBM Watson Visual Recognition service.
---
# Common Use Cases
This section will cover some of the basic patterns and cognitive use cases that are implemented using the Watson services.

## Chatbots

Chatbots are popular right now, and they can help serve a real purpose.  Many customers use them for customer care and customer support scenarios.  They have been integrated into a number of different communications channels, and they can often do the repetitive work associated with common customer questions and requests.

### References for Further Reading
- [Build a Wikipedia Factoid Bot](https://medium.com/@biosopher/wikipedia-factoid-bot-1-of-6-intro-and-configure-demo-code-884d6c2ac35e\#.zex5raoru) - a six part series taking you through building a factoid bot based on [Wikipedia](https://www.wikipedia.org/), which also shows an integration with the Watson Alchemy service.
- [Build a Chatbot That Cares](https://medium.com/ibm-watson-developer-cloud/build-a-chatbot-that-cares-part-1-d1c273e17a63\#.h9ahlfoh1) - nice series on building an IOT chatbot using the Coversation, Tone Analyzer, Speech-to-Text and Text-to-Speech services.
- [Build a Chatbot with Watson and Spoontacular](https://medium.com/ibm-watson-developer-cloud/how-to-build-a-recipe-slack-bot-using-watson-conversation-and-spoonacular-api-487eacaf01d4\#.xxt6vwknl) - another chatbot tutorial that builds a chatbot using Watson Conversation and the Spoontacular API.

## Customer Care

This is another popular use case, where a cognitive agent is used to handle common customer care problems and issues.  

### References for Further Reading

- [Customer Care Starter Kit](https://github.com/watson-developer-cloud/social-customer-care) - This application is a Starter Kit (SK) that is designed to get you up and running quickly with a common industry pattern, and to provide information and best practices around Watson services. This application was created to demonstrate how the Natural Language Classifier can be used to direct customer requests and queries to the appropriate agent or workflow. Additionally, Tone Analyzer, Alchemy Language, and Personality Insights demonstrate how to efficiently provide an agent with customer insights.  You will need to replace the Alchemy Language portions of this starter kit with NLU service calls - since Alchemy is being deprecated.

## Visual Inspection

This use case involves a visual inspection of still images using the Visual Recognition service and some other technologies.  Used to inspect, identify, and inform.

### References for Further Reading
- [Seafood Inspection (Dory)](https://devpost.com/software/dory) - a team created a seafood inspection app using Visual Recognition that will distinguish between different types of seafood.
- [Pokemon Go App](https://www.ibm.com/blogs/internet-of-things/pokemon-go-watson/) - Find Pokemon with the help of Watsons Visual Recognition services.

---
# Cognitive Development Topics

This is a colection of various popular topics within the realm of cognitive development.

## General Cognitive Development Information
Cognitive development in general is not always a well understood topic.  Software development teams are unfamiliar with the changes to typical concerns and iterations that a cognitive development project will have.  Teams often have incorrect expectations, and underestimate the importance of data, as well as the number of training iterations required to build a highly effective cognitive model.

### References and Further Reading
- [Building a Cognitive App in 70 days](https://developer.ibm.com/dwblog/2016/cognitive-solution-70-days-joe-kozhaya/) - An insider take on the critical factors involved in building a cognitive application (the [Watson Business Coach](https://www.ibm.com/cognitive/businesscoach/) ) in only 70 days.

## Cognitive Architectures
Cognitive architectures are not that different from the architectures for applications that you are familiar with.  They just use cognitive capabilities and components that may behave somewhat differently than a more "classical" software component.  You also need to take into account the need for _training_ in your maintenance of a cognitive solution, which adds a new wrinkle to how you architect a cognitive application.

### References for Further Reading
- [Common Cognitive Architectures](https://www.ibm.com/devops/method/content/architecture/cognitiveArchitecture) - taken from the IBM Cloud Garage Method, this set of architectures makes a good starting point for architects new to the building of cognitive solutions.

## The Importance of Data
Data is the lifeblood of any cognitive solution.  You need to be aware of [the common challenges that you will face](http://freedville.com/blog/2017/03/05/machine-learning-is-just-the-tip-of-the-iceberg-5-dangers-lurking-below-the-surface/) when working with the data that powers your cognitive solution.  The training processes used with cognitive systems is iterative, and the management of the data to do this training is an ongoing concern.  It's part of the common maintenance that is needed for a truly cognitive system.

### References for Further Reading
- [Why Does Machine Learning Require So Much Data](http://freedville.com/blog/2016/12/15/why-does-machine-learning-require-so-much-training-data/) - Great look at why you need so much data, and a veiled reference to [Malcoim Gladwell's 10000 hour rule](http://gladwell.com/outliers/the-10000-hour-rule/).
- [Data Considerations When Building a Cognitive Solution](https://kozhayasite.wordpress.com/2016/07/31/data-considerations-when-building-a-cognitive-solution/) - an overview of data considerations when working with Watson services.
- [Data Scientists and App Develpment](https://medium.com/cognitive-resonance/data-scientists-and-app-development-fde50ebb54de#.nz70d9ke0) - Anthony discusses the importance of data science in the building of cognitive applications, and he shares some ways to learn more about data science.

## DevOps with Cognitive on Bluemix
xxx

### References for Further Reading
- [Full Cycle Cognitive Development (4 part series)](https://dtoczala.wordpress.com/2017/02/02/full-cycle-cognitive-development-part-1-business-concepts/) - A series by D. Toczala on the concerns, tools, and strategies for doing Cognitive development, from ideation through build and maintenance.

## Testing Approaches and Methods
When looking at testing Cognitive systems, we run into issues that are new to software developers.  Cognitive systems are _trained_, and they may be non-deterministic.  So we have to apply some different principles and techniques when we test cognitive systems.

Andrew Freed has an excellent series of articles that cover the [testing pyramid](https://developer.ibm.com/watson/blog/2016/09/21/cognitive-system-testing-part-1-how-to-test-a-cognitive-system-and-why-its-so-important/), and discuss cognitive system concepts for [smoke testing](https://developer.ibm.com/watson/blog/2016/10/03/cognitive-system-testing-smoke-testing/), [accuracy testing](https://developer.ibm.com/watson/blog/2016/11/07/cognitive-system-testing-part-5-overall-system-accuracy-testing/), [ingestion](https://developer.ibm.com/watson/blog/2016/10/19/cognitive-system-testing-testing-at-the-beginning-with-ingestion-verification-test/) and [NLP](https://developer.ibm.com/watson/blog/2016/10/31/cognitive-system-testing-natural-language-processing-unit-testing/) testing, and finally [unit testing](https://developer.ibm.com/watson/blog/2016/11/21/cognitive-system-testing-so-i-dont-need-to-unit-test-my-cognitive-system/).  The series is a great overview of cognitive testing concepts.

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
# Code, Development Resources, and GitHub Repositories
This section has a list of great places where you can see working code, find development resources, or GitHub repositories with useful content.

- [Application Starter Kits (ASKs)](https://www.ibm.com/watson/developercloud/starter-kits.html) - great collection of common use cases, and code to go with them, which you can use and deploy on Bluemix to see how things work for yourself.
- [Watson Developer Cloud (GitHub)](https://github.com/watson-developer-cloud) - this GitHub repository has commonly used SDK's (software development kits) and code for some interesting demos.

---
# Common Tips and Tricks
This section will cover some of the common tips and tricks used by cognitive develpment professionals, and covers some of those things that are not addressed in the documentation.

- [Bluemix Tips and Tricks](docs/bluemix_tipstricks.md)



