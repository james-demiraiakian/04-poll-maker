# Poll Maker App

## Data Model

- Poll Object

```js
poll = {
  topic: "topic",
  a: "Option A",
  aVotes: int,
  b: "Option B",
  bVotes: int,
};
```

Polls Array

```js
polls = [
  {
    topic: "topic 1",
    a: "Option A",
    aVotes: int,
    b: "Option B",
    bVotes: int,
  },
  {
    topic: "topic 2",
    a: "Option A",
    aVotes: int,
    b: "Option B",
    bVotes: int,
  },
  {
    topic: "topic 3",
    a: "Option A",
    aVotes: int,
    b: "Option B",
    bVotes: int,
  },
];
```

## State

- Question/Topic "String"
- Option A "String"
- Option B "String"
- Current Poll {Object}
- Votes for A "Int"
- Votes for B "Int"
- Previous Polls + Results [Array of {Objects}]
- Show/Hide Poll Form
- Show/Hide Poll Tracker

## Events

- Button: New Poll
  - New page to input poll data
- Input: Question
- Input: Option A
- Input: Option B
- Button: Start Poll
- Button: Vote A
- Button: Vote B
- Button: Remove vote for A
- Button: Remove vote for B
- Button: Close Poll

## Components

- Poll Input
  - Button: New Poll
    - Create new poll object
  - Input: Question
  - Input: Option A
  - Input: Option B
  - Button: Start Poll
    - Update Poll Object
- Poll Tracker
  - Button: Vote A
    - aVotes++
  - Button: Vote B
    - bVotes++
  - Button: Remove vote for A
    - aVotes--
  - Button: Remove vote for B
    - bVotes--
- Poll End
  - Store Poll Object in Polls Array
  - Reset Current Poll
