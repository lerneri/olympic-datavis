# 🏅 Inequality on the Podium

An interactive data visualization exploring how global inequality shapes Olympic performance.

## Overview

Olympic medals are often seen as symbols of national excellence, but they also reflect deeper structural inequalities. This project investigates how factors like wealth, development, and geopolitical dynamics influence success on the world stage.

Through interactive visualizations, we explore three key dimensions:

* Athlete migration between countries
* The relationship between performance and socioeconomic indicators
* The impact of hosting the Olympic Games

---

## Visualizations

### Moves Between Countries

This network graph traces athletes who changed national representation over time. It reveals how talent flows across borders—often from less wealthy nations to countries with stronger infrastructure and support systems, highlighting a global imbalance in opportunity.

---

### Performance vs Socioeconomic Factors

A scatter plot comparing Olympic performance with indicators such as GDP and Human Development Index. While wealthier countries tend to dominate, notable outliers challenge the pattern, showing that success is shaped by more than resources alone.

---

### Host Advantage Analysis

Heatmaps illustrate how countries perform when hosting the Olympics compared to other years. 

---

## Technologies Used

* **D3.js** — for custom interactive visualizations
* **Observable Runtime** — to embed and manage reactive notebooks
* **HTML / CSS / JavaScript** — for layout and styling

This project builds on data and visualizations from:

https://observablehq.com/d/28d23d1ad7224153

View this notebook in your browser by running a web server in this folder. For
example:

~~~sh
npx http-server
~~~

Or, use the [Observable Runtime](https://github.com/observablehq/runtime) to
import this module directly into your application. To npm install:

~~~sh
npm install @observablehq/runtime@5
npm install https://api.observablehq.com/d/28d23d1ad7224153@245.tgz?v=3
~~~

Then, import your notebook and the runtime as:

~~~js
import {Runtime, Inspector} from "@observablehq/runtime";
import define from "28d23d1ad7224153";
~~~

To log the value of the cell named “foo”:

~~~js
const runtime = new Runtime();
const main = runtime.module(define);
main.value("foo").then(value => console.log(value));
~~~

---

## License

This project is open-source and available under the MIT License.
