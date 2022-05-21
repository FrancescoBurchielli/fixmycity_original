## Important note
The initial project was hosted on Gitlab. I transferred the source code here for the purpose of showing it as part of my personal portfolio. 
The project has been discontinued. I am now working on an improved version 2.0, hosted on a different repo on my Github.

## Project motivation and scope
The purpose of Fix My City is to give members of a community the opportunity to easily report any issue they spot in the town they live in (broken traffic light, a damaged park bench, litter not being collected, ecc.). Reporting an issues has intentionally beend made user-friendly and playful. Citizens collect points and achieve a certain status for reporting issues. Citizens can also upvote existing issues, thus increasing their urgency. The local city council can easily detect which issues are the most urgent at any given point, thanks to leaderboards as well as changing color property of the map markers. The upvoting mechanism also address the problem of issue duplication - a citizen will most likey upvote the issue his neighbour has opened, instead of creating a duplicate.

## Tech stack
1. ReactJS
2. Redux
3. Django
4. Nginx
5. Docker
6. Gitlab CI/CD

## Features
1. User can create and edit profile
2. User can use map and search bar to navigate to his desired address
3. User can pin a specific point on the map
4. User can create an issue by sharing a picture and information on the type of issue
5. User can upvote an existing issue / remove upvote
6. Pins show a different color depending on number of upvotes of the issue
7. Pins get clustered together after a certain zoom-out threshold
8. Super-user (local city council) can mark an issue as open / in progress / resolved
9. User get points based on number of issues reported
10. User achieves a certain status (scout / knight / legend / hero) as they colllect points
11. User / Super-user can benefit from "hottest issues" page, where issues are ranked based on their urgency (number of upvotes)
12. User can see his own reported issues as part of his profile info, listed in chronological order
13. User can filter on the map for a specific issue category

## Known issues
1. Map rendering is at times slow
2. Pins on certain addresses return a civic number to which two zeros are added (e.g. 1 becomes 100)

## Next steps
1. Give the platform a more modern and fresher styling
2. Use Typescript
3. Replace Mapbox API with Google Maps API (more reliable / maintained / scalable)
4. Give the local city council the possibility to comment on an issue (e.g. to ask for additional information)
5. Give the author of the issue the possibility to reply to a government request
6. Add Jest testing framework
7. Make the website a PWA, for it to have a presence on users' mobile desktops
8. Consider replacing Django backend with Go