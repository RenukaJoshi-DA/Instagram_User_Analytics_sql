# Instagram_User_Analytics_sql

**Description:**
  In this project, we are supposed to provide a detailed report for the Marketing and Investor Metric departments. This analysis will help them make a decision based on different metrics and insights.

**Dataset Description:**
Dataset contains tables such as:
**1. Users:** Stores user information such as id, username, and account created_at
**2. Photos:** Holds photos uploaded by users, linked by user_id
**3. Comments:** Contains comments on photos, with links to both the user and the photo
**4. Likes:** Represents photo likes by users; composite primary key (user_id, photo_id)
**5. Follows:** Records the follower-followee relationships between users
**6. Tags:** Contains hashtags or tags used on photos
**7. Photo_tags:** Junction table mapping many-to-many relationships between photos and tags

**Relationships Between Tables:**
**1. Users ↔ Photos:** One-to-Many (user_id foreign key in photos)
**2. Users ↔ Comments:** One-to-Many (user_id foreign key in comments)
**3. Photos ↔ Comments:** One-to-Many (photo_id foreign key in comments)
**4. Users ↔ Likes ↔ Photos:** Many-to-Many through likes
**5. Users ↔ Users:** Many-to-Many self-join through follows
**6. Photos ↔ Tags:** Many-to-Many through photo_tags

**Analytics Tasks:**
**Marketing Analysis:**
1. Loyal User Rewards: Identify the five oldest users on Instagram from the provided database.
2. Inactive User Engagement: Identify users who have never posted a single photo on Instagram.
3. Contest Winner Declaration: Determine the winner of the contest and provide their details to the team.
4. Hashtag Research: Identify and suggest the top five most commonly used hashtags on the platform.
5. AD Campaign Launch: Determine the day of the week when most users register on Instagram. Provide insights on when to schedule an ad campaign.

**Investor Metric Analysis:**
1. User Enagagement: Calculate the average number of posts per user on Instagram. Also, provide the total number of photos on Instagram divided by the total number of users.
2. Bots & Fake Accounts: Identify users (potential bots) who have liked every single photo on the site, as this is not typically possible for a normal user.

**Insights & Recommendations:** 
1. Loyal Users: Reward long-time users to enhance loyalty. 
2. Inactive Users: Launch campaigns to encourage them to post. 
3. Popular Hashtags: Use top hashtags for marketing partnerships. 
4. Contest Insights: Feature the contest winner to boost engagement. 
5. Ad Campaigns: Focus on high-registration days for ad launches. 
6. Bots Detection: Review flagged accounts for removal. 
- SQL analysis provided actionable insights for Instagram’s growth and Recommendations align with marketing and investor needs. 
