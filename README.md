# BrewDive
A front-end exercise using react and a few animations libraries.

> node version: v14.13.0

## How to run the app on your computer
Run the project on your computer. It will be available at 
[http://localhost:1234/](http://localhost:1234/)
```
npm install
npm run dev
```
## Ready to deploy on Netlify
Using [Parcel](https://parceljs.org/) as bundler. 
Fork the project on your Github account and deploy it on [Netlify](https://www.netlify.com/) for free. A configuration file and the deploy script are already set. 
```
npm run build
```
### Difficulties
- **_Mobile accessibility_** 
Refactoring had to be done on the styling, I originally used `vh` at many places but I realized after deploying and trying on a phone that it was breaking most of the layout. Few issues : items overlapping making interaction not possible anymore, animation happening away from their initial place.
- **_Animations_** 
The animations where a tough part, I don't have much experience with animation or SVG so I had to take time to learn and find a suitable solution for that experimental version. I finally found and adapted [wavify](https://github.com/woofers/react-wavify), a react library that can generate waves. 
For the bubbles, I used [Particles](https://www.npmjs.com/package/react-particles-js) that I have used previously. 
From the original UI/UX I had to skip the text animation part. I wasn't far but faced different issues with other states of the application; so I decided to work on what I had and move forward.
### Improvements
- **_User experience_** 
As an app targeted for mobile, It would be interesting to implement device functionalities instead of a range slider. 
A call to action to wipe the screen up and down to fill the glass with beer. 