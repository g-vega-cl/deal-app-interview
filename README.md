
# Local development
0. Make sure you have node.js installed, we use version 18.14.2
1. *Optional if you use nvm*:  Run `nvm use` to use the correct version of nodejs.
2. run `npm i` to install required packages.
3. run `npx expo start` to start local development.


Now you should see a QR code in the terminal.
You see the app in you phone by scanning the QR code in the Expo Go App on Android or using the Camara App on iOS.

You can also press "w" to see the app in your web browser. But make sure you keep track of the dimensions of a phone screen. For this you can open the developer tools (command + option + J) in chrome based browsers or (command + option + i) for firefox. 
    * control + shift + j/i on Windows/Linux

You should now see your app and your changes in real time.

# Development guidelines
For this app we use the React Native Elements UI framework: https://reactnativeelements.com/ And React Native components


# Requirements for your submission
This is the good part. You need to create a pull request so that the code homepage looks similar to this:

![Landing page](https://github.com/g-vega-cl/deal-app-interview/blob/main/readme-images/deal-app-interview-gif-example.gif?raw=true)

2. EXTRA: The VIEW NOW button should open a modal with product information like price, compare_at_price, and updated_at (with properly formatted date)
3. EXTRA: Make sure there is a loading or error page if there is an error with fetching data.
4. EXTRA: Make it pretty!
# Good practices:
1. Small commits are better than one large commit. This also shows you know git
2. Divide your code into components and import them. It's better to have a codebase component like `<App> <Header /> <Card /> <Footer /> </App>` than a single file with all the code.
3. Don't assume product information is complete. Take into account scenarios where data could be undefined.
4. Styles should be consistent across a component, avoid creating two card components with different styles.


# FAQ:
1. I can't run "npx"
    * It's likely that you don't have it installed OR that you don't have it in your path.
    * run `npm install -g npx`
    * If it doesn't work after running the previous command, check your PATH (google it).
    * A useful article https://www.freecodecamp.org/news/npm-vs-npx-whats-the-difference/

2. Does this app has a backend?
    * This app does have a backend. It's pre-made and the only function implemented is: `getShopifyProducts`, which lives at `https://deal-app-backend.vercel.app/getShopifyProducts`
