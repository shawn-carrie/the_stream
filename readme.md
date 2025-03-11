# The Stream (App)

A (web-based?) application which supports Ukrainian creators to showcase their work, fundraise, and reach new audiences.

## Features Spec
- user login & authentication
- public user profile pages
- relational database of people, projects/campaigns, collection jars
- online store
- integration with [MonoBank API](https://api.monobank.ua/index.html)
- image generation functionality

## Database Structure
- People
- Projects (Campaigns)
- Jars (Monobank, other?)
- Products (Store)

**Projects** can have multiple **People** involved (and vice versa)
**Jars** can be related to other jars as parts of a whole

## User Experience 
**For Creators**

1. Users can customize their profile page to showcase their work, add Projects/Campaigns, Jars, and Products to their Store
1. Users can create a collection with a large goal (example: ₴100,000) and invite people to take part in partial collections toward this goal 
1. Participants in the joint collection can customize & download personalized images to share to social media to promote their collection jars 
 - _(where do these image templates come from?)_
 - Integration with MonoBank API to get current Jar Balances
 - Calculate balances of linked Jars, % of total, etc.
1. 

**For Users**

1. Users follow a link shared on social media and land on a page for a Project, Campaign, or Person
2. User navigates to a page dedicated to a specific Jar
3. User completes payment
- _Is this possible within same page or app, without navigating away?_
- After payment completed, user is redirected to a thanks page, where they view a "special thanks" video from the creators and can download personalized images to share on their social media