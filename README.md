# DayTimeRange

TypeScript library for managing and comparing time ranges within a week.

## Installation

To install the dependencies, run:
```sh
npm install daytimerange

```
## Usage

### Importing

To use the library, import the necessary functions and classes.
```js 
import { TimeRange, twoTimeRangesOverlap } from './index';
```

### Creating a TimeRange

Create a `TimeRange` by specifying the day, start time, and end time.
```js 
const timeRange1 = new TimeRange('M', '09:00', '11:00');
const timeRange2 = new TimeRange('T', '10:00', '12:00');
```
### Checking Overlap

Check if two arrays of `TimeRange` objects overlap.
```js
const overlap = twoTimeRangesOverlap([timeRange1], [timeRange2]);
console.log(overlap); 
```

### Rendering a TimeRange

Render a `TimeRange` as a string.

```js
console.log(timeRange1.render()); // Output: "09:00->11:00"
```

## Development

### Building

To build the project, run the build command.
```sh
npm run build
```
### Linting

To lint the project, run the lint command.
```sh
npm run lint
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License
This project is licensed under the MIT License.