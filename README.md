# iOS User Platform
## Table of Contents
 * [App Design](#app-design)
   * [Objective](#objective)
   * [Audience](#audience)
   * [Experience](#experience)
   * [Nice to have](#next-version)
 * [Technical](#technical)
   * [Screens](#Screens)
   * [External services](#external-services)
   * [Views, View Controllers, and other Classes](#Views-View-Controllers-and-other-Classes)
 * [MVP Milestones](#mvp-milestones)
   * [Week 1](#week-1)
   * [Week 2](#week-2)
   * [Week 3](#week-3)
   * [Week 4](#week-4)
   * [Week 5](#week-5)
   * [Week 6](#week-6)

---

### App Design

#### Objective
prescription based business model that provides business deals.

#### Audience
People who are looking for date activity, restaurant, movie… cheap deals.

#### Experience
1. Users have access to local business deals and able to leave reviews/stars once the business confirm that they redeemed the deal. 
2. Users can see how many people bought a certain deal and the original price of the deal.
3. Users can see the prerequisite like time frame / preparation / how early should they arrive of the deal.
4. Users can see the name, picture, introduction, address of the business that listed the deal.
5. Users are able to search for deals based on different  categories like : restaurants,  dating activities, hanging out with friends, health/fitness, Beauty/spas, travel, deal of the day.
6. Users can save the deals they like to shopping cart.
7. Users can pay by PayPal or credit card
8. Users can buy the same deal for limited amount of time.(based on different business)
9. Users can share the deals to friends.

#### Nice to have (V2)
1. Users get better deal if they buy the deals from the same business

[Back to top ^](#)

---

### Technical

#### Screens


#### External services
* [list which APIs or external services will your app use?]
1. Yelp api for pulling out the review for business 
2. stripe api for payment

#### Internal Apis
1. get request from our database for all deals around user.
2. get request from out db for deals of the day ( advertised business )
3. get request from database for deals in different categories.
4. post request to database for deals user has saved
4. post request to database for deals user has bought
5. get request from database for saved deals
6. get request from db for redeemed deals (buy again)


#### Views, View Controllers, and other Classes
* Views
 
* View Controllers
 
* Other Classes


#### Data models
__ Mongodb 
* User:
* userId
* username
* email
* password
* savedDeals: [dealId]
* boughtDeals: [dealId]

__ Deal:
* dealId
* dealTitle
* dealBusinessID
* redeemed: Bool
* dealPrerequisite
* dealTimeFrame
* dealReview(if redeemed)

__ Business:
* businessId
* businessName
* businessAddress
* businessImgURL: [ImgString]
* businessReview(from yelp API)
* businessPostedDealsID: [dealID]

[Back to top ^](#)

---

### MVP Milestones

#### Week 1
_planning your app
* 1.  finish the basic wireframe 
* 2. finish feature discussion 

#### Week 2
1. setting up backend database, CRUD routes set up, internal API all tested on Paw/postman
2. 50% tested out stripe API
3. build out login/signup on iOS 

#### Week 3
* [goals for the week]

#### Week 4
* [goals for the week, should be finishing all core features]

#### Week 5
_starting the polish_
* [goals for the week]

#### Week 6
_submitting to the App Store_
