# mohan-final-project

About the Service Referral "ServiceConnect.com" Web based solution
__________________________________________________________________________________________________________

[Mission Statement]

This solution connects those who deliver services, corporations or individuals, to general public offering
highest possible discounts while maintaining the best quality services. 

[Mission Objectives]

The solution will rank the service providers and also the clients based on our merit points criteria and give the utmost quality of service for fraction of cost.

This is a free service to the public but they should have already signed-in to access the required services. The service
providers will pay a percentage of the sales to the Service Referral business.

They will be able to see all the best ranked service providers and eligible to get the most amount of discount and 
the best quality services compared to usually what is out there in the market.

Based on the client history, they will receive notification to any new services or promotions added into the system.

__________________________________________________________________________________________________________
[Figma Design]

https://www.figma.com/file/aBGEEWYecWnlxMqvG5Hxbb/Service-Referral?type=design&node-id=0%3A1&mode=design&t=knDnlt3lgR5kKscj-1

__________________________________________________________________________________________________________
[User Stories/Interviews]

Client User:

As a member (client) to "ServiceReferral" program, I would like to easily access the best and reliable 
services in each category for discounted price.

Service provider:

I will make sure to provide the best possible service with the best possible discount to clients through ServiceReferral 
program thus keeping the clients intact and create additonal client base.

Admin:

As a manager, I want to make sure only the best quality services are being offered for competitive price.
Also want to make sure the most competitive services are ranked on the top and featured on our site.

______________________________________________________________________________________________________________
[Data Structures]

Service Providers
  - Name
  - User Name
  - Password
  - Address
  - Email
  - Phone
  - Service Provider Type (Corporation/Individual)
  - Type of Service / Category (Real Estate, Plumbing, Electrical....)
  - Regular Price

Clients
  - Name
  - User Name
  - Password
  - Address
  - Email
  - Phone

Services
  - Type of Service
  - Location
  - Description

Service Listing
  - Service Provider Name
  - Type of Service
  - Discount

Sales
  - Client ID
  - Service Listing ID
  - Offer
  - Confirmation

______________________________________________________________________________________________________________

[Business Rules]

- Public has access to services without discount.
- Only the clients who signed up has discount.
- Clients and Service Providers score points based on history. High score clients and Service providers has better discount and got priorities for services.
______________________________________________________________________________________________________________

[ Entiry relationships]

- One Service provider may have many services.
- One service provider create many serivce listings
- One Client can access many service listings
- Many Clients can have many Sales transactions

______________________________________________________________________________________________________________

[Defining views]

