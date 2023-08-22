<!-- Banner Image -->
<p align="center">
  <a href="https://expo.dev/">
    <img alt="expo sdk" height="128" src="./assets/images/banner.png">
    <h1 align="center">Expo Router v2 </h1>
    <h2 align="center">step by step tutorial </h2>
    Building Apps for Crafting Static Websites for Google and Other Social Networks, as well as a Mobile App for iOS and Android  </h3>
  </a>
</p>

<p align="center">
  <a aria-label="try expo with snack" href="https://expo-router-v2-static-web-app-step-1.netlify.app/"><b>This 1 step</b></a>
 | <a aria-label="try expo with snack" href="https://expo-router-v2-static-web-app-step-1.netlify.app/"><b>Look web site for 1 step</b></a>
 |
  <a aria-label="expo documentation" href="https://expo-router-v2-static-web-app-step-1.netlify.app/">Next 2 step 📚</a>
</p>

---

- [📚 About this step](#-documentation)
- [🗺 Project Layout](#-project-layout)
- [🏅 Badges](#-badges)
- [👏 Contributing](#-contributing)
- [❓ FAQ](#-faq)
- [💙 The Team](#-the-team)
- [License](#license)

<h2 align="center">Empowering Creation: Crafting a Search-Optimized React-Native Website with expo-router v2</h2>

In this tutorial, we embark on a step-by-step journey to construct a static website on React-Native using expo-router v2. Our goal is to build a website builder and mobile app constructor all in one, with maximum search optimization. The project itself spans a considerable scope, encompassing a Multilingual Website Constructor, user registration, payment capabilities, and an array of other features.

In the upcoming chapters, we will establish the foundation of this site's structure and introduce a multitude of navigational possibilities. As we progress, we'll lay the groundwork for seamless navigation and explore the potential for dynamic, user-centric experiences.

## 📚 About this step
Creating a Search-Optimized React-Native Website and App: Your First Dive into expo-router v2

Embark on an exciting journey as we guide you through crafting your grand project – an extensive endeavor designed to encompass essential technologies for aspiring FULL STACK developers. This comprehensive guide offers a step-by-step approach, addressing common challenges while unleashing the potential of expo-router v2. Each obstacle, rather than a hindrance, becomes a stepping stone to enhance your application.

Step-by-Step Guide:

1. Begin by creating a project folder with your chosen title.
2. Open the folder in VSCode's terminal and execute the command: npx create-expo-app@latest --template tabs@49
3. Once prepared, navigate to the project folder and launch it with npm start.

4. If you don't already have the expoGo app, now's the perfect time to install it on your phone. Despite the current project's browser compatibility on your computer, it's essential to have the app for testing. Install the app and open your project on your phone. For those unfamiliar with project structure, a brief video tutorial provides insights into the architecture and navigator functionality.

5. Open your GitHub repository, create a new project, and execute the necessary commands. However, refrain from making a PUSH just yet. Prior to that, we need to export the project.

6. Our project is already equipped with settings to generate a static HTML site during export. Additionally, we can obtain a React SPA, which will prove useful when working with Redux. Pause the project execution and use the command npx expo export -p web in VSCode's console.

<h3 align="left">Problem 1: EXPO-ROUTER v2 </h3>
There may be an error during export, necessitating the installation of the sharp-cli package with npm install sharp-cli. After a successful export, a dist folder emerges at the project root – your inaugural static website.

Or simply start with this template.

7. Avoid rushing to PUSH your code; it serves little purpose for publishing your site. First, open .gitignore at your project's root.

<h3 align="left">Problem 2: EXPO-ROUTER v2</h3>
dist folder, marked as ignored, must be removed from .gitignore.

Now, execute the commands as prompted by GitHub, starting with git init and git add&nbsp;. (note the space between git add and the dot). Follow the subsequent commands in the order specified on GitHub's page.

8. With our project, including the dist folder, now on GitHub, we're ready to publish it on free hosting platforms such as Vercel or Netlify. After logging in, select "ADD A SITE FROM GITHUB." However, take heed: when configuring for publication, avoid selecting any framework. Instead, clear existing settings and add "dist" to PUBLISH DIRECTORY.

Congratulations! Your site is now published.

Chances are your expo-router v2-based static site might not load properly after publication, showing an error message: "SOMETHING WENT WRONG, TRY AGAIN."

My experience led me to discover a solution. Perhaps this issue is resolved now, allowing you to skip the next step. Nevertheless, I had to:

<h3 align="left">Problem 3: EXPO-ROUTER v2</h3>
Comment out the problematic code in /app/_layout.tsx:

// if (!loaded) {<br/>
// return null;<br/>
// };

Now, re-export and publish.

Hurrah! Your first React-Native static site using expo-router v2 is live.

And by the way, I'm a little more upset than the fact that I find a 360kb script in the browser console on the NETWORK tab. My first thought was this:
An empty page from expo-router already occupies 360 kb, whereas in my full-fledged projects on react, my bundle size is 170 kb ... at first I was sad.

<img alt="expo sdk" height="128" src="./assets/images/git/Scr1.png">

My initial disappointment turned into intrigue. Blocking scripts and refreshing the console reduced the page size to 6KB. This newfound efficiency bolsters my enthusiasm for expo-router v2.

<img alt="expo sdk" height="128" src="./assets/images/git/Scr.png">

In this iteration, we haven't added the meta tags and other SEO essentials yet, but we'll address those in the future. Currently, three HTML pages exist: two in the "Tab" navigator and one in a modal window.

<h3 align="left">Problem 3: EXPO-ROUTER v2</h3>
However, after export from Expo, the Expo/Vector-Icons don't appear in the app. The only way to access the MODAL page is to hardcode "/modal" in the address bar.

We'll tackle this issue in the next step.

Although this problem has been discussed online for some time, Expo developers haven't yet provided a definitive solution. It's hoped that when you engage with this content, the issue will be resolved. Regardless, this challenge isn't all negative. Working with SVG images instead of Expo-vector-icons allows us to expand our app's potential.

Congratulations, you've created your first React-Native static site, or more precisely, React-Native. More details about the site's structure will be covered in a dedicated video for this step.

## 🗺 Project Layout

- [`packages`](/packages) All the source code for Expo modules, if you want to edit a library or just see how it works this is where you'll find it.
- [`apps`](/apps) This is where you can find Expo projects which are linked to the development modules. You'll do most of your testing in here.
- [`docs`](/docs) The source code for **https://docs.expo.dev**
- [`templates`](/templates) The template projects you get when you run `npx create-expo-app`
- [`react-native-lab`](/react-native-lab) This is our fork of `react-native` used to build Expo Go.
- [`guides`](/guides) In-depth tutorials for advanced topics like contributing to the client.
- [`android`](/android) contains the Android project.
- [`home`](/home) contains the JavaScript source code of the app.
- [`ios`](/ios) contains the iOS project.
- [`ios/Exponent.xcworkspace`](/ios) is the Xcode workspace. Always open this instead of `Exponent.xcodeproj` because the workspace also loads the CocoaPods dependencies.
- [`tools`](/tools) contains build and configuration tools.
- [`template-files`](/template-files) contains templates for files that require private keys. They are populated using the keys in `template-files/keys.json`.
- [`template-files/ios/dependencies.json`](/template-files/ios/dependencies.json) specifies the CocoaPods dependencies of the app.

## 💙 Author

Roman Bolshiyanov < status : open for cooperation, look job >

## License

The Expo source code is made available under the [MIT license](LICENSE). Some of the dependencies are licensed differently, with the BSD license, for example.


<img alt="Star the Expo repo on GitHub to support the project" src="https://user-images.githubusercontent.com/9664363/185428788-d762fd5d-97b3-4f59-8db7-f72405be9677.gif" width="50%">
