<br/>
<br/>
<br/>

<p align="center">
    <img alt="betterhalf-logo" src="https://pbs.twimg.com/profile_images/1505780427444809728/y2OthVqA_400x400.jpg" width="200" />
</p>
<br/>
<p align="center">Official Betterhalf Mobile Application Repo</p>
<br/>
<br/>

<div align="center">
<a href='https://play.google.com/store/apps/details?id=com.betterhalf&hl=en_IN&gl=US&pcampaignid=pcampaignidMKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1'>
  <img alt='Get it on Google Play' width="300" src='https://user-images.githubusercontent.com/49429259/175395897-0eed7bfc-34fc-48d6-a859-9d10f7f050f0.png' style="border-radius: 13px; border: 10px solid white;"/>
</a>
&nbsp; &nbsp;
<a href="https://apps.apple.com/us/app/betterhalf-ai-matrimony-app/id1438203766?itsct=apps_box_badge&amp;itscg=30200">
  <img src="https://miro.medium.com/max/600/1*xqT83bMEz92IBYxS9UQNow.png" alt="Download on the App Store" style="border-radius: 13px">
</a>
  </div>
 
  <br />

<p align="center">
Built With ❤️ :
  React Native, TypeScript, Redux, React Query
</p>

___

## Installation

1. Clone the repo :

```
git clone https://github.com/betterhalf-ai/betterhalf-mobile-rn.git
```

2. Install packages : _(We use the Yarn package manager in our project. Do NOT use npm)_

```
yarn
```

3. Install pods for iOS : _(No special steps required for Android)_
```
npx pod-install
```

## Run the app on Device or Simulator

#### iOS :
```
yarn ios
```

#### Android :
```
yarn android
```

Running either of these commands automatically starts the Metro bundler and then starts building the app.
If you want to run the Metro bundler instance separately and then build the app, you can :

Start the Metro bundler :
```
yarn start 
```
Then run the app in Android `yarn android` or iOS `yarn ios`

## FAQ :

### Why are we running npx pod-install instead of (cd ios && pod install) ?
[You can read in detail here](https://github.com/expo/expo-cli/tree/main/packages/pod-install#-why). But the gist is : `npx pod-install` performs any additional
checks in case pod installation errors out and tries to resolve it, which is not done by `pod install`.

