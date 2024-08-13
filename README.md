# Website Template


## Dev URL's
Main Branch - 
Develop Branch - 

## How to Install and Run the Project
1. Clone this repo. Navigate to the directory where you'd like to put the VA-CCPI directory and run:
    ```bash
    git clone https://github.com/blackberggroup/VA-CCPI.git
    ```
    
    This will create a directory with the website files inside. Navigate to this new directory:
    ```bash
    cd VA-CCPI
    ```

1. Install Node.js `16.16.0` or higher =>
    * Check your node version if it is already installed `node -v`
    * [Download](https://nodejs.org/en/).    

1. Install the project dependencies:
    ```bash
    npm install
    ```
    
1. Start the local server. You'll find the home page located at: `http://localhost:8080/`
    ```bash
    npm start
    ```

1. Run gulp to watch any changes you make to `scss` files:
    ```bash
    gulp watch

## In case of concurrent legacy and new web pages
1. So that we don't overwrite the legacy "assets" directory, we will need to name the new "assets" directory "assets-3-5".

1. Make a copy of the existing "assets" directory and rename it "assets-3-5"

1. Change all paths in your code to point to "assets-3-5"

1. When developing, you will need to remember to add any new images or documents to BOTH directories

1. When changing `scss` files, you will need to manually copy the newly compiled styles.css into "assets-3-5" to see changes.

1. Be sure to update the deploy script to include "assets-3-5" and exclude "assets" from _site