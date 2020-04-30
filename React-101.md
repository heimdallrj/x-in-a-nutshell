# React 101

## Thinking in React

**Basic building blocks** of React Application are **Components**.

[Image 1]

A **Component** consists of;
- HTML Markup 
- Props
- State
- Constructor
- Life-cycle

There are **Two Types** of React Components;
- Stateless
- Stateful (Class Component)

[Image 2]

### Stateless Components
**Pure Function** React Component.

Returns **HTML** Markup.

No **Advanced Component Logics** included.

### Stateful Components
JavaScript **Class**

Includes;
- Local State
- Constructor
- Advanced Component Logics

### State vs Props

[Image 3]

### JSX
Stands for **JavaScript XML**.

Allows to write **HTML** in React.js

**JSX**
```js
const CompA = <h1>I Love JSX!</h1>;
ReactDOM.render(CompA, document.getElementById('root'));
```

**~JSX**
```js
const CompA = React.createElement('h1', {}, 'I do not use JSX!');
ReactDOM.render(CompA, document.getElementById('root'));
```

### React Life-cycle

**Mounting**
- constructor()
- getDerivedStateFromProps()
- render()
- componentDidMount()

**Updating**
- getDerivedStateFromProps()
- shouldComponentUpdate()
- render()
- getSnapshotBeforeUpdate()
- componentDidUpdate()

**Unmounting**
- componentWillUnmount()
