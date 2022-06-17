# Project-Prep 4

**Project Management Board**
https://regex-rejects.atlassian.net/jira/people/team/8fa0b522-338a-48bd-9cf3-3225db255fc2

**Wireframes**
<img width="1033" alt="Screen Shot 2022-06-17 at 4 00 46 PM" src="https://user-images.githubusercontent.com/91853244/174410813-7044ead6-09fd-4025-9512-eab647157098.png">


**User Stories**

1. Weather API Data
   - As a user, I want to access up-to-date weather forecasts for a given location and date range, so that I can use that information to plan an upcoming trip.
   - Feature Tasks:
     - User can specify data query based on location and time range
     - User’s query is met with a visually pleasing, and easily digestible, display of the requested weather data
   - Acceptance Tasks:
     - Ensure validation for location in case user enters a location query not valid for weather API (i.e. outside of U.S., spells location wrong, etc.)
     - Ensure user cannot select dates outside of the range available for the given API, or have error handling for when data does not exist for any dates in their range
2. Persist User Data
   - As an end-user, I want to be able to save particular location and data range pairs as a “saved trip” so that I can come back to it over time and get more information as i plan my travel and stay.
   - Feature Tasks:
     - User has ability to “log in” (perhaps through third party Auth or locally) so data can be persisted that is specific to user via their login credentials (i.e. email or username/ID)
     - Logged-in user has an “add” button available after receiving valid query results that creates a new Trip object in the database that holds the location and date_range attributes
     - Saved/persisted Trip objects can be accessed by the user to update location or date_range, or to delete Trip object
     - Trip objects can be accessed by the user to return the weather+ API search results specific to the saved location and date_range
   - Acceptance Tests:
     - Ensure login credentials (unique user identifier) are automatically added as attribute to any saved/persisted Trip objects; users can see/access all their Trip objects but only their Trip objects
     - Ensure that the Trip objects successfully persist to the database
     - Ensure full RESTful CRUD capability for add, update, and deletion of Trip objects
3. Frontend Interface
   - As an end-user, I want a web application interface that is as intuitive and frictionless as possible, so that I don’t need to seek out other less complicated, confusing, or time-consuming tools for my trip planning.
   - Feature Tasks:
     - User sees and interacts with aesthetically pleasing, familiar looking search bar at eye-level / central focal point of screen
     - User is prompted (either before or after search) to login / be authenticated so they can save Trip data
     - User can see top-line summary list of saved Trips from any screen without needing to leave, but can click to go to the page for that Trip
     - Site has a unique branded color-scheme that is consistent for all rendered components (forms, text displays, buttons, icons, images, etc.)
     - Site has responsive design (will look good if viewed on either desktop, tablet, or mobile device)
   - Acceptance Tests:
     - Ensure specific (yet basic) styling guide is agreed up by design team earlier on, and adhered to (both for pleasant and consistent aesthetic, and for achieving responsive site design)
     - Frontend design tools should be simple to work with, yet flexible so too much time is not spent on fixing frontend issues but various components and functionality can be added / scaled up in the event of additional API data displays for user’s search results
4. iFrame(s) (FRONTEND STRETCH GOAL)
5. Additional APIs (BACKEND STRETCH GOAL)

**Domain Modeling**
<img width="1148" alt="domain model" src="https://user-images.githubusercontent.com/91853244/174410343-1e59fee0-c56c-412e-9b5b-f9717b495c95.png">

**Database Schemema** 
![401 Final Database Schema](https://user-images.githubusercontent.com/91853244/174410421-aa1f4046-83b0-4377-b21f-a03bf4072702.png)


