# Poll Maker App

## State

- Question/Topic "String"
- Option A "String"
- Option B "String"
- Current Poll {Object}

```js
poll = {
  topic: "topic",
  a: "Option A",
  b: "Option B",
};
```

- Votes for A "Int"
- Votes for B "Int"
- Previous Polls + Results [Array of {Objects}]

```js
polls = [
  {
    topic: "topic 1",
    a: "Option A",
    b: "Option B",
  },
  {
    topic: "topic 2",
    a: "Option A",
    b: "Option B",
  },
  {
    topic: "topic 3",
    a: "Option A",
    b: "Option B",
  },
];
```

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
