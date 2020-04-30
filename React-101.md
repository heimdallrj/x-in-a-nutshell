# React 101

> **Table of contents**
> - [Thinking in React](#thinking-in-react)
>   * [Stateless Components](#stateless-components)
>   * [Stateful Components](#stateful-components)
>   * [State vs Props](#state-vs-props)
>   * [JSX](#jsx)
>   * [React Life-cycle](#react-life-cycle)

## Thinking in React

**Basic building blocks** of React Application are **Components**.

![](https://github.com/thinkholic/x-101/raw/master/assets/1.jpg)

A **Component** consists of;
- HTML Markup 
- Props
- State
- Constructor
- Life-cycle

There are **Two Types** of React Components;
- Stateless
- Stateful (Class Component)

![](https://github.com/thinkholic/x-101/raw/master/assets/2.jpg)

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

![](https://github.com/thinkholic/x-101/raw/master/assets/3.jpg)

### JSX
Stands for **JavaScript XML**.

Allows to write **HTML** in React.js

```js
// JSX
const CompA = <h1>I Love JSX!</h1>;
ReactDOM.render(CompA, document.getElementById('root'));
```

```js
// ~ JSX
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
