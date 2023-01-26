# react-usemobile

This is a simple hook which help you detect the device view and orientation.

## react-usemobile

This is a simple hook will help you detect the device view and orientation.

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

If you want to leave a message to a specific browser (e.g IE), you can use `isIE` selector

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
