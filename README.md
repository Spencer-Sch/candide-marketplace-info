# <img align="left" alt="Candide" width="36px" src="./assets/logo.png" />Candide Marketplace

We're building an NFT rental marketplace for P2E games 🕹️

#### The marketplace is now in beta testing! 🚀

#### <a href="https://marketplace.candide.site/">marketplace.candide.site</a> ⚠️ site under active development ⚠️

<br>

## Table of Contents

<details open>
<summary></summary>

- [About Candide](#about-candide)
- [The Front-end](#the-front-end)
  - [Technologies Used](#technologies-used)
  - [My Role](#my-role)
- [Features](#features-alpha-version)
  - [NFT Card & Details Page](#nft-card--details-page)
  - [Dynamic Popover Screen Containment](#dynamic-popover-screen-containment)
  - [NFT Sorting and Filtering](#nft-sorting-and-filtering)

</details>

<br>

## About Candide

### We are a small, international, team that is passionate about providing value to p2e players.

The Candide marketplace will allow users to rent p2e NFTs for their favorite NFT games.

- When renting an NFT you gain access to its utility without risking your capital
- When lending an NFT you put it to work generating passive income
  <br>

### Come Say Hello 👋

[<img align="left" alt="Candide | Discord" width="35px" src="https://s3-storage.textopus.nl/wp-content/uploads/2015/05/18050104/Discord-icon-270x270.png" />][discord]
[<img align="left" alt="Candide | LinkedIn" width="35px" src="https://algomine.pl/wp-content/uploads/LinkedIn-Icon-380x380.png" />][linkedin]
[<img align="left" alt="Candide | Twitter" width="35px" src="https://www.seekpng.com/png/full/5-54303_twitter-introduces-a-new-app-for-windows-twitter.png" />][twitter]
[<img align="left" alt="Candide | Instagram" width="35px" src="https://upload.wikimedia.org/wikipedia/commons/a/a5/Instagram_icon.png" />][instagram]

<br>
<br>

## The Front-end

<!-- #### 🚨 The following images demonstrate features & functionality I built for the site. These demos are populated with static data and assets used in development and do not accurately represent the current state of the project. 🚨 -->

### Technologies Used:

- Nuxt/Vue 2
- Tailwind.css
- Assorted utility libraries (date-fns, js-cookie, fontawesome, etc.)
- **No front-end component libraries**

### My Role

I fill the role of sole designer & front-end engineer. I built the UI and all of the components from scratch using Tailwind.css.

<!-- <a href="https://marketplace.candide.site/" target="_blank">
<img src="./assets/candide-marketplace.png" alt="candide landing page screen shot" width="500px" />
</a> -->

## Features (alpha version)

#### 🚨 The following images demonstrate features & functionality I built for the site. These demos are populated with static data and assets used in development and do not accurately represent the current state of the project. 🚨

### NFT Card & Details Page

All the components are dynamic and reusable. Each axie's stats and traits in the popover and on the details page are dynamically selected and styled based on the data passed into the components.

<img src="./assets/axie-display.gif" />
<br>

### Dynamic Popover Screen Containment

1. The popover is "staged" for display when the mouse enters the
   border of the card component. - `display: none;` is swapted for `display: flex;` & `opacity: 0;`

2. At this point `getBoundingClientRect()` is used to get the appropriate coordinates of the popover and the containing window.

3. If the coordinates of the popover excede the limit of the window then the position of the popover is altered to be within the appropriate boundaries.

4. The "i" icon is hovered and the popover transitions into view using `opacity` and `scale`

5. Reverse steps for fade-out and "unstaging" of the popover.

<img src="./assets/containment.gif" width="600px" />
<br>

### NFT Sorting and Filtering

<img src="./assets/axie-filters.gif" />

[twitter]: https://twitter.com/CandideNft
[instagram]: https://www.instagram.com/candidenft/
[linkedin]: https://www.linkedin.com/company/candidenft/
[discord]: https://discord.com/channels/1000021187600076810/1000021854058205224
