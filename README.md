# react-goodreads-shelf
![build](https://github.com/kylekarpack/react-goodreads-shelf/workflows/Node.js%20CI/badge.svg) ![CodeQL](https://github.com/kylekarpack/react-goodreads-shelf/workflows/CodeQL/badge.svg) [![Maintainability](https://api.codeclimate.com/v1/badges/468bb279800b728cb808/maintainability)](https://codeclimate.com/github/kylekarpack/react-goodreads-shelf/maintainability) [![Test Coverage](https://api.codeclimate.com/v1/badges/468bb279800b728cb808/test_coverage)](https://codeclimate.com/github/kylekarpack/react-goodreads-shelf/test_coverage)

This React component allows you to display a public Goodreads shelf in a React application. It's a lot like the Goodreads JavaScript widget, but allows for more customization, better async loading, and React-like usage.

![Example image](/sample/sample.png)

## Installation

```
npm install --save react-goodreads-shelf
```
or
```
yarn add react-goodreads-shelf
```

## Usage

```jsx
import React from "react";
import { GoodreadsBookshelf } from "react-goodreads-shelf";

export default function App() {
	return (
		<GoodreadsBookshelf userId="USER_ID_HERE" apiKey="API_KEY_HERE" />
	);
}
```

## Customization

You can also set some options as supported by the Goodreads API:

| Option | Type | Description | Default |
| ------ | ---- | ----------- | ------- |
| shelf  | string | The shelf from which to fetch books | read
| sort  | string | The order in which to sort the results returned | date_read
| limit  | number | The maximum number of books to be returned | 10
| width | number | Minimum width allowed for each book | 100
| details | boolean | Whether to show book details like book title, author, and summary | false

## Development
- `yarn start` to watch changes and build
- `yarn storybook` to launch storybook for testing

## ToDo

Short-term plans include adding additional API options and styling
