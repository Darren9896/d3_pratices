# Building a simple tooltip
This folder contains the exercise files for chapter 7 section 7.3.2 of [D3.js in Action, 3rd edition](https://www.manning.com/books/d3js-in-action-third-edition).
</br>
In this folder, you’ll find a *start* and an *end* folder. To follow along with the book’s instructions, write your code in the *start* folder. If you ever get stuck, you’ll find the solution in the *end* folder.

## How to run the project
To run this project, you'll need a local webserver. We recommend using [VS Code](https://code.visualstudio.com/)'s Live Server extension. You can find instructions on installing this extension in Appendix A of the book.
1. Open the project folder (a *start* OR an *end* folder from the subsections mentioned above) in VS Code.
2. To run the project with the Live Server extension, click the *Go live* button in the status bar of VS Code.
3. The project should open automatically in your browser.

## Structure of the project
* The `/data` folder contains the CSV file `data.csv`, listing the sales revenue from different music formats between 1973 and 2019. The revenues are in million USD and adjusted for inflation (2017).
    * The music formats are `vinyl`, `8-track`, `cassette`, `cd`, `download`, and `streaming`.
    * The category `other` includes revenues from music videos (physical), synchronization, and royalties.
* The `/css` folder contains two CSS files:
     * `shared-constants.js` contains each chart's margins, width, and height, as per the strategy discussed in chapter 4. It also includes an array named `formatsInfo` that lists the id, label, and color associated with each format.
    * `scales.js` is where we initialized the D3 scales used to build the streamgraph.
    * `streamgraph.js` is where the streamgraph is already generated.
    * `interactions.js` is where you'll create the tooltip and handle the mouse events.
    * `load-data.js` is where the data is loaded and passed to the different functions that generate the visualizations.
* `index.html` contains the markup and text that composes the project. The D3 library, the CSS files, and the JavaScript files are already loaded in `index.html`.

Happy D3 coding! 🤓