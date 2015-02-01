# Phase 2: Finish JSON API, be able to upload pictures, profile page

## Rails
### Models

### Controllers
Api::UsersController (create, show)
Api::UserViewsController (create, index)
Api::ImagesController (create, destroy, show)
Api::ImageLikesController (index)

### Views
* users/show.json.jbuilder
* images/index.json.jbuilder

## Backbone
### Models
* User (parses nested images if present)
* UserView
* (Needed?)Image

### Collections
* (Needed?)Images
* UserViews

### Views
* UserShow (composite view, contains ImageIndexItem subviews)
* ImageIndexItem
* ImageNew

## Gems/Libraries
* 'filepicker.io'
