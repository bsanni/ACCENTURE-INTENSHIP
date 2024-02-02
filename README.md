**INTRODUCTION**
I joined the Accenture Data Analytics virtual internship through Forage, taking on the role of a data analyst to aid the organization "Social Buzz" in the analysis of their data. My objective was to help them harness the full potential of their substantial data assets. The project involved three primary responsibilities: comprehending the project, refining and modeling the data, and crafting data visualizations along with compelling storytelling.

**TASK 1: PROJECT UNDERSTANDING**

Client Information:
•	Client Name: Social Buzz
•	Client Industry: Social media and Content Creation
•	Establishment Year: 2010
•	Employee Count: 250

**Client Background:**
Social Buzz originated in 2010 through the collaboration of two former engineers—one hailing from London and the other from San Francisco. Both had previously worked for a major social media conglomerate and, after leaving their positions in 2008, united in San Francisco to establish their venture. The impetus behind creating Social Buzz arose from their recognition of an opportunity to build upon the foundations laid by their former employer. Their vision was to forge a unique platform that prioritizes content.

Highlighting the significance of content, Social Buzz adopts an exclusive approach by upholding user anonymity and solely tracking user reactions to each piece of content. The platform features an extensive array of over 100 reaction options, surpassing conventional responses such as likes, dislikes, and comments. This distinctive strategy ensures that trending content, rather than individual users, takes center stage in user feeds.
PROBLEM STATEMENT: Over the past five years, Social Buzz has experienced rapid growth, amassing a monthly user base of over 500 million active participants. The unexpectedly substantial success has necessitated the engagement of an advisory firm to oversee and optimize their ongoing expansion process efficiently.

Due to their swift expansion and the digital essence of their primary product, Social Buzz generates, collects, and analyzes an immense volume of data. On a daily basis, more than 100,000 pieces of content, encompassing text, images, videos, and GIFs, are posted. The entirety of this data is highly unstructured, demanding sophisticated and costly technology for effective management and maintenance. Among the 250 individuals employed by Social Buzz, 200 are technical staff dedicated to maintaining this intricately complex technology.

Until now, Social Buzz has been self-reliant and has not sought external assistance to reach its current status. However, three primary reasons have prompted them to consider leveraging external expertise:

1.	They aim to undergo an Initial Public Offering (IPO) by the conclusion of the next year and seek guidance to ensure a smooth transition to a publicly traded company.
2.	Despite their significant growth, they remain a relatively small company and lack the resources to effectively manage their current scale. While hiring more personnel is an option, they prefer the expertise of an experienced external partner.
3.	They aspire to adopt data best practices from larger corporations. Given the substantial volume of data integral to their business, they are eager to glean insights into how leading global companies tackle the challenges associated with big data.







My Task as a Data Analyst: Analysis of sample data sets with visualizations to understand the popularity of different content categories.
TASK 2: DATA CLEANING AND MODELING
I was provided with seven datasets and a data model. My first step is to use this data model to identify which datasets will be required to answer my business question — figuring out the top 5 categories with the largest popularity.
 
**Data Model**

![image](https://github.com/bsanni/ACCENTURE-INTENSHIP/assets/101055903/4ac9f25a-bf80-4710-9019-67c2a7e1ee5e)







Below are details about the datasets and the columns they contain.
User
The User table comprises three columns: ID, representing the unique user identification (automatically generated); Name, indicating the full name of the user; and Email, containing the email address of the user.
Profile
The Profile table consists of three columns: User ID, representing the unique identification of a user existing in the User table; Interests, containing the interests of the associated user; and Age, indicating the age of the associated user.
Location
The Location table includes two columns: User ID, which is the unique identification of a user existing in the User table, and Address, representing the full address of the user.
Session
The Session table comprises three columns: User ID, denoting the unique identification of a user existing in the User table; Device, specifying the mobile device used by the user for the session on the application; and Duration, indicating the amount of time in minutes that the user remained active on the application during this session.
Content
The Content table encompasses five columns: ID, representing the automatically generated unique identification of the uploaded content; User ID, denoting the unique identification of a user existing in the User table; Type, a string describing the type of uploaded content; Category, a string specifying the relevant category of the content; and URL, providing a link to the location where the content is stored.
Reaction
The Reaction table includes four columns: Content ID, representing the unique identification of an uploaded piece of content; User ID, denoting the unique identification of a user existing in the User table who reacted to this content; Type, a string describing the type of reaction given by the user; and Datetime, indicating the date and time of this reaction.
ReactionTypes
The ReactionTypes table consists of three columns: Type, which is a string specifying the type of reaction given by a user; Sentiment, a string indicating whether this reaction type is categorized as positive, negative, or neutral; and Score, a numerical value calculated by Social Buzz that quantifies the “popularity” of each reaction. A reaction type with a higher score is deemed more popular.
For my analysis, I’ll be focusing solely on the Reaction, Content, and ReactionTypes tables, disregarding the other four tables in the dataset.
However, before delving into the analysis of the datasets, it is essential to ensure that the data is clean and prepared for analysis.

