# live-voting
An application for organizing live votes. The idea is that we'll have a collection of things to vote from: Movies, songs, programming languages, quotes, anything. The app will put them against each other in pairs, so that on each round people can vote for their favorite of the pair. When there's just one thing left, that's the winner. Votes are displayed in real time.

## Goals
1. Make two separate UI's. One for mobile and one for web.
2. Make two apps, the browser app that'll handle user inferfaces and the server app to handle the voting logic.
3. Server app operation:
	-A client sends an action to the server.
	-The server hands the action to the Redux Store.
	-The Store calls the reducer and the reducer executes the logic related to the action.
	-The Store updates its state based on the return value of the reducer.
	-The Store executes the listener function subscribed by the server.
	-The server emits a 'state' event.
	-All connected clients - including the one that initiated the original action - receive the new state.
4. Use Redux to manage application code and Immutable JS to handle state. 

## Requirements

## Getting Started
From within the root directory:

```sh
npm install

```