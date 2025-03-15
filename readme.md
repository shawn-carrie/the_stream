# The Stream (App)

A (web-based?) application which supports Ukrainian activists and communities to showcase their work, fundraise, and reach new audiences.

## Features Spec
- user login & authentication
- public user profile pages with user-uploaded content
- relational database of people, campaigns, collection jars
- integration with [MonoBank API](https://api.monobank.ua/index.html)
- image generation functionality

## Database Structure
- People
- Projects (Campaigns)
- Jars (Monobank, other?)

- A **Campaign** is a collection with a large fundraising goal 
- **People** involved (and vice versa)
- **Jars** can be related to other jars as parts of a whole


## User Experience - For Organizers

1. Users create a personal account on the app
1. User is presented with options:
 - Create New Campaign
 - Add a Jar to an existing Campaign

**Add Jar to Exisiting Campaign**
- User is prompted to choose from a list of campaigns
- Upon selecting one, user is shown a preview of the Campaign, and asked to confirm
- User is then prompted to add the [Monobank Jar link / API token?] _(what is required?)_
- The **Jar** and the **Campaign** are then linked in the database

**Create New Campaign**
 - Campaign name 
 - Total Goal
 - Description
 - Collection Image Template 


1. Upon successfully creating a **Campaign**, the Organizer is prompted with the **Add Jar to Exisiting Campaign** dialogue
1. Organizer can generate links to invite new users to join their Campaign, which takes the new user to a page where they create an account, then subsequently to the **Add Jar to Exisiting Campaign** dialogue, with the Campaign pre-filled

**Display Personal Profile Page**

1. Participants in the joint collection can customize & download personalized images to share to social media to promote their collection jars 

 - Integration with MonoBank API to get current Jar Balances
 - Calculate balances of linked Jars, % of total, etc.



**Display Campaign Information**
- The page for each Campaign displays data:
 	- Campaign Basic Data (Title, Description)
	- Total Campaign Goal Amount
	- Total Raised, Calculation of percentage (computed by database: sum of linked jars / Total)
	- Results Section: Uploaded Photos & Videos

**For Donors**

1. Do donors need to log in?
1. Donor follows a link shared on social media and navigates to a page dedicated to a specific Collection, clicks on Donate
1. User completes payment
- _Is this possible within same page or app, without navigating away?_
1. After payment is completed, user is redirected to a thanks page, where they view a "special thanks" video from the creators and can download personalized images to share on their social media (these are uploaded by the Campaign Organizer)
1. (User is _then_ prompted to optionally create an account, at the end of the process)

## Next Steps

- Review & complete functional spec (Shawn, Drew)
- Phone Call (Drew, Artem)