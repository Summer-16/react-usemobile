# react-usemobile

This is a simple hook will help you detect the device view and orientation.

[Find NPM Package here](https://www.npmjs.com/package/react-usemobile)

## Installation

To install, you can use npm or yarn:

```
npm i react-usemobile --save
or
yarn add react-usemobile
```

## Usage

Example:

```javascript
import useMobile from "react-usemobile";
```


```javascript
import useMobile from "react-usemobile";

function App() {
  const isMobile = useMobile();

  return (
    <>
      {isMobile.mobile ? (
        <p>This is Mobile Device</p>
      ) : isMobile.tablet ? (
        <p>This is Tablet Device</p>
      ) : (
        <p>This is Desktop/Laptop Device</p>
      )}
      <p>
        Current Orientation:{" "}
        {isMobile.landscape
          ? "Landscape"
          : isMobile.portrait
          ? "Portrait"
          : "Unknown"}
      </p>
    </>
  );
}

export default App;
```
