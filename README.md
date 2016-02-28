# Tweater

An android app that allows a user to view their Twitter timeline and post a new tweet. The app utilizes [Twitter REST API](https://dev.twitter.com/rest/public).

Time spent: 10 hours spent in total

## User Stories

- [x] User can switch between Timeline and Mention views using tabs. (4 points)
- [x] User can view their home timeline tweets.
- [x] User can view the recent mentions of their username.
- [x] User can navigate to view their own profile (3 points)
- [x] User can see picture, tagline, # of followers, # of following, and tweets on their profile.
- [x] User can click on the profile image in any tweet to see another user's profile. (2 points)
- [x] User can see picture, tagline, # of followers, # of following, and tweets of clicked user.
- [x] Profile view should include that user's timeline
- [ ] Optional: User can view following / followers list through the profile
- [x] User can infinitely paginate any of these timelines (home, mentions, user) by scrolling to the bottom (1 point)

The following advanced user stories are optional:

- [ ] Advanced: Robust error handling, check if internet is available, handle error cases, network failures (1 point)
- [x] Advanced: When a network request is sent, user sees an indeterminate progress indicator (1 point)
- [x] Advanced: User can "reply" to any tweet on their home timeline (1 point)
- [x] The user that wrote the original tweet is automatically "@" replied in compose (1 point)
- [ ] Advanced: User can click on a tweet to be taken to a "detail view" of that tweet (1 point)
- [x] Advanced: User can take favorite (and unfavorite) or retweet actions on a tweet (1 point)
- [x] Advanced: Improve the user interface and theme the app to feel "twitter branded" (1 to 5 points)
- [ ] Advanced: User can search for tweets matching a particular query and see results (2 points)
- [ ] Bonus: Use Parcelable instead of Serializable using the popular Parceler library. (1 point)
- [x] Bonus: Apply the popular Butterknife annotation library to reduce view boilerplate. (1 point)
- [ ] Bonus: User can view their Twitter direct messages (and/or send new ones) (2 points)efactory.com/blog/get-to-know-glide-recommended-by-google/en) for more efficient image rendering.

The following **additional** features are implemented:

- [x] Use a single fragment with a recyclerview for the User Timeline, Mentions, Home TimeLine and Profiles
- [x] Ensure clicking on a profile when on the current users profile does not trigger an additional activity
- [x] Use Gson to store UserData into shared preferences
- [x] Add a layer of abstraction on top our TwitterClient to hide some ugliness
- [x] Add a way to use mock data from save json files so I wouldn't hit the rate limiter

## Video Walkthrough 

### Basic user flow
![Alt text](/demos/twitter_flow.gif)

## Open-source libraries used

- [Android Async HTTP](https://github.com/loopj/android-async-http) - Simple asynchronous HTTP requests with JSON parsing
- [ButterKnife](http://jakewharton.github.io/butterknife/) Annotation library to reduce view boilerplate
- [Glide](https://github.com/bumptech/glide) Image downloading and caching library 
- [RecyclerView Animators](https://github.com/wasabeef/recyclerview-animators) RecyclerView Animiations
- [Prettytime](http://www.ocpsoft.org/prettytime/) Timestamp formatting
