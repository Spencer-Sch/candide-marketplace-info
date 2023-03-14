# <img align="left" alt="Candide" width="36px" src="./assets/logo.png" />Candide Marketplace

We're building an NFT rental marketplace for P2E games 🕹️

#### The marketplace is now in beta testing! 🚀

#### <a href="https://marketplace.candide.site/">marketplace.candide.site</a> 🛒
⚠️ site under active development ⚠️


## Table of Contents

<details open>
<summary></summary>

- [About Candide](#about-candide)
- [The Front-end](#the-front-end)
  - [Technologies Used](#technologies-used)
  - [My Role](#my-role)
  - [Media](#media)
- [Features](#features-alpha-version)
  - [NFT Card & Details Page](#nft-card--details-page)
  - [Dynamic Popover Screen Containment](#dynamic-popover-screen-containment)
  - [Sorting and Filtering](#sorting-and-filtering-tools)
  - [Form & Validation](#form-and-validation)

</details>
<br>

## About Candide

### We are a small, international, team that is passionate about providing value to p2e players.

The Candide marketplace will allow users to rent p2e NFTs for their favorite NFT games.

- When renting an NFT you gain access to its utility without risking your capital
- When lending an NFT you put it to work generating passive income
  <br>

#### Come Say Hello 👋

[<img align="left" alt="Candide | Discord" width="35px" src="https://s3-storage.textopus.nl/wp-content/uploads/2015/05/18050104/Discord-icon-270x270.png" />][discord]
[<img align="left" alt="Candide | LinkedIn" width="35px" src="https://camo.githubusercontent.com/9d66eeaa79b4f53e7ab2d6a0169bf220829f0bac4c21c57576a09371111a838d/68747470733a2f2f616c676f6d696e652e706c2f77702d636f6e74656e742f75706c6f6164732f4c696e6b6564496e2d49636f6e2d333830783338302e706e67" />][linkedin]
[<img align="left" alt="Candide | Twitter" width="35px" src="https://www.seekpng.com/png/full/5-54303_twitter-introduces-a-new-app-for-windows-twitter.png" />][twitter]
[<img align="left" alt="Candide | Instagram" width="35px" src="https://upload.wikimedia.org/wikipedia/commons/a/a5/Instagram_icon.png" />][instagram]

<br>
<br>
<br>

## The Front-end


### Technologies Used:

- Nuxt/Vue 2
- Tailwind
- Assorted utility libraries (date-fns, js-cookie, fontawesome, etc.)
- **No front-end component libraries**

### My Role

I fill the role of sole designer & front-end engineer. I built the UI and all of the components from scratch.

### Media

A video walkthrough of Candide's site and beta test process.
<br>

🟣 Note: the video is in french
<br>

<a href="https://www.youtube.com/watch?v=khgYVcq7hG8">
<img src="./assets/marketplace-review-thumbnail.png" width="500px" alt="candide marketplace beta test review" />
</a>

[Back to top](#candide-marketplace)

<br>

## Features (alpha version)

#### 🚨 The following images demonstrate features & functionality I built for the site. These demos are populated with static data and assets used in development and may not accurately represent the current state of the project. 🚨

### NFT Card & Details Page

- All the components are dynamic and reusable
- Each axie's stats, traits, and icons, in both the popover and on the details page, are dynamically selected and styled.

<img src="./assets/axie-display_150speed.gif" />

[Back to top](#candide-marketplace)

### Dynamic Popover Screen Containment

1. The popover is "staged" for display when the mouse enters the
   border of the card component i.e. `display: none` exchanged for `display: flex`

2. `getBoundingClientRect` is used to get the appropriate coordinates of the popover and the containing window

3. If the coordinates of the popover exceed the limit of the window then the position of the popover is adjusted to be within the appropriate boundaries

4. The `🛈` icon is hovered and the popover transitions into view using `opacity` and `scale`

5. Reverse steps for fade-out and "unstaging" of the popover

<img src="./assets/containment_speed150.gif" width="600px" />

[Back to top](#candide-marketplace)

### Sorting and Filtering Tools

- Custom select box components built from scratch along with filter chips which display all filters currently being applied
- Active filters are displayed both in the filter chip row and also as highlighted options within each select box
- When a filter is deleted (which can originate from four different user actions) All relevant components are updated to reflect the change

<img src="./assets/axie-filters_speed150.gif" />

[Back to top](#candide-marketplace)

### Form and Validation

- Custom from components and validation built from scratch
- Error messages prompt the user to enter valid information
- Form state prevents an incomplete form from being submitted.

<img src="./assets/form_val_150speed.gif" />

[Back to top](#candide-marketplace)

[twitter]: https://twitter.com/CandideNft
[instagram]: https://www.instagram.com/candidenft/
[linkedin]: https://www.linkedin.com/company/candidenft/
[discord]: https://discord.com/channels/1000021187600076810/1000021854058205224
