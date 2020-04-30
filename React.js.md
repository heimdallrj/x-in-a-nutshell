# React in a nutshell.

**Table of contents**
- [Thinking in React](#thinking-in-react)
  * [Concepts and Keywords](#concepts-and-keywords)
    + [Component](#concepts-and-keywords)
      - [Stateless Components](#concepts-and-keywords)
      - [Stateful Components](#concepts-and-keywords)
      - [Higher-Order Components](#concepts-and-keywords)
    + [State vs Props](#concepts-and-keywords)
    + [JSX](#concepts-and-keywords)
- [API Reference](#api-reference)
  * [React Top-Level API](#react-top-level-api)
  * [ReactDOM](#reactdom)
  * [ReactDOMServer](#reactdomserver)
  * [DOM Elements](#dom-elements)
  * [SyntheticEvent](#syntheticevent)
  * [Test Utilities](#test-utilities)
  * [Test Renderer](#test-renderer)
  * [JavaScript Environment Requirements](#javascript-environment-requirements)
- [Coding in React](#coding-in-react)
  * [Hello World!](#hello-world-)
    + [Pure Function](#pure-function)
    + [Class Component](#class-component)
  * [Sample Application Structure](#sample-application-structure)
- [Type Checking](#type-checking)
- [Web Components](#web-components)
- [Accessibility](#accessibility)
- [Performance optimization](#performance-optimization)
- [React Profiler](#react-profiler)
- [Redux](#redux)
  * [Redux Middlewares](#redux-middlewares)
    + [Saga](#saga)

## [Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

### Concepts and Keywords

**Component**

> Basic building blocks of React Application are Components.

![](https://github.com/thinkholic/x-101/raw/master/assets/1.jpg)

A **Component** consists of;
- HTML Markup
- Props
- State
- Life-cycle

There are **Two Types** of React Components;
- Stateless
- Stateful (Class Component)

![](https://github.com/thinkholic/x-101/raw/master/assets/2.jpg)

***Stateless Components***

```text
*Pure Function* React Component.

Returns *HTML* Markup.

No *Advanced Component Logics* included.
```

***Stateful Components***

```text
JavaScript *Class*

Includes;
- Local State
- Life-cycle methods
- Advanced Component Logics
```

***Higher-Order Components***

```js
const higherOrderComponent = (Component) => {
  const newProps = {};
  return (<Component {...newProps} />)
}

const EnhancedComponent = higherOrderComponent(WrappedComponent);
```

**State vs Props**

![](https://github.com/thinkholic/x-101/raw/master/assets/3.jpg)

**JSX**

```text
Stands for *JavaScript XML*.

Allows to write *HTML* in React.js
```

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
## API Reference

### React Top-Level API
- *Components*
  - React.Component
    - Lifecycle 
      - *Mounting*
        - constructor(props)
        - static getDerivedStateFromProps(props, state)
        - render()
        - componentDidMount()
      - *Updating*
        - static getDerivedStateFromProps(props, state)
        - shouldComponentUpdate(nextProps, nextState)
        - render()
        - getSnapshotBeforeUpdate(prevProps, prevState)
        - componentDidUpdate(prevProps, prevState, snapshot)
      - *Unmounting*
        - componentWillUnmount()
      - *Error Handling*
        - static getDerivedStateFromError(error)
        - componentDidCatch(error, info)
    - Other
      - setState(updater, [callback])
      - component.forceUpdate(callback)
    - Class Properties
      - defaultProps
      - displayName
    - Instance Properties
      - props
      - states
    - Error Handling**
      - static getDerivedStateFromError(error)
      - componentDidCatch(error, info)      
  - React.PureComponent
  - React.memo
- *Creating React Elements*
  - React.createElement(type, [props], [...children])
  - React.createFactory(type)
- *Transforming Elements*
  - React.cloneElement(element, [props], [...children])
  - React.isValidElement(object)
  - React.Children
    - React.Children.map(children, function[(thisArg)])
    - React.Children.forEach(children, function[(thisArg)])
    - React.Children.count(children)
    - React.Children.only(children)
    - React.Children.toArray(children)
- React.Fragment
- React.StrictMode
- *Refs*
  - React.createRef
  - React.forwardRef
- *Suspense*
  - React.lazy
  - React.Suspense
- Hooks
  - Basic Hooks
    - useState(initialState)
    - useEffect(didUpdate)
    - useContext(MyContext)
  - Additional Hooks
    - useReducer(reducer, initialArg, init)
    - useCallback(() => {},[args])
    - useMemo(() => (), [a, b])
    - useRef(initialValue)
    - useImperativeHandle(ref, createHandle, [deps])
    - useLayoutEffect
    - useDebugValue(value)
- Context
  - React.createContext(defaultValue)
  - Context.Provider
  - Class.contextType
  - Context.Consumer
  - Context.displayName
    
### ReactDOM
- ReactDOM.render(element, container[, callback])
- ReactDOM.hydrate(element, container[, callback])
- ReactDOM.unmountComponentAtNode(container)
- ReactDOM.findDOMNode(component)
- ReactDOM.createPortal(child, container)

### ReactDOMServer
- ReactDOMServer.renderToString(element)
- ReactDOMServer.renderToStaticMarkup(element)
- ReactDOMServer.renderToNodeStream(element)
- ReactDOMServer.renderToStaticNodeStream(element)

### DOM Elements
- *Differences In Attributes*
  - checked
  - className
  - dangerouslySetInnerHTML
  - htmlFor
  - onChange
  - selected
  - style
  - suppressContentEditableWarning
  - suppressHydrationWarning
  - value

### SyntheticEvent
- *Clipboard Events*
  - onCopy
  - onCut
  - onPaste
- *Composition Events*
  - onCompositionEnd
  - onCompositionStart
  - onCompositionUpdate
- *Keyboard Events*
  - onKeyDown onKeyPress onKeyUp
- *Focus Events*
  - onFocus onBlur
- *Form Events*
  - onChange onInput onInvalid onReset onSubmit
- *Generic Events*
  - onError onLoad
- *Mouse Events*
  - onClick onContextMenu onDoubleClick onDrag onDragEnd onDragEnter onDragExit
onDragLeave onDragOver onDragStart onDrop onMouseDown onMouseEnter onMouseLeave
onMouseMove onMouseOut onMouseOver onMouseUp
- *Pointer Events*
  - onPointerDown onPointerMove onPointerUp onPointerCancel onGotPointerCapture
onLostPointerCapture onPointerEnter onPointerLeave onPointerOver onPointerOut
- *Selection Events*
  - onSelect
- *Touch Events*
  - onTouchCancel onTouchEnd onTouchMove onTouchStart
- *UI Events*
  - onScroll
- *Wheel Events*
  - onWheel
- *Media Events*
  - onAbort onCanPlay onCanPlayThrough onDurationChange onEmptied onEncrypted
onEnded onError onLoadedData onLoadedMetadata onLoadStart onPause onPlay
onPlaying onProgress onRateChange onSeeked onSeeking onStalled onSuspend
onTimeUpdate onVolumeChange onWaiting
- *Image Events*
  - onLoad onError
- *Animation Events*
  - onAnimationStart onAnimationEnd onAnimationIteration
- *Transition Events*
  - onTransitionEnd
- *Other*
  - onToggle

### Test Utilities
- act()
- mockComponent()
- isElement()
- isElementOfType()
- isDOMComponent()
- isCompositeComponent()
- isCompositeComponentWithType()
- findAllInRenderedTree()
- scryRenderedDOMComponentsWithClass()
- findRenderedDOMComponentWithClass()
- scryRenderedDOMComponentsWithTag()
- findRenderedDOMComponentWithTag()
- scryRenderedComponentsWithType()
- findRenderedComponentWithType()
- renderIntoDocument()
- *Simulate.{eventName}(element, [eventData])*

### Test Renderer
- TestRenderer.create(element, options)
- TestRenderer.act(callback)
- testRenderer.toJSON()
- testRenderer.toTree()
- testRenderer.update(element)
- testRenderer.unmount()
- testRenderer.getInstance()
- testRenderer.root
- testInstance.find()
- testInstance.findByType(type)
- testInstance.findByProps(props)
- testInstance.findAll(test)
- testInstance.findAllByType(type)
- testInstance.findAllByProps(props)
- testInstance.instance
- testInstance.type
- testInstance.props
- testInstance.parent
- testInstance.children

### JavaScript Environment Requirements
- imports;
  - `core-js/es/map`
  - `core-js/es/set`
  - `raf/polyfill`

## Coding in React

### Hello World! 

**Usage**
```js
<HelloWorld name="John Doe" />
```

#### Pure Function
```js
const HelloWorld = ({ name }) => (
  <div>
    Hello, {name}!
  </div>
);
```

#### Class Component
```js
class HelloWorld extends React.Component {
  displayName = "Hello World Component";
  
  // state = {}; // Alternative way to set initial states
  
  constructor(props) {
    // Mounting
    
    super(props);
    this.state = {}
  }
  
  static getDerivedStateFromProps(props, state) {
    // Mounting, Updating
  }

  componentDidMount() { // Mounting }
  
  shouldComponentUpdate(nextProps, nextState) { // Updating }
  
  getSnapshotBeforeUpdate(prevProps, prevState) { // Updating }
  
  componentDidUpdate(prevProps, prevState, snapshot) { // Updating }

  componentWillUnmount() { // Unmounting }
  
  static getDerivedStateFromError(error) { // Error Handling }
  
  componentDidCatch(error, info) { // Error Handling }

  render() {
    return (
      <div>
        Hello, {this.props.name}!
      </div>
    );
  }
}

HelloWorld.defaultProps = {
  name: 'Stranger'
};
```

### Sample Application Structure

**index.html**
```html
<html>
 ...
 <body>
  <div id="root"></div>
 </body>
<html>
```

**index.js**
```js
import React from "react";
import ReactDOM from "react-dom";
import App from "App.js"

ReactDOM.render(
  <App />,
  document.getElementById('root')
);
```

**App.js**
```js
import React from "react";

const App = () => (<>Component code goes here.</>);

export App;
```

## Type Checking
- Prop Types
- Flow
- TypeScript

## Web Components

## Accessibility

## Performance optimization

## React Profiler

## Redux
### Redux Middlewares
#### Saga
