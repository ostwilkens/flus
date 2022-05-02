# flus
Fluent styling API for React Components

![npm](https://img.shields.io/npm/v/flus)

```bash
npm install flus
```

```jsx
import { el } from 'flus'

const HStack = el("div").display("flex").flexDirection("row")

const Button = 
  el("button")
    .padding("2px 4px")
    .borderRadius("6px")
    .fontWeight("bold")

const PrimaryButton = 
  Button
    .color("white")
    .background("blue")

const SecondaryButton = 
  Button
    .color("black")
    .background("white")
    .border("1px solid blue")

// fancy call syntax
const ComponentB = () => 
  HStack.background("salmon")(
    PrimaryButton("Foo"), 
    SecondaryButton("Bar")
  )

// classic jsx
const ComponentA = () => 
  <HStack style={{ background: "salmon" }}>
    <PrimaryButton>Foo</PrimaryButton>
    <SecondaryButton>Foo</SecondaryButton>
  </HStack>
```

## todo
 - [x] proof of concept
 - [x] publish npm package
 - [x] code example
 - [ ] features
 - [ ] performance
