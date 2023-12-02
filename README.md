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

Owner/Administrator/Manager:

As a manager, I want to make sure only the best quality services are being offered for competitive price.
Also want to make sure the most competitive services are ranked on the top and featured on our site.

_____________________________________________________________________________________________________________

[Operations/Functionalities]

Operation 1: Owner/Administer will manage client and service provider detail and access to the system

            Functionality:
            a. Owner/Administrator will create, edit and update the clients and service provider personal details. 
            b. allow access of clients to the system. This will trigger notification to the clients of their permission to access.
            b. monitor the clients requests
            c. adjust the discount according to the latest market conditions.
            d. view clients and Service provider history
            e. view financial details.

Operation 2: Service provider to manage their services

            Functionality:
            a. Service provider will accept the invitation from owner/administor and update their profile.
            b. Service provider setup payment method (Payment goes only to the owner)
            c. Service provider create service category lists and with their offer of discount

Operation 3: Service provider view request from clients, decide to accept or reject, if accepted then contact client to provide service

            Functionality:
            a. Service provider to accept/deny requests from the clients
            b. service provider contacts clients through available contact information
            c. service provider complete the service and close the request.

Operation 4: Client user view the discount by category on the front page and decide to register to request the service

             Funtionality:
             a. Client can register with the system
             b. Client can create/update their profile.
             c. Client can browse services and the discounts based on the client history.
             d. Add number of services to the shoppig cart.
             e. Submit requests to the service provider (Service provider's contact is hidden)
             f. View status of the requests.
             g. Rate and feedback each requests after receiving the services.

______________________________________________________________________________________________________________
[Data Structures / Tables]

Administrator
  - userid
  - first_name
  - last_name
  - user_name
  - password
  - email
  - active
    
Service_Providers
  - Service_Provider_id
  - First_Name
  - Last_Name
  - User_Name
  - Password
  - Address
  - Email
  - Phone
  - address
  - Service_Provider_Type (Corporation/Individual)
  - service_category (Real Estate, Plumbing, Electrical....)
  - Regular_Price
  - active

Service_Category
   - category_id
   - category_name
   - category_description
   - min_discount

Service_Listing
  - service_listing_id
  - Service_provider_id
  - category_id
  - listed_date
  - Discount

Clients
  - Client_id
  - First_Name
  - Last_Name
  - User_Name
  - Password
  - Address
  - Email
  - Phone
  - Active

Sales
  - Sales_id
  - Client_id
  - Service_Provider_id
  - Service_listing_id
  - Sales_description
  - Client_Request (Yes/No)
  - Retailer_Confirmation (Yes/No)
  - actual_discount (must be equal or more than set discount) 
  - Active (yes/no)
  - Close (yes/no)

______________________________________________________________________________________________________________

[Business Rules]

- Public can view services without discount. No registration needed.
- Only the clients who registered has discount and request for services.
- Clients and Service Providers score points based on history. High score clients and Service providers has better discount and got priorities for services.
______________________________________________________________________________________________________________

[ Entiry relationships]

- One Service provider may have many services.
- One service provider create many serivce listings
- One Client can access many service listings
- Many Clients can have many Sales transactions

______________________________________________________________________________________________________________

[Defining views]

