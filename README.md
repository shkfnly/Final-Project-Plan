# model findr

[Heroku link][heroku]

[heroku]

## Minimum Viable Product
Model findr is a clone of Flickr with only some of its features. It allows
users to state whether they are a photographer or model. Based on that
information, they may discover other users who are also a photographer or model
by city. They may also see other users who are popular in their area. Users can:

- [x] Create accounts
- [x] Create sessions (log in)
- [x] Upload pictures to their portfolio
- [x] Have a profile page with all their details and pictures
- [x] View their pictures, as well as other user's pictures
- [x] Search by city for other users
- [x] View other user's profile pages, as well as view their portfolio
- [x] See the most popular users the city that the current user lives in (Explore page)

## Design Docs
* [View Wireframes][views]
* [DB schema][schema]

[views]: ./docs/views.md
[schema]: ./docs/schema.md

## Implementation Timeline

### Phase 1: User Auth, Investigate Picture storing, maybe JSON API routes (~1 day)
I will implement user authentication in Rails based on the practices learned at
App Academy. By the end of this phase, users will be able to create an account
and view their own profile page. I will have to look into how picture storage
works. I will also start adding JSON API routes if there is time. The most
important part of this phase will be pushing the app to Heroku and ensuring
that everything works before moving on to phase 2.

[Details][phase-one]

### Phase 2: Finish JSON API, be able to upload pictures, profile page (~2 days)
I will finish API routes to serve user data as JSON, then add Backbone
models and collections that fetch data from those routes. Users should be able
to view their own profile page. By the end of this phase, users should be able
to upload pictures into their "portfolio", and set their profile picture upon
creation of their account.

[Details][phase-two]

### Phase 3: Most popular users in the world (explore), and your city (~2 days)
I'm going to have a tab on the navbar called 'Explore' which lists the most
popular users registered on the site (probably top 20). Make corresponding
Backbone view. Do the same for most popular users in the current user's city.
The tab for most popular users in the city will be called "Your City". Under
the "Explore" and "Your City" tab, I'd like to have a button that switches from
most popular users, to most liked pictures. I assume this will take the whole
second day.

[Details][phase-three]

### Phase 4: Search bar (~1-2 days)
I'll probably have to use Google Maps API in order to have a nice search bar.
When a user types in the search bar, I want to have matching cities pop up as
the typing is happening. It would be nice to also be able to switch from
searching cities to searching for individual users. I'm not sure exactly how
this going to work yet, but I'll roll with it. I also want to make the Backbone
view for the users of that city.

[Details][phase-four]

### Phase 5: Showing and liking a photo, styling (~2 days)
It should be possible to like a picture without showing it. I hope I have time for
styling :(

[Details][phase-five]

[phase-one]: ./docs/phases/phase1.md
[phase-two]: ./docs/phases/phase2.md
[phase-three]: ./docs/phases/phase3.md
[phase-four]: ./docs/phases/phase4.md
[phase-five]: ./docs/phases/phase5.md
