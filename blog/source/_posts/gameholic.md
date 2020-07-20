---
title: GameHolic
subtitle: <b> ( Web Development / HTML / CSS )</b>
date: 2019-12-02 12:04:44
tags: portfolio
cover_index: /assets/gindex.jpg
cover_detail: /assets/game.png
---

`Web Development` `HTML/CSS`  `React` `UI/UX Design` 

The website can be viewed here: [**GameHolic**](https://game-holic-590ee.firebaseapp.com/ "run the application"). And the github repository can be accessed [here](https://github.com/RuoyanMeng/Game-Holic "link to github ").

> ### ContentS
> [Background](#background) 
> [Framework and API](#framework-and-api) 
> [Design and Development](#design-and-development)
> [Conclusion](#conclusion)

<span id = "background"></span>

## Background
GameHolic is a web application where users can search for trendy games and view detailed information of games. I did this project with another 2 students during the course Interaction Programming and the Dynamic Web (KTH University, Sweden, 2019). The goal of this project is to practice web development.

<span id = "framework-and-api"></span>

## Technology Stack
- **Framework** 
 React, Redux
- **API** 
 [IGDB API](https://www.giantbomb.com/api/)
- **Library**
 [Ant Design of React](https://ant.design/ " "), [react-beautiful-dnd](https://github.com/atlassian/react-beautiful-dnd  " "), Tachyons

<span id = "design-and-development"></span>

## Design and Development
In this project, each member of the team was responsible for different components: the main architecture and most of the function codes were done by one of our team member Ruoyan, then I and the other member Kehan were mainly responsible for the layouts and styles part, as well as some other interaction parts. 

I was responsible for the layouts, styles, and basic interaction codes of the following components: Header.js / Main.js / Search.js / SingleGame.js / gameDetails.js / GameGrid.js, as well as gamegrid.scss / header.scss / main.scss / search.scss / singlegame.scss. This website mainly used the Ant Design Components, and the followings are the main design and development work done by me:

-   **Homepage**
    The homepage is consisted of 4 components: header (logo/sign in, sign out button), search, banner and game grid.
    <img src="hp.png" width="49%"/> <img src="hp2.png" width="49%"/> 
    The main color of the website is black since we want it to be simple and cool. The big background picture of Batman was designed to catch user's eye when they open the website. Then the game grid was designed to recommend trendy games (here sorted by popularity) to users.

    The webpages were responsive by using the 24 Grids System of Ant Design:
        <Row>
            <Col xs={24} sm={24} md={20} lg={16} xxl={12}>
              <div className="banner-info">
                <h1>Here, plenty of trendy games for you!</h1>
                <h2>
                  Start discovering fancy games and getting your own
                  collections now! You could find everything you need!
                </h2>
              </div>
            </Col>
        </Row>

-   **Game Detail Page**
    In the game detail page, users can check the cover image and introduction of the game. There is also a circle bar to show the recommendation level of the game. The button under the texts is used to add the game to different lists of users account, e.g. wish list. 
    <img src="gd.png" width="49%"/> <img src="gd3.png" width="49%"/> 
    Below this, there is some other information of the game: keywords, screenshots and comments. The keywords can also be clicked and then will lead users to the search results page showing games that share the same keywords. I added the screenshots part since it can help users better know the game, and luckily I can fetch images with high quality through the API. I also added comments part to provide more information and interactions for users. 
    <img src="gd1.png" width="49%"/> <img src="gd2.png" width="49%"/> 

-   **Search Page**
    The search results show the cover image, name and summary of the game, and users would be guided to game detail page by clicking the items.
    <img src="se.png" width="70%"/></br>

-   **Wish List**
    In this part, users are supported to drag and drop items in personal lists to move or reorder them, as well as delete the item from the list directly by hovering the mouse over it. Here I implemented the drag and drop effect by using react-beautiful-dnd. 
    <img src="wl.png" width="70%"/></br>

<span id = "conclusion"></span>

## Conclusion
By doing this project, I got to know and practice web development, and I got a good chance to understand the knowledge and application of React/HTML/CSS.



--- 