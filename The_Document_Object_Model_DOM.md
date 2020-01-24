# The Document Object Model (DOM)

## What is the DOM?

The Document Object Model is a platform- and language-neutral interface that will allow programs and scripts to dynamically access and update the content, structure and style of documents. The document can be further processed and the results of that processing can be incorporated back into the presented page. Below is an image the represents the DOM generated for an HTML table in a web page.

![Example DOM Instance](./img/dom.gif)

The HTML you write is parsed by the browser and turned into the DOM. But your HTML is not the DOM. The DOM is a sequence of *parent* and *child* element objects. You can visualize and inspect the DOM using the [Developer Console](https://github.com/Kevin-CodeCrew/coding_concepts_sprint_1/blob/master/Debugging_and_the_Browser_Development_Console.md#inspecting-the-dom) in your browser.

## User Events and the DOM

Every object in the DOM generates events. Events are generated anytime you interact with an object in any way. This includes events such as mouse clicks, key presses, and the like. We can capture and handle the various events using JavaScript to provide a interactive experience.

We will cover JavaScript and event handlers in detail in another module.
