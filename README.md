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
  React Native, TypeScript, Redux, React Query & more.
</p>

---

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

## Building the app

#### Android
_Prerequisite : Make sure you have the keystore required for signing the Android builds_
1. Open Android Studio
2. Open the `android` folder from our project in Android Studio
3. Click on Project on the menu bar -> `Clean Project`. Wait for this process to complete.
4. Click on Project on the menu bar again -> `Generate Signed Bundle / Apk...`
5. Select Android App Bundle. Click on next.
6. Point the Key store path to the download keystore and fill the other fields. Reach out to the team to enquire about the password and alias. Click on next.
7. Check the Destination Folder. Select the build variant and click on Finish.
8. Once the process is complete, the `aab` will be generated.

### iOS
_Prerequisite : Make sure you have the certificates required for building iOS dev and production builds. Reach out to [Joy Patel](https://github.com/joy-betterhalf) for the same_
1. Open XCode.
2. Open `betterhalf` project so that it shows in the main content panel on the right.
3. Click on Product on the menu bar -> `Clean Build Folder`. Wait for this process to complete.
4. Click on Product on the menu bar again -> `Archive`. Wait for this process to complete.
5. Once the Build succeeds, the Archives window automatically opens up. Select your archive and click on `Distribute App`.
6. Select `Development` and click on Next. Click on Next again in the following window.
7. In the `betterhalf.app` input, select the relevant Development profile. Click on Next.
8. Once the process is complete, the `ipa` will be generated.

## Important Links
[Front-end Engineering - Design, Architecture & Best Practices](https://betterhalf-product.atlassian.net/wiki/spaces/P/pages/1624178699/Front-end+Engineering+-+Design+Architecture+Best+Practices)

## FAQ :

### 1. Why are we running npx pod-install instead of (`cd ios && pod install`) ?

[You can read in detail here](https://github.com/expo/expo-cli/tree/main/packages/pod-install#-why). But the gist is : `npx pod-install` performs any additional
checks in case pod installation errors out and tries to resolve it, which is not done by `pod install`.

### 2. What is the right way to clean the project if I see any errors while building the app ?
Based on what error you're facing and the platform, you can try one of the clean commands [listed here](https://github.com/pmadruga/react-native-clean-project#content).
