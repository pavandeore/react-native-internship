# React Native

## Resources
- https://reactjs.org/
- https://www.freecodecamp.org/news/learning-react-roadmap-from-scratch-to-advanced-bff7735531b6/
- https://github.com/MoonHighway/learning-react/tree/master/chapter-02
- https://facebook.github.io/react-native/

## Task 1
- Go to [gitlab.com](https://gitlab.com/) and create a repository named `internship-2019`
- Clone the project from git
- Create a new [react native CLI app](https://facebook.github.io/react-native/docs/getting-started)
- Push the new created project to git

## Task 2
- Create a new `TabNavigation` component and position it at the bottom of the screen
- Create and display the following screens when switching the tab: `Home`, `XO`, `Card`, `Account`

## Task 3
- This screen will be the `Home Tab`
- Take a look at the [Star Wars API](https://swapi.co/). We'll use it to get all kinds of data and display it in our app
- Fetch the `/people` data
- List the data according to the wireframe (TBD)

> Get data from the following endpoint `https://swapi.co/api/people/`

## Task 4
- Add an input on top of the list with an `Add` button
- Implement the add to list feature
- Add a new input below the first one and use it to add a search feature
- Add a `remove item` feature in-line of each entry in the list
- Optional: Instead of the button, implement a `swipe to remove item` feature 

## Task 5
- This screen will be the `XO Tab`
- Implement a 3x3 tic-tac-toe `Solo Play` game mode
- Optional: make `Computer play mode`

> Hint: for checking the winner, create an array with all winning position pairs

You can use this game state to get started:
```js
this.state = {
  gameType: 'player', // ENUM('player', 'computer')
  next: 'X',
  board: Array(9).fill(''), // Array with 9 empty string characters
  totalMoves: 0, // there can't be more than 9 moves. Useful for 'draw' result
  winner: null
};
```

## Task 6
- This screen will be the `Card Tab`
- Create a card flip memory game. [Example](https://www.webgamesonline.com/memory/)
- Make 4 rows with 4 cards on each row
- Add a `Reset` button
- Design is up to you

The `Card` component will have the following structure:
```json
{
    "id": 1,
    "image": "http://img.test",
    "show": true
}
```

- Use local images or use an open API to generate the image of the cards