# Final Project Proposal

Your assignment this week is to write a detailed proposal for your final
project. In proposing your final, try to address each of the following
areas.

## Problem / Question

Applications are ultimately just tools. What problem or question does
your application attempt to resolve or grapple with? How does your
application speak to this problem/question?

If you are planning a road trip to see national/state parks, there isn't
a great resource available. My application will be like Google Maps where
you can create a route, but it will then tell you what state or national
parks are along the route. That way you can plan to see America's nature
without going too far out of your way.

https://roadtrippers.com does this a bit. But their site is messy and has stuff
that I don't care about, like hotels or tourists traps. I want my site to be
very simple - just state/national parks and forests.

## The data

Geospatial applications are all about working with data. What datasets
would you plan/like to use? If the data you'll be working with isn't
already stored in a way that you can use, how will you be storing your data?

The data is all on Wikipedia. I've been using R to webscrape so I currently have
all the national data and 40 states. R makes it easy to manipulate data so I
can have coordinates in a readable format for mapping and photos or descriptions
for a popup.

## Technologies used

Which technologies covered in class (or discovered on your own!) do you
plan to use? How do you anticipate using each of these technologies?

Review the APIs/online examples of leaflet, turf, jQuery, underscore (or
any library not explicitly covered in class) for functions/uses which
you'd like to explore. Briefly describe how you might use them.

R - webscraping
mapbox - Making basemaps. I've already made a light pollution basemap and a terrain basemap
leaflet - the map
mapzen - Get routing information and make a buffer around route to see what parks are nearby
carto - Nathan recommended this for the markers as it is fast and I'll have ~3000 markers
jQuery - editing my page to add directions - like in week 9


## Design spec

#### User experience

At a high level, how do you expect people to use your application?
- Who are the users?
- What do they gain from your application' use?
- Are there any website/application examples in the wild to which you can compare your final?

The main user will be me because I want to do a parks roadtrip after I graduate.
Anyone who is interested in a roadtrip to see parks can use it. They gain because it'll be
a simple website that does one thing (shows parks on the route) but does it well.

#### Layouts and visual design

So far, we've built all our applications with a side bar for
representing non-map content and navigation. This is not the only
successful design. Extra content could be displayed in a top bar,
through modals, through side bars on both sides, and any combination of
these as well as a number not mentioned. Try to describe your
application's visual layout. Conceptually (no need for extensive CSS
here), what will this design require?

I want it to be similar to Google Maps. Full screen map with a transparent
panel showing details on what you click. All of the parks will be on
the map as dots and those within a buffer of the route (buffer distance set by user)
will be a different color.

## Anticipated difficulties

Thinking about weaknesses can be useful. What do you anticipate being
most difficult about this project? How will you attempt to cope with
these difficulties? For example, asynchronous behavior (ajax, events)
are hard to use and think about. Global variables are a strategy for
coping with that difficulty by breaking data out of the asynchronous
context.

Getting all the data will be time consuming - lots of cleaning work, especially
getting all the images. It's not really difficult, just long to do.
I want the site usable if I'm on the road which means
it has to work without internet or slow internet which I'm not sure how to do.
I'm also fairly bad with making pages look good. This weeks assignment will help
with that. And it seems to be something that just takes practice and time.

## Missing pieces

We've only managed to scratch the surface of the available technologies
by which you could construct an application. What use-cases haven't we covered
that you think would be useful? What technologies not covered seem exciting to
you (you don't necessarily have to fully understand what they're for,
this is a chance for you to get our help interpreting a technology's
purpose/usage).

More focus on buffers. And working with user interactions. We've done user input
but it'd be cool to make stuff that more complex user interaction. 
