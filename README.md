# R3F-Performance

**[Changelog](https://github.com/anhldh/r3f-performace/blob/main/CHANGELOG.md)**

A lightweight and easy-to-use tool to monitor the performance of your @react-three/fiber application.

<table>
  <tr>
    <td>Add the <code>&lt;PerformanceMonitor /&gt;</code> component anywhere in your R3F Canvas.</td>
    <td>
      <a href="https://wtp9t.csb.app/">
        <img src="https://bf3xu0otcy.ufs.sh/f/lSBP1EY5xRSnLHNlxKuvoRAdugXS39mBlIzpHEcwjKqeLFNJ" alt="R3F Performance Monitor" />
      </a>
    </td>
  </tr>
</table>

## Installation

```bash
# npm
npm install r3f-perf

# yarn
yarn add r3f-perf

# pnpm
pnpm add r3f-perf
```

## Options

```jsx
logsPerSecond?: 10, // Refresh rate of the logs

antialias?: true, // Take a bit more performances but render the text with antialiasing

overClock?: false, // Disable the limitation of the monitor refresh rate for the fps

deepAnalyze?: false, // More detailed informations about gl programs

showGraph?: Toggles the visibility of the performance graphs. Default true

graphType?: Style of the graph. Options: 'line' or 'bar'.

minimal?: false // condensed version with the most important informations (gpu/memory/fps/memory/vram)

matrixUpdate?: false // count the number of time matrixWorldUpdate is called per frame

chart?: {
  hz: 60, // graphs refresh frequency parameter
  length: 120, // number of values shown on the monitor
}

className?: '' // override CSS class

style?: {} // override style

position?: Sets the position of the panel. Options: 'top-right', 'top-left', 'bottom-right', 'bottom-left'.

```

## Usage

```jsx
import { Canvas } from "@react-three/fiber";
import { PerformanceMonitor } from "r3f-performance";

function App() {
  return (
    <Canvas>
      <PerformanceMonitor />
    </Canvas>
  );
}
```

### Maintainers :

- [`@anhldh`](https://github.com/anhldh/r3f-performance)

### Thanks

Special thanks to [`twitter @utsuboco`](https://twitter.com/utsuboco). This library is a port/fork based on the original r3f-perf.
