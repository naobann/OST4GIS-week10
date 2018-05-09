# Final Project Proposal

Your assignment this week is to write a detailed proposal for your final
project. In proposing your final, try to address each of the following
areas.

## Problem / Question

Applications are ultimately just tools. What problem or question does
your application attempt to resolve or grapple with? How does your
application speak to this problem/question?

My final project is a public information platform for all stakeholders in animal
welfare of stray animals.
This is an application to visualize stray animals and rescue shelters
in Austin, TX. It is a visualization tool for people in Austin who just lost their
pet to find out whether their pets have been found, they can do so by screening
recent lost animals within selected radius of their location. This is also a tool that helps
rescuers to analyze the locations that stray animals are usually found, and it also
gives city residents a chance to see how many stray animals within their residence,
and probably a good source of identifying possible adoption.

## The data

Geospatial applications are all about working with data. What datasets
would you plan/like to use? If the data you'll be working with isn't
already stored in a way that you can use, how will you be storing your data?
(If it is too large for a javascript application, using a backend might
be necessary)

The dataset I'm going to use is the Austin Animal Center Found Pets dataset made by
City of Austin.( https://data.world/cityofaustin/kz4x-q9k5 )I'm going to
transform it into GeoJSON file and store it on my GitHub account and access by
GitHub raw data link.

## Technologies used

Which technologies covered in class (or discovered on your own!) do you
plan to use? How do you anticipate using each of these technologies?

Review the APIs/online examples of leaflet, turf, jQuery, underscore (or
any library not explicitly covered in class) for functions/uses which
you'd like to explore. Briefly describe how you might use them.

The methodologies used are primarily in two parts:
1. Map and dataset plotting, user-interactive selective plotting, and popup.
2. User-interactive draw of circle on the map and calculate the number of markers
in the circle.

The methods used are Leaflet plotting, Leaflet Draw, and some JS functions.

## Design spec
The design is devided into two parts: leftside sidebar part and right side map part.
cats, dogs, and shelters all have different colors to differentiate.

#### User experience

At a high level, how do you expect people to use your application?
- Who are the users?
- What do they gain from your application' use?
- Are there any website/application examples in the wild to which you can compare your final?

The users are the owners who just lost their pets, animal rescuers, and potential
adopters. The owners could use this map to screen the animals lost within certain
radius of the location where their pets got lost to find out whether their pets
have been rescued by animal shelters. Animal rescuers could use this map to analyze
and summarize the locations that animals are most often found, and by doing so,
possibly better arrange for their future rescue work geographic emphasis. potential
adopters could look at this map and see if there are any stray animals of interest
that they want to adopt. Also, this website serve as a public information platform
for all stakeholders of animal welfares.
#### Layouts and visual design

So far, we've built all our applications with a side bar for
representing non-map content and navigation. This is not the only
successful design. Extra content could be displayed in a top bar,
through modals, through side bars on both sides, and any combination of
these as well as a number not mentioned. Try to describe your
application's visual layout. Conceptually (no need for extensive CSS
here), what will this design require?

I will do with side bar as the information displayed may be a lot (the list of
  animals selected), a side bar with scrolling feature would be good.

## Anticipated difficulties

Thinking about weaknesses can be useful. What do you anticipate being
most difficult about this project? How will you attempt to cope with
these difficulties? For example, asynchronous behavior (ajax, events)
are hard to use and think about. Global variables are a strategy for
coping with that difficulty by breaking data out of the asynchronous
context.

Most skills needed for the first part of the project are covered before mid term
so I will be comparatively comfortable with it. The difficulties are in the second
part where I need to count the number of markers within a user-identified circle.
To do so I want to use Leaflet Draw and Turf.

## Missing pieces

We've only managed to scratch the surface of the available technologies
by which you could construct an application. What use-cases haven't we covered
that you think would be useful? What technologies not covered seem exciting to
you (you don't necessarily have to fully understand what they're for,
this is a chance for you to get our help interpreting a technology's
purpose/usage).

I want to do real-time data input in this project but as the data is updated on
the government website every week or so (rather than a real time data sharing website
with usable link), this is not approachable. Now I plan to use only the most recent
week data (from April 30 to May 8, 2018).
