# Welcome to Watson
Cognitive computing can be complex, but we're here to help you make sense of it.  This is a technically focused set of pages that will allow you to explore the technology, see the latest best practices, and help you master cognitive application development.
# Contents
- **[Introduction](https://github.com/dtoczala/watson-landing-page#introduction---getting-started)**
- **[Watson Services and APIs](https://github.com/dtoczala/watson-landing-page#watson-services-and-apis)**
  - [Watson Assistant](https://github.com/dtoczala/watson-landing-page#watson-assistant-formerly-conversation)
  - [Discovery](https://github.com/dtoczala/watson-landing-page#discovery)
  - [Alchemy API](https://github.com/dtoczala/watson-landing-page#alchemy-api)
  - [Natural Language Understanding (NLU)](https://github.com/dtoczala/watson-landing-page#natural-language-understanding-nlu)
  - [Natural Language Classifier (NLC)](https://github.com/dtoczala/watson-landing-page#natural-language-classifier-nlc)
  - [Personality Insights](https://github.com/dtoczala/watson-landing-page#personality-insights)
  - [OpenScale](https://github.com/dtoczala/watson-landing-page#openscale)
  - [Speech to Text and Text to Speech (STT/TTS)](https://github.com/dtoczala/watson-landing-page#speech-to-text-and-text-to-speech-stttts)
  - [Tone Analyzer](https://github.com/dtoczala/watson-landing-page#tone-analyzer)
  - [Tradeoff Analytics](https://github.com/dtoczala/watson-landing-page#tradeoff-analytics)
  - [Visual Recognition](https://github.com/dtoczala/watson-landing-page#visual-recognition)
  - [Watson Knowledge Studio](https://github.com/dtoczala/watson-landing-page/blob/master/README.md#watson-knowledge-studio-wks)
- **[Common Use Cases](https://github.com/dtoczala/watson-landing-page#common-use-cases)**
  - [Chatbots](https://github.com/dtoczala/watson-landing-page#chatbots)
  - [Customer Care](https://github.com/dtoczala/watson-landing-page#customer-care)
  - [Visual Inspection](https://github.com/dtoczala/watson-landing-page#visual-inspection)
- **[Watson Integrations](https://github.com/dtoczala/watson-landing-page#watson-integrations)**
  - [ServiceNow Integration](https://github.com/dtoczala/watson-landing-page#service-now-integration)
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
  - [Staying Aware of Watson and Cloud Best Practices](https://github.com/dtoczala/watson-landing-page/blob/master/README.md#staying-aware-of-watson-and-cloud-best-practices)

---
# Introduction - Getting Started

## The Watson Developer Cloud
The Watson Developer Cloud (WDC) is a collection of cogntive services hosted on the [IBM Bluemix](https://console.ng.bluemix.net/) platform.  They are available as cloud based services.  These services include:
- **[Watson Conversation service](https://console.ng.bluemix.net/catalog/services/conversation/)** - which is used to drive conversations with end users.  Some of the more common use cases include customer care scenarios and chatbots.  Also check out the various Application Starter Kits which uses Watson Conversation to build a chatbot.
- **[Watson Discovery Service](https://console.ng.bluemix.net/catalog/services/discovery/)** - which is used to answer "long tail" questions, catalog knowledge and information, and retrieve relevant documents.  

### References for Further Reading
- [Bluemix tutorial](https://console.ng.bluemix.net/docs/admin/adminpublic.html) - A simple getting started tutorial
- **[Watson Developer Tools](https://www.ibm.com/watson/developercloud/developer-tools.html)** - a nice landing page with links to Application Starter Kits (ASK's), SDKs, documentation, blogs and videos.
- [A Beginner's Guide to Artificial Intelligence, Machine Learning, and Cognitive Computing](https://www.ibm.com/developerworks/library/cc-beginner-guide-machine-learning-ai-cognitive/index.html) - nothing Watson specific here, just a high level review of the history of AI, and introduction to some of the basic concepts of AI.
- [Cloud Architecture Center](https://www.ibm.com/devops/method/category/architectures?cm_mc_uid=59482719098114889125842&cm_mc_sid_50200000=1488912584) - basic architecture concepts and patterns for Cloud and Cognitive development.
- [Watson Cognitive Developer Certification Study Guide](https://github.com/havasnewyork/IBM-Watson-Developer-Certification-Study-Guide) - a nice guide on GitHub with a nice background on core cognitive principles and concepts.
- [Watson Developer Blog](https://developer.ibm.com/watson/blog/) - don't be fooled by the title, most of the blog entries here are more along the lines of announcements of new capabilities available with Watson.  Some technical content here, but it's good to follow this to remain aware of the new things coming.
- [Watson Developer Handbook](https://ibm.box.com/s/nav52vt6q2xwib5zqwupwjf78mxtgems) - A PDF with links to important materials.
- [Building With Watson](https://www.ibm.com/watson/building-with-watson-webinar.html) - source for a series of technical webcasts on a variety of different Watson and cognitive computing topics.
- [IBM Watson - Where Do I Start?](https://joshicohen.wordpress.com/2016/11/08/ibm-watson-wdis/) - a quick blog post with links to good places to get started on your exploration of the Watson services and technology.
- [IBM Watson Developer Certification Study Guide](https://github.com/havasnewyork/IBM-Watson-Developer-Certification-Study-Guide) - parts of this are out of date, but the review of Cognitive Computing Fundamentals is pretty solid.

**Tools**
- [Bluemix Console Tool](http://myconsole.mybluemix.net/\#/dashboard) - Cool tool deployed on Bluemix that will show you all of your Bluemix services, spaces, applications, and organizations.

---
# Watson Services and APIs
The following section will focus on the various Watson services and API's, providing links to high quality technical content focused specifically on these services.

## Watson Assistant (formerly Conversation)
The Watson Assistant was formerly called Watson Conversation.  The name was changed in March 2018.

The Assistant service allows you to add a natural language interface to your application, to automate interactions with your end users. Common applications include virtual agents and chat bots that can integrate and communicate on any channel or device.  The [car dashboard chatbot](https://console.bluemix.net/developer/watson/starter-kits/watson-assistant-basic) on the [Application Starter Kits (ASKs) page](https://console.bluemix.net/developer/watson/starter-kits) is an excellent example of a chatbot application, with code and instructions on how to implement this on [IBM Cloud](https://console.ng.bluemix.net/).

The tooling used to "develop" the Assistant service consists of three parts.  The first part deals with user intents.  The purpose of intents is to map “what a user says” to “what a user means”. Because of the wide variety of utterances users say to mean the same intent, Watson Assistant leverages deep learning technology to extract intents from utterances. You, as the app developer, have complete control in defining what intents are relevant to your application. Once you’ve defined your list of intents, you need to teach Watson how to recognize these intents by providing it with sample utterances and how they map to these intents. Probably the most common question we get from developers is “how many sample utterances do I need to provide”. While the tool requires a minimum of five sample utterances, the general guideline is “the more the better”. We’ve typically seen good results with 20-30 sample utterances per intent. The key observation is to try and capture real end-user input utterances and then map those to the intents you’ve defined for your application.

The second part handles Entities.  Entities provide specific information that your bot can leverage to provide most relevant response. For example, if the user’s utterance is “I would like to book a flight to Paris”, then the intent is “book_flight” and the entity is “Paris”. You, as the app developer, define the entities that are relevant for your application by providing a list of entity names and for each entity, a list of values and for each value a corresponding list of synonyms.

Once intents and entities are defined in the Assistant service, it is the third part, called Dialog, that actually orchestrates the conversation based on extracted intents and entities, as well as context provided by the application. Context is an extremely important concept as it is the bridge that links the Assistant service to your bot (or application). Any information communicated back and forth between the Assistant service and the bot goes across through the context variables. Dialog consists of a number of user defined nodes where each node executes based on whether its condition is true. Think of each node as an “if” condition where the condition checked is based on a combination of intents, entities, and context variables (or any derived variables). If the condition is true, then the node executes; if not, the flow continues to the next node in the dialog. Please note that the order of the nodes is important as the flow executes top to bottom, left to right.

### References for Further Reading
- [Conversation with Alchemy Entity Extraction](https://kozhayasite.wordpress.com/2016/08/27/watson-conversation-with-alchemy-entity-extraction/) - great overview of Assistant concepts, and how to integrate with other Watson capabilities.  Complete with a GitHub repo with sample code.
- [Conversation Redbook](http://www.redbooks.ibm.com/Redbooks.nsf/RedbookAbstracts/sg248394.html) - A large document with some best practices and example use cases using Assistant.  Very big, lots of details.
- [The Socratic Method for Bot Writers](https://www.pullstring.com/blog/socratic-method) - great blog post on what to consider when planning and building a chatbot.  Planning and thought up front can have a huge impact on the value of your chatbot.
- [Watson Assistant Continuous Improvement Best Practices](https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?htmlfid=54022554USEN) - nice whitepaper that you can download which highlights some best practices to set up a continuopus improvement environment for a deployed application with Watson Assistant.  Not a lot on the DevOps pieces, but more focused on the "How do I test it? How do I improve it?" questions.

**Intents**
- [Defining Intents](https://www.ibm.com/watson/developercloud/doc/conversation/intents.html) - great starter page with video to help you in defining your intents.
- [Compund Questions](https://sodoherty.ai/2017/02/06/compound-questions/) - Nice article on a technique for detecting compound questions.
- [Watson in the White and Black Room](https://sodoherty.ai/2017/02/10/watson-in-the-black-and-white-room/) - Quick article on understanding Watson confidence scores.

**Entities**
- [Defining Entities](https://www.ibm.com/watson/developercloud/doc/conversation/entities.html) - great starter page with video to help you in defining your entities.
- [Improving Your Intents with Entities](https://sodoherty.ai/2017/01/16/improving-your-intents-with-entities/) - an exploration of how intents and entities work together.

**Dialog**
- [Building Dialogs](https://www.ibm.com/watson/developercloud/doc/conversation/dialog-build.html) - great starter page with video to help you in defining your entities.  It's a long page, but building a dialog can be a complex task.
- [SpEL Language Guide]() - Valid expressions in conditions are written in the Spring Expression (SpEL) language.  This is a reference guide for the SpEL language.
- [Recursive Questions with Conversations](https://ollycox.me/2016/10/21/recursive-questions-with-ibm-watson-conversations/) - a quick post showing how to disambiguate user utterances, without driving the end user crazy.
- [Pattern for Gathering Information with Conversation](https://ollycox.me/2016/11/18/pattern-for-gathering-information-in-ibm-watson-conversations/) - an example (with code) of gathering multiple pieces of information in a Conversation flow.
- [Gathering Information with Conversation](https://medium.com/@snrubnomis/gathering-information-with-ibm-watson-conversation-e23887ccbe3d) - a nice example using a pizza ordering use case that demonstrates using "frames" in Conversation to collect a series of inputs from a user.

**Integration**
- [8 steps for developing question answer solutions using Watson Conversation and Watson Discovery](https://developer.ibm.com/dwblog/2017/best-practices-developing-question-answer-solutions-watson-conversation-discovery/?social_post=1230338742&fst=Discover) - Excellent overview of how to develop an Expert Advisor or Q&A system using Watson Assistant and Watson Discovery.  Great real-world advice from two guys who have done this themselves.
- [Example of Conversation and Discovery Integration](https://www.youtube.com/watch?v=SasXUqBE-38&feature=youtu.be) - This YouTube video shows an example of a Java application that integrates the Assistant and Discovery services. 
- [Build a configurable, retail-ready chatbot](https://developer.ibm.com/code/journey/create-cognitive-retail-chatbot/) - this is a good example of integrating usage of [Conversation](https://github.com/dtoczala/watson-landing-page#watson-assistant-formerly-conversation) and [Discovery](https://github.com/dtoczala/watson-landing-page#discovery), along with some other things.  It includes code as well.
- [How to build an enhanced chatbot with Watson Conversation](https://developer.ibm.com/recipes/tutorials/how-to-build-an-enhanced-chatbot-with-watson-conversation/) - tutorial shows how to build a Watson chatbot that is integrated with Facebook Messenger.
- [Create a news chatbot to deliver content through Facebook Messenger](https://www.ibm.com/developerworks/library/cc-cognitive-chatbot-facebook/index.html) - this three part series goes over creating a chatbot application that integrates with Facebook and Slack.  The orchestration application is written in Java.
- [Learn how to export & import a Watson Assistant workspace](https://github.com/rodalton/export-import-wa-workspace) - great little guide done by [Ronan Dalton](https://github.com/rodalton) (with curl examples) of how to migrate your work via API calls from one Watson Assistant workspace to another.
- [Watson Conversation: How to Manage Workspaces](https://www.ibm.com/blogs/bluemix/2017/04/watson-conversation-manage-workspaces/) - great article and [code for a Watson Assistant workspace management tool](https://github.com/data-henrik/watson-conversation-tool.

**Code**
- [Watson Assistant API Reference](https://www.ibm.com/watson/developercloud/assistant/api/v1) - The API reference page.
- [Introducing Version Control in Watson Assistant](https://medium.com/ibm-watson/watson-assistant-versions-announcement-d60869b1f5f) - the announcement of the ability to create versions of your Watson Assistant skills, with a nice explanation of how it works. 
- [Simple Conversation App](https://github.com/watson-developer-cloud/conversation-simple) - A simple sample Node.js app that uses Watson Assistant to power to car dashboard.
- [10 Steps to Train a Chatbot and its Machine Learning Models to Maximize Performance](
https://developer.ibm.com/dwblog/2016/10-steps-train-chat-bot-chatbot-machine-learning/) - this outlines the methodology for training chatbots and the associated machine learning models to maximize performance. Although presented in the context of chatbots due to their high popularity, the methodology applies to all cognitive solutions, not just chatbots.
- [Sample Conversation Applications](https://www.ibm.com/watson/developercloud/doc/conversation/sample-applications.html) - sample applications with code in GitHub, showing simple Conversation applications, as well as some simple applications with other services integrated. 
- [Chatbot with Conversation, NLU and Weather](https://developer.ibm.com/dwblog/2017/chatbot-watson-conversation-natural-language-understanding-nlu/) - developerWorks article that walks you through setting up and cloning a project that will build a chatbot that uses Assistant, NLU and Weather.  Good example and you can poke through the code.
- [Building Cognitive Applications with IBM Watson Services: Volume 2](http://www.redbooks.ibm.com/redpieces/pdfs/sg248394.pdf) - this is an IBM Redbook that shows some different use cases with the Assistant service.  It's long, at 248 pages, but has good detailed examples of different use cases.

**Logs**
- [Improve Your Chatbot using Watson Assistant Chat Logs](https://chatbotslife.com/improve-your-chatbot-using-watson-conversation-chat-logs-54a36b671261) - nice article showing you how to use the Assistant chat logs to provide feedback on chatbot performance and operations, and use that information to improve your chatbot.
- [I love Pandas!](https://sodoherty.ai/2017/04/19/i-love-pandas/#comment-765) - quick but informative blog post on how to use the Python pandas library to analyze your Assistant logs.

## Discovery
The Watson Discovery service helps you gather insights from large amounts of data, similar to the Retrieve and Rank service.  Discovery lets you upload your own enterprise data and then use its enrichment capabilities to understand the data and gather insights.  You can use Discovery in various use cases such as capturing insights from data as well as question/answer use cases where the corpus consists of a large number of documents and the objective is to find the most relevant answers to a query.

Another interesting feature of Discovery is that it comes preinstalled with a Watson News data set.  This is a public data set of the news, with approximately 300,000 articles and blogs daily, that is pre-enriched with cognitive insights. This results in a data set of primarily English language news sources that is updated continuously. You can use the Discovery News capability to query this data set for insights that you can integrate directly into your application.

### References for Further Reading
- [Discovery API Reference](https://www.ibm.com/watson/developercloud/discovery/api/v1/) - The API reference page.
- [Explore the news and gather insights using Watson Discovery](https://www.ibm.com/developerworks/library/cc-watson-discovery-service-bluemix-explore/) - Nice tutorial on how to use the news reading and curation capabilities in the Discover services, and how to use some of the basic functionality to get insights into what the news is.
- [The IBM Advantage for Cognitive Discovery Cloud Architecture](https://www.ibm.com/cloud/garage/files/IBM-Advantage-Paper-for-Cognitive-Discovery.pdf) - hesitated to add this because it is a LITTLE bit of a "rah-rah" sales pitch.  However, it does a nice job of explaining the Discovery service, shares some reference architectures, and talks about the importance of good data and data handling.

**Code**
- [Sample UI and code pattern for Discovery with Node,js](https://developer.ibm.com/code/patterns/create-an-app-to-perform-intelligent-searches-on-data/) - the demo video is 15 minutes long, and you can just go and grab the code out of GitHub.  Nice way to get yourself kickstarted with using Discovery with Node,js.

**Integration**
- [8 steps for developing question answer solutions using Watson Conversation and Watson Discovery](https://developer.ibm.com/dwblog/2017/best-practices-developing-question-answer-solutions-watson-conversation-discovery/?social_post=1230338742&fst=Discover) - Excellent overview of how to develop an Expert Advisor or Q&A system using Watson Assistant and Watson Discovery.  Great real-world advice from two guys who have done this themselves.
- [Example of Conversation and Discovery Integration](https://www.youtube.com/watch?v=SasXUqBE-38&feature=youtu.be) - This YouTube video shows an example of a Java application that integrates the Assistant and Discovery services.
- [Build a configurable, retail-ready chatbot](https://developer.ibm.com/code/journey/create-cognitive-retail-chatbot/) - this is a good example of integrating usage of [Assistant](https://github.com/dtoczala/watson-landing-page#watson-assistant-formerly-conversation) and [Discovery](https://github.com/dtoczala/watson-landing-page#discovery), along with some other things.  It includes code as well.

## Alchemy API
The Alchemy API is being deprecated, and will not be available for the creation of new Alchemy instances on April 7, 2017.  Existing Alchemy API instances will remain functional until March 7, 2018.  Because of this, we strongly suggest starting new development with NLU or Discovery.  We will not be actively maintaining links to resources in this area.

Users who utilized Alchemy Language in the past are now encouraged to use the [Natural Language Understanding (NLU)](https://github.com/dtoczala/watson-landing-page#natural-language-understanding-nlu) service.

Users who utilized Alchemy Data News in the past are now encouraged to use the Watson [Discovery](https://github.com/dtoczala/watson-landing-page#discovery) service.

### References for Further Reading
- [Top 3 reasons to move from AlchemyLanguage to Watson Natural Language Understanding](https://www.ibm.com/blogs/watson/2017/05/top-3-reasons-move-alchemylanguage-watson-natural-language-understanding) - Not technical, but does highlight three good reasons to migrate from Alchemy to [NLU](https://github.com/dtoczala/watson-landing-page#natural-language-understanding-nlu) sooner rather than later.
- [How to Migrate from Alchemy Lanaguage to NLU](https://www.ibm.com/watson/developercloud/doc/natural-language-understanding/migrating.html) - the official guide for migrating to the NLU service.
- [How to Migrate from Alchemy Data News to Discovery](https://www.ibm.com/watson/developercloud/doc/discovery/migrate-adn.html) - the official guide for migrating to the Watson Discovery service.
- [Alchemy API Migration - Tips and Tricks](docs/Alchemy_migrate.md) - answers to some of the more common questions that are not addressed in the documentation.

## Natural Language Understanding (NLU)
The NLU service allows you to analyze text to extract meta-data from supplied content such as concepts, entities, keywords, categories, sentiment, emotion, relations, and semantic roles.  It also has the capability to be used in conjunction with custom annotation models developed using Watson Knowledge Studio, enabling you to identify industry/domain specific entities and relations in unstructured text.

It has replaced most of the functionality that was exposed in the [Alchemy Language](https://github.com/dtoczala/watson-landing-page#alchemy-api) service.  Users who utilized Alchemy Language in the past are now encouraged to use the NLU service.

### References for Further Reading
- [NLU API Reference](https://www.ibm.com/watson/developercloud/natural-language-understanding/api/v1/) - The API reference page.
- [NLU Redbook](http://www.redbooks.ibm.com/Redbooks.nsf/RedbookAbstracts/sg248398.html?Open) - A large document with some best practices and an example use case using NLU.  Very big, lots of details.
- [NLU Categories Hierarchy](https://console.bluemix.net/docs/services/natural-language-understanding/categories.html#categories-hierarchy) - from the online docs, a list of the categories hierarchy returned by NLU.  See if this breakdown will work for your use case.

**Code**
- [Chatbot with Conversation, NLU and Weather](https://developer.ibm.com/dwblog/2017/chatbot-watson-conversation-natural-language-understanding-nlu/) - developerWorks article that walks you through setting up and cloning a project that will build a chatbot that uses Assistant, NLU and Weather.  Good example and you can poke through the code.

## Natural Language Classifier (NLC)
The Natural Language Classifier service applies cognitive computing techniques to return the best matching classes for a sentence or phrase. For example, you submit a question and the service returns keys to the best matching intents. You create a classifier instance by providing a set of utterances and a corresponding set of correct intents for each training question. After training, the new classifier can accept new questions or phrases and return the top matches with a probability score for each match.

### References for Further Reading
- [NLC API Reference](https://www.ibm.com/watson/developercloud/natural-language-classifier/api/v1/) - The API reference page.
- [NLC Best Practices](https://www.ibm.com/watson/assets-watson/pdf/Watson-NLC-Links-Best-Practices-Design-Patterns.pdf) - a quick slide deck reviewing some best practices and design patterns for NLC.
- [NLC Handbook](https://ibm.box.com/s/rdlog2sue79178816s0rabkbi7ifu5vg) - A PDF with guidance, links to materials and code, and best practices for Natural Language Classifier.
- [NLC Redbook](http://www.redbooks.ibm.com/Redbooks.nsf/RedbookAbstracts/sg248391.html) - A large document with some best practices and some example use cases using NLC.  Very big, lots of details.
- [Create and train a classifier for Watson’s Natural Language Classifier Service](https://developer.ibm.com/videos/create-and-train-a-classifier-for-watsons-natural-language-classifier-service/) - great video by Ronan Dalton that shows how to create a custom classifier using NLC.

## Personality Insights
Personality Insights derives insights from written and social media data to identify psychological traits which can influence personal decisions, intent and behavioral traits; all of which can be utilized to improve customer interactions, customer engagement, and customer satisfaction.

### References for Further Reading
- [Personality Insights API Reference](https://www.ibm.com/watson/developercloud/personality-insights/api/v3/) - The API reference page.
- [Personality Insights Handbook](https://ibm.box.com/s/nav52vt6q2xwib5zqwupwjf78mxtgems) - A PDF with guidance, links to materials and code, and best practices for Personality Insights.
- [User Segmentation with Jungian Archetypes](https://ibm.ent.box.com/s/jtnlgbvszf9bn1pakn6fvsiwvas4x8fq) - a slide deck showing how use of Jungian archetypes can help in market segmentation, effectively segmenting users into categories to target communications based on user personality.
- [Leveraging PI to Predict Consumption Preferences](https://www.ibm.com/blogs/watson/2016/10/leveraging-personality-predict-consumption-preferences/) - a paper describing how Personality Insights can be used to help predict what people will choose to consume, based on their personality.
- [25 Tweets to Know You: A New Model to Predict Personality with Social Media](https://arxiv.org/abs/1704.05513) - a paper describing the science behind the Personality Insights service.

**Code**
- [Personality Insights with Twitter](https://github.com/watson-developer-cloud/personality-insights-twitter-python) - This sample shows how to get Twitter data using the Twitter REST API (via the python-twitter client library) and submit it to the Personality Insights Service.
- [Your Celebrity Match](https://github.com/watson-developer-cloud/your-celebrity-match) - a sample application that does an analysis of your Twitter traffic, and matches you to a variety of celebrities, based on personality, needs and values.

## OpenScale
Watson OpenScale allows enterprises to automate and operationalize the AI lifecycle in business applications.  It will help ensure that AI models are free from bias, can be easily explained and understood by business users, and are auditable in business transactions. I OpenScale supports AI models built and run in Watson Studio.  Examples are Watson Machine Learning, Azure ML, Amazon SageMaker, and others.  

### References for Further Reading
- [Getting Started with OpenScale](https://test.cloud.ibm.com/docs/services/ai-openscale?topic=ai-openscale-gettingstarted#gettingstarted) - The getting started guide.  I STRONGLY recommend going through this, since OpenScale can be a bit tough to wrap your head around at first.
- [Watson OpenScale API](https://cloud.ibm.com/apidocs/ai-openscale) - The API reference page.

## Speech to Text and Text to Speech (STT/TTS)
Speech to Text (STT) and Text to Speech (TTS) are well understood capabilities, so no use in going into a boring explanation.  These are often coupled with [Natural Language Understanding (NLU)](https://github.com/dtoczala/watson-landing-page/blob/master/README.md#natural-language-understanding-nlu) or [Assistant](https://github.com/dtoczala/watson-landing-page#watson-assistant-formerly-conversation), to help form compelling cognitive applications.

Often latency can be an issue with STT, and is is HIGHLY recommended that you you use Web Sockets for your data transfer when using STT.  It greatly reduces the latency (as compared to http).

### References for Further Reading
- [Speech to Text (STT) API Reference](https://www.ibm.com/watson/developercloud/speech-to-text/api/v1/) - The API reference page.
- [Text to Speech (TTS) API Reference](https://www.ibm.com/watson/developercloud/text-to-speech/api/v1/) - The API reference page.
- [TTS/STT Redbook](http://www.redbooks.ibm.com/Redbooks.nsf/RedbookAbstracts/sg248388.html) - A large document with some best practices and an example use case using NLU.  Very big, lots of details.
- [IBM STT Model Hits New Milestone](https://www.ibm.com/blogs/watson/2017/03/reaching-new-records-in-speech-recognition/) - no technical information here, but an overview of how STT is done, and how IBM continues to improve it's speech recognition models.
- [Introducing Diarization](https://www.ibm.com/blogs/watson/2016/12/look-whos-talking-ibm-debuts-watson-speech-text-speaker-diarization-beta/) - announcement of the "diarization" capability in STT that allows you to differentiate between different speakers in an audio passage.
- [Watson Text to Speech Transformation Play](https://www.youtube.com/watch?v=scwVNHgRrOU&feature=youtu.be) - a video (showing code) which shows examples of modifications of speaker, tone, pitch, voice, and emotion, in Watson text-to-speech.
- [Experimental: IBM's Voice Agent with Watson and Twillio](https://developer.ibm.com/recipes/tutorials/ibms-voice-agent-with-watson-and-twilio/) - video shows the new IBM Voice Agent (which uses Assistant, Speech-to-Text and Text-to-Speech) integrated with Twillio, to create a talking chatbot.

**Code**
- [Simple Node.js STT App](https://github.com/watson-developer-cloud/speech-to-text-nodejs) - A simple starter app in Node.js that utilizes the Speech to Text service.
- [Simple Python/WebSockets STT App](https://github.com/watson-developer-cloud/speech-to-text-websockets-python) - A simple starter app in Python, using WebSockets, that utilizes the Speech to Text service.

## Tone Analyzer
Tone Analyzer leverages cognitive linguistic analysis to identify a variety of tones at both the sentence and document level. This insight can then used to refine and improve communications. It detects two types of tones, emotion (anger, fear, joy and sadness), and language styles (analytical, confident and tentative) from text.

### References for Further Reading
- [Tone Analyzer API Reference](https://www.ibm.com/watson/developercloud/tone-analyzer/api/v3/) - The API reference page.
- [Service Changes to Tone Analyzer]() - current as of Spetemebr 2017, this announces the elimination of social tones (openness, conscientiousness, extroversion, agreeableness, and emotional range) which were not used, the combination of the anger and disgust tones (which caused some confusion), and the return of only high scoring tone data.

## Tradeoff Analytics
This service has been deprecated.  

### References for Further Reading
None

## Visual Recognition
The Visual Recognition API is used for vision services.

Often when doing analysis of pictures, it is useful to "tile" the image, and break it down into smaller chunks.  See the link to the [Visual Recognition Tile Localization](https://github.com/IBM-Bluemix/Visual-Recognition-Tile-Localization) tool, which is a KEY component for segmenting larger images into bite size pieces for Visual Recognition.

### References for Further Reading
- [Visual Recognition API Reference](https://www.ibm.com/watson/developercloud/visual-recognition/api/v3/) - The API reference page.
- [Visual Recognition Command Line Interface](https://developer.ibm.com/dwblog/2017/command-line-tools-watson-visual-recognition/) - doing training and classification can be easier from the command line.
- [Sharpen Watson Visual Recognition Results](https://www.ibm.com/blogs/bluemix/2017/03/sharpen-watson-visual-recognition-results/) - Great blog by Andy Trice, his blog explains how to use "tile localization" to help your classifiers find details in images, and includes [the code for doing this](https://github.com/IBM-Bluemix/Visual-Recognition-Tile-Localization) on GitHub, which will run on Bluemix as-is.
- [Best Practice for Training Custom Classifiers](https://www.ibm.com/blogs/bluemix/2016/10/watson-visual-recognition-training-best-practices/) - article outlining some good approaches and best practices for custom classifiers.
- [Guidelines for Training Custom Classifiers](https://www.ibm.com/watson/developercloud/doc/visual-recognition/customizing.html) - some basic guidance on training custom classifiers from the online documentation.
- [Visual Recognition Redbook](http://www.redbooks.ibm.com/Redbooks.nsf/RedbookAbstracts/sg248393.html) - A large document with some best practices and some example use cases using Visual Recognition.  Very big, lots of details.
- [Chihuahua or Muffin Revisited](https://sodoherty.ai/2017/09/28/chihuahua-or-muffin-revisited/) - funny demo that trains a visual classifier to detect dogs or food.

**Code**
- [Visual Recgnition with ASP.NET](https://github.com/watson-developer-cloud/visual-recognition-aspnet) - Simple starter application in ASP.NET which uses the IBM Watson Visual Recognition service.

## Watson Knowledge Studio (WKS)
The Watson Knowledge Studio is used to teach Watson the language of your domain, creating custom models that identify entities and relationships unique to your industry, in unstructured text. You are able to build your models in a collaborative environment designed for both developers and domain experts, without needing to write code. Use the resulting models in [Watson Discovery](https://github.com/dtoczala/watson-landing-page#discovery), [Natural Language Understanding (NLU)](https://github.com/dtoczala/watson-landing-page#natural-language-understanding-nlu), and Watson Explorer.

### References for Further Reading
- [Accelerate Watson model development with a rule-based approach](https://developer.ibm.com/tv/accelerate-watson-model-development-rule-based-approach/) - video showing that sometimes machine learning can be complimented by the use of rules in more deterministic patterns found in the content.  This webinar demonstrates this new feature in WKS to define such patterns in such a way that you do not have to be a programmer of regular expressions to define rules and apply them to annotate content with the resulting model.

---
# Common Use Cases
This section will cover some of the basic patterns and cognitive use cases that are implemented using the Watson services.  Ryan Anderson has a blog post on [common design patterns and use cases for cognitive development](https://www.linkedin.com/pulse/cognitive-bucket-list-leveraging-design-patterns-value-ryan-anderson) which I suggest you take 5 minutes to read.

## Chatbots

Chatbots are popular right now, and they can help serve a real purpose.  Many customers use them for customer care and customer support scenarios.  They have been integrated into a number of different communications channels, and they can often do the repetitive work associated with common customer questions and requests.

### References for Further Reading
- [Short-tail, Long-tail, and Human-tail Chatbots](http://fredrikstenbeck.com/short-tail-long-tail-and-human-tail-chatbot/) - I don't agree with EVERYTHING this guy says, but he lays out a nice, quick explanation of the various depths/degrees that chatbots get to.  A good way to explain the difference between short-tail and long-tail questions.
- [Build a Wikipedia Factoid Bot](https://medium.com/@biosopher/wikipedia-factoid-bot-1-of-6-intro-and-configure-demo-code-884d6c2ac35e\#.zex5raoru) - a six part series taking you through building a factoid bot based on [Wikipedia](https://www.wikipedia.org/), which also shows an integration with the Watson Alchemy service.
- [Build an IT Support Chatbot with Watson Assistant](https://www.ibm.com/cloud/garage/tutorials/watson_conversation_support) - great tutorial and guide for building your first chatbot.
- [Build a Chatbot That Cares](https://medium.com/ibm-watson-developer-cloud/build-a-chatbot-that-cares-part-1-d1c273e17a63\#.h9ahlfoh1) - nice series on building an IOT chatbot using the Coversation, Tone Analyzer, Speech-to-Text and Text-to-Speech services.
- [Build a Chatbot with Watson and Spoontacular](https://medium.com/ibm-watson-developer-cloud/how-to-build-a-recipe-slack-bot-using-watson-conversation-and-spoonacular-api-487eacaf01d4\#.xxt6vwknl) - another chatbot tutorial that builds a chatbot using Watson Assistant and the Spoontacular API.
- [Chatbot with Conversation, NLU and Weather](https://developer.ibm.com/dwblog/2017/chatbot-watson-conversation-natural-language-understanding-nlu/) - developerWors article that walks you through setting up and cloning a project that will build a chatbot that uses Assistant, NLU and Weather.  Good example and you can poke through the code.
- [10 Steps to Train a Chatbot and its Machine Learning Models to Maximize Performance](
https://developer.ibm.com/dwblog/2016/10-steps-train-chat-bot-chatbot-machine-learning/) - this outlines the methodology for training chatbots and the associated machine learning models to maximize performance. Although presented in the context of chatbots due to their high popularity, the methodology applies to all cognitive solutions, not just chatbots.

## Customer Care

This is another popular use case, where a cognitive agent is used to handle common customer care problems and issues.  

### References for Further Reading

- [Customer Care Starter Kit](https://github.com/watson-developer-cloud/social-customer-care) - This application is a Starter Kit (SK) that is designed to get you up and running quickly with a common industry pattern, and to provide information and best practices around Watson services. This application was created to demonstrate how the Natural Language Classifier can be used to direct customer requests and queries to the appropriate agent or workflow. Additionally, Tone Analyzer, Alchemy Language, and Personality Insights demonstrate how to efficiently provide an agent with customer insights.  You will need to replace the Alchemy Language portions of this starter kit with NLU service calls - since Alchemy is being deprecated.
- [Knowledge Base Search](https://www.ibm.com/watson/developercloud/starter-kits.html#knowledge-base-search) - this is an improved knowledge base search based on annotated content in a corpus.  Uses the Watson Discovery service.
- [8 steps for developing question answer solutions using Watson Conversation and Watson Discovery](https://developer.ibm.com/dwblog/2017/best-practices-developing-question-answer-solutions-watson-conversation-discovery/?social_post=1230338742&fst=Discover) - Excellent overview of how to develop an Expert Advisor or Q&A system using Watson Assistant and Watson Discovery.  Great real-world advice from two guys who have done this themselves.
- [Call Analytics Integrated Application](https://github.com/rodalton/call-analytics) - an EXCELLENT piece of code done by [Ronan Dalton](https://github.com/rodalton) that uses a Java application in combination with various Watson services, Cloud Object Storage (COS), and DB2 on Cloud.  Does analytics of call center recordings using the cognitive capabilities of Watson.

## Visual Inspection

This use case involves a visual inspection of still images using the Visual Recognition service and some other technologies.  Used to inspect, identify, and inform.

### References for Further Reading
- [Seafood Inspection (Dory)](https://devpost.com/software/dory) - a team created a seafood inspection app using Visual Recognition that will distinguish between different types of seafood.
- [Pokemon Go App](https://www.ibm.com/blogs/internet-of-things/pokemon-go-watson/) - Find Pokemon with the help of Watsons Visual Recognition services.

---
# Watson Integrations

This is a colection of various popular topics around the idea of Watson integrations.  This is NOT an exhaustive list of potential integrations, or business partner integrations.  It is a list of integrations that we have used, and some tips and ionsights on how to use them.

## Service Now Integration

ServiceNow is a CRM solution that is widely used by many SaaS providers.  There is a pre-built integration between ServiceNow and Watson Assistant - which allows you to easily incorporate Watson conversational capabilities into a ServiceNow implementation.

### References and Further Reading

- [Deploy a Virtual Agent with IBM Watson's Assistant (Conversation) Service](https://community.servicenow.com/community?id=community_blog&sys_id=2e7ca2e1dbd0dbc01dcaf3231f96192b) - article in the ServiceNow community detailing how to obtain a Virtual Agent prebuilt for self service incident deflection, and easily extensible to additional use cases both within and outside ITSM.  Definitely worth a look.

---
# Cognitive Development Topics

This is a colection of various popular topics within the realm of cognitive development.

## General Cognitive Development Information
Cognitive development in general is not always a well understood topic.  Software development teams are unfamiliar with the changes to typical concerns and iterations that a cognitive development project will have.  Teams often have incorrect expectations, and underestimate the importance of data, as well as the number of training iterations required to build a highly effective cognitive model.

### References and Further Reading
- [Building a Cognitive App in 70 days](https://developer.ibm.com/dwblog/2016/cognitive-solution-70-days-joe-kozhaya/) - An insider take on the critical factors involved in building a cognitive application (the [Watson Business Coach](https://www.ibm.com/cognitive/businesscoach/) ) in only 70 days.
- [IBM Certified Application Developer - Watson V3](https://www.ibm.com/certify/cert?id=60000101) - get your Watson certification badge.

## Cognitive Architectures
Cognitive architectures are not that different from the architectures for applications that you are familiar with.  They just use cognitive capabilities and components that may behave somewhat differently than a more "classical" software component.  You also need to take into account the need for _training_ in your maintenance of a cognitive solution, which adds a new wrinkle to how you architect a cognitive application.

### References for Further Reading
- [Common Cognitive Architectures](https://www.ibm.com/devops/method/content/architecture/cognitiveArchitecture) - taken from the IBM Cloud Garage Method, this set of architectures makes a good starting point for architects new to the building of cognitive solutions.

## The Importance of Data
Data is the lifeblood of any cognitive solution.  You need to be aware of [the common challenges that you will face](http://freedville.com/blog/2017/03/05/machine-learning-is-just-the-tip-of-the-iceberg-5-dangers-lurking-below-the-surface/) when working with the data that powers your cognitive solution.  The training processes used with cognitive systems is iterative, and the management of the data to do this training is an ongoing concern.  It's part of the common maintenance that is needed for a truly cognitive system.

### The IBM Watson Studio
IBM has an environment that will help you with the intersection of data science and machine learning, it's called the [IBM Watson Studio](https://datascience.ibm.com/).  This has a variety of resources and tools to help with your data science projects, and allow you to "unlock" the value hidden in your data.  Below are some interesting links to help you begin using the resources associated with [Watson Studio](https://datascience.ibm.com/).

- [Watson Studio and Watson Knowledge Catalog Documentation](https://datascience.ibm.com/docs/content/getting-started/welcome-main.html) - an ordered set of links to materials to help you get started with Watson Studio.
- [Watson Machine Learning within the Data Science Experience](https://developer.ibm.com/dwblog/2017/watson-machine-learning-within-ibm-data-science-experience/#main) - a blog post which walks you through setting up a machine learning model for a predictive retail use case.  Walks you through the entire process.  Some of this is out of date, it mentions the Data Science Experience (DSX), which was the predecessor of Watson Studio.
- [Data Science Experience Community](https://apsportal.ibm.com/community?context=analytics) - a good place to grab tutorials, data sets (yes - real data sets), articles, and notebooks.  Nice place to grab things to get you started.

### Data Science, Design and User Experience
Data science manages to surface data and information from large data sets, to help us understand better.  Design and user experience design help bring this data, and it's insights, to life for your end user.  Any powerful application that delights it's end users will have both a strong user experience, and a strong data science component.  Here is some suggested reading on the intersection of design and data.

- [How Designers can use Data to create amazing work](http://blog.invisionapp.com/how-designers-can-use-data/) - Roger Huang of Springboard talks about 5 basic goals in this area, and provides some key resources and tips for the day-to-day application of these concepts.
- [Experience Design in the Machine Learning Era](https://medium.com/@girardin/experience-design-in-the-machine-learning-era-e16c87f4f2e2) - A long but very good post by Fabien Girardin of BBVA, on the importance of design and data for the success of a any cognitive application.  Thought provoking content.
- [How Data and Design Can Work Together](http://www.hugeinc.com/ideas/perspective/how-data-and-design-can-work-together) - Heiko Waechter brings some some quick points that you need to consider when working in the intersection of data and design.
- [5 Steps to Thinking Like a Designer in Machine Learning](http://machinelearningmastery.com/5-steps-to-thinking-like-a-designer-in-machine-learning/) - Kevin Dallas brings up 5 basic points that need to be considered when doing data science, and makes the argument that good data scientists need to be good designers.
- [Machine Learning and UX](https://medium.com/designer-hangout/machine-learning-and-ux-c28725b5f3) - Byron Houwens discusses great design for machine learning, and highlights the point that there is not a lot of information about the intersection of machine learning and design out there right now.  It's a field full of opportunity.

### References for Further Reading
- [Why Does Machine Learning Require So Much Data](http://freedville.com/blog/2016/12/15/why-does-machine-learning-require-so-much-training-data/) - Great look at why you need so much data, and a veiled reference to [Malcoim Gladwell's 10000 hour rule](http://gladwell.com/outliers/the-10000-hour-rule/).
- [Data Considerations When Building a Cognitive Solution](https://kozhayasite.wordpress.com/2016/07/31/data-considerations-when-building-a-cognitive-solution/) - an overview of data considerations when working with Watson services.
- [Extract insights from social media posts with Watson and Spark in Data Science Experience](https://www.ibm.com/developerworks/library/cc-cognitive-watson-extract-insights-spark-dsx/index.html) - this tutorial brings together several tools and services to address realistic business problems, that of brand analytics, user segmentation and personalized messaging. It illustrates how to run a Python notebook in Data Science Experience to analyze social media data leveraging Watson services (NLU and PI) for enriching the unstructured content.
- [Data Scientists and App Develpment](https://medium.com/cognitive-resonance/data-scientists-and-app-development-fde50ebb54de#.nz70d9ke0) - Anthony discusses the importance of data science in the building of cognitive applications, and he shares some ways to learn more about data science.
- [Invisible Design - AirBnb](http://airbnb.design/invisible-design/) - Amber Cartwright of AirBnB writes about how you need to truly understand a product and the technology behind it, to be able to design effectively.
- [The 50 Best Free Datasets for Machine Learning](https://gengo.ai/articles/the-50-best-free-datasets-for-machine-learning/) - 50 solid free datasets for machine learning models.  Nice collection of resources here.


## DevOps with Cognitive on Bluemix
The topic of DevOps when working in Bluemix is deserving of it's own "landing page".  The open cloud platform and the ability to apply the [Continuous Delivery](https://console.ng.bluemix.net/devops/getting-started) service, along with it's support for toolchains, means that you have a lot of options when configuring your Bluemix environment to promote best practices and DevOps principles.

### References for Further Reading
- [Setting up your Bluemix environment](https://console.ng.bluemix.net/docs/admin/patterns.html#patterns) - Not a lot of guidance here, but this documentation page on Bluemix has a lot of the basic information that you will need to understand when setting up a DevOps supported development environment for your cloud and cognitive development.
- [Full Cycle Cognitive Development (4 part series)](https://dtoczala.wordpress.com/2017/02/02/full-cycle-cognitive-development-part-1-business-concepts/) - A series by D. Toczala on the concerns, tools, and strategies for doing Cognitive development, from ideation through build and maintenance.

## Testing Approaches and Methods
When looking at testing Cognitive systems, we run into issues that are new to software developers.  Cognitive systems are _trained_, and they may be non-deterministic.  So we have to apply some different principles and techniques when we test cognitive systems.

Andrew Freed has an excellent series of articles that cover the [testing pyramid](https://developer.ibm.com/watson/blog/2016/09/21/cognitive-system-testing-part-1-how-to-test-a-cognitive-system-and-why-its-so-important/), and discuss cognitive system concepts for [smoke testing](https://developer.ibm.com/watson/blog/2016/10/03/cognitive-system-testing-smoke-testing/), [accuracy testing](https://developer.ibm.com/watson/blog/2016/11/07/cognitive-system-testing-part-5-overall-system-accuracy-testing/), [ingestion](https://developer.ibm.com/watson/blog/2016/10/19/cognitive-system-testing-testing-at-the-beginning-with-ingestion-verification-test/) and [NLP](https://developer.ibm.com/watson/blog/2016/10/31/cognitive-system-testing-natural-language-processing-unit-testing/) testing, and finally [unit testing](https://developer.ibm.com/watson/blog/2016/11/21/cognitive-system-testing-so-i-dont-need-to-unit-test-my-cognitive-system/).  The series is a great overview of cognitive testing concepts.

There are also some good tools available to help you in you testing of your Watson cognitive services.  There is the [Watson Cognitive Testing Framework](https://github.com/joe4k/wdcutils/) for measuring performance, which provides several commonly used performance metrics of custom ML models (Accuracy, Precision/Recall/F1, Confusion Matrix, AUC).

### References for Further Reading
- [Andrew Freed Blogs](https://developer.ibm.com/watson/blog/author/afreed/) - Andrew has done some thinking about cognitive testing, his blog posts will give you some insight into solid testing approaches.
- [Cognitive Quality Assurance \- An Introduction](https://brainsteam.co.uk/2016/03/29/cognitive-quality-assurance-an-introduction/) and [Cognitive Quality Assurance \- Performance Metrics](https://brainsteam.co.uk/2016/05/29/cognitive-quality-assurance-pt-2-performance-metrics/) - both authored by James Ravenscroft, with some good advice and introduction to the concepts of accuracy, precision, recall, and confusion matrices.
- [Watson Cognitive Testing Framework](https://github.com/joe4k/wdcutils/) - a great set of Python Notebooks for measuring the performance of NLC, Assistant, NLU, and Visual Recognition.  Also check out the blog post, [Train and evaluate custom machine learning models of Watson Develper Cloud](https://developer.ibm.com/dwblog/2017/machine-learning-custom-models-watson-developer-cloud/), which introduces this framework and discusses how to use it.


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
- [Watson Developer Cloud (GitHub)](https://github.com/watson-developer-cloud) - this GitHub repository has commonly used SDK's (software development kits) and code for some interesting demos.  Some of the SDK's included here are listed below, but you should check this site for other less common SDKs as well.
  - [.NET SDK](https://github.com/watson-developer-cloud/dotnet-standard-sdk)
  - [Python SDK](https://github.com/watson-developer-cloud/python-sdk)
  - [Node SDK](https://github.com/watson-developer-cloud/node-sdk)
  - [Unity SDK](https://github.com/watson-developer-cloud/unity-sdk)
  - [Swift SDK](https://github.com/watson-developer-cloud/swift-sdk)
  - [Java SDK](https://github.com/watson-developer-cloud/java-sdk)
  - [Android SDK](https://github.com/watson-developer-cloud/android-sdk)

---
# Common Tips and Tricks
This section will cover some of the common tips and tricks used by cognitive develpment professionals, and covers some of those things that are not addressed in the documentation.

- [Bluemix Tips and Tricks](docs/bluemix_tipstricks.md)
- [Bluemix Landing Page](https://github.com/dtoczala/bluemix-landing-page) - a similar project to this one, except it is focsed on the Bluemix Platform.

## Staying Aware of Watson and Cloud Best practices
There are some very good sources for current material on best practices with the Watson services.  Often these are published in a few "hotspots", and it's possible for you to monitor these so you are always aware of the latest information.  Here are some RSS feeds to some key "hotspots":

- [RSS feed for Cloud Computing blogs on developerWorks](https://developer.ibm.com/dwblog/category/cloud-computing/feed/)
- [RSS feed for Cognitive Computing blogs on developerWorks](https://developer.ibm.com/dwblog/category/cognitive-computing/feed/)
- [IBM Watson page on Medium](https://medium.com/ibm-watson) - seems to have quick notes on what is new and what is newsworthy in the Watson world - not always technical, but informative.

_Note: You can also follow your favorite author by subscribing to an RSS feed for just their content.  The RSS feed follows this format:_
```
https://developer.ibm.com/dwblog/author/<author_id>/feed/
```
Here are some examples:
- To follow Dan Toczala's content, use https://developer.ibm.com/dwblog/author/dtoczala/feed/.
- To follow Joe Kozhaya's content, use https://developer.ibm.com/dwblog/author/kozhaya/feed/
