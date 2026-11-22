# TraceIT: Product Requirement Document

## Product Overview:
  BUfind is a website where Babcock students and staff can report lost items,
  register found items, search lists, an admin will confirm the ownership of that property.

## Problem Statement:
  Students and staffs lose items like phones, keys, ID cards etc. 
  Reports, complaints will be scattered around  and most times not answered or extremely difficult to find,
  and people don't have evidence on that item and it's almost unreliable to confirm who owns the item.

## Target users
- Students and staffs:reporting their lost items and the ability to claim it. 
- Administrators such as student affairs or security or any other body will review,
    verify and record returns and complaints
## User stories
- Users must be able to register and log in to the site
- Users should be able to filter and search for their lost items so they can find it faster
- Users should be able to report a lost item so it could be found
- Spotters should report a missing item they find with a photo and location
- Spotters should be able to add identification details so that only the real owners can get it
- Owners should be able to submit a claim with proof
- Claimers/obtainers should be able to track their status
-  Admins should accept or reject claims so that the lost item get to the rightful owner
- Admins must mark records as returned to make sure records stay accurate

## Requirements
### Functional Requirements
-  Users can register, log in, and log out.
- After logging in, the user sees a dashboard with two options: *Report Lost Item* and *Report Found Item*. The system shows the form that matches the choice.
-  Users can report a lost item by entering its name, category, description, last known location, date lost, and an optional photo.
-  Users can register a found item by entering two types of details:
  - Public details: item name, category, general description, photo, location found, and date found. These are displayed in listings and item pages and are used when users browse or search.
  - Private details: identifying information only the owner would know, entered in a free-text field with suggested prompts based on the item's category. At least one private detail is required.
-  Private details are stored separately and never shown in listings, item pages, or search results. Only administrators can view them.
-  Users can browse listings and view the public details of an item.
-  Users can search and filter listings using public details only (keyword, category, location, date, and type).
-  Users can submit a claim on a found item by answering verification questions about it.
- Administrators compare the claimant's answers with the item's private details, then approve or reject the claim.
-  Administrators can mark an item as returned after the claimant shows their university ID.
- Items have a status: Lost, Found, Claim Pending, Returned, or Closed.
### Non-functional Requirements
- Security : passwords are hidden and admin features are restricted by role
- Privacy: private item details should be visible to only Admins
- Performance: search loads should be very quick
- Usability: Must be able to work on Phones, desktops and other gadgets
- Reliability: data should be stored in a database 
- Flexibility

### MVP (Minimum Viable Product)
- Registration and login with user and admin roles
-  Reporting lost and found items with photos and a very good description
- Listings, item details, search and filters
- Claim submission
- Admin claim, review and return
- Status tracking

### Acceptance criteria
- Given valid details, when user registers then an account is created and the user logs in
- Given a completed form, when submitted then the item appears in Listings with status "found" and it's private details should not be made public.
- Given a keyword, when a user searches, only matching items are shown or a "no results" message appears.
- Give a found item, when a user submits the claim, the status should change to claim pending and when approved by the admin, the claimant is to collect it and if admin rejects, status changes back to "found" and when an admin marks it as returned then status changes to returned.

### Scope: website, user and admin roles, reporting, search and claims, verification status tracking
Projects and works: mobile apps (optional), integration with Babcock system, tracking. 

Priorities: the MVP,
What you can have: notifications and suggested matches

Questions:
1. How long should found items be kept
2. Which office holds the items 
3. What structure can be used to keep the found items
