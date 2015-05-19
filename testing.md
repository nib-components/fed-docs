# Testing

## External Components

Check the `test/*.js` file. If it has `require('<component-name>')` use `component-test`. Otherwise test using `mocha` (because it's easier - usually for code which doesn't touch DOM).

### Component

Install the tools (if you haven't already):

    npm i -g component component-test

Build the tests:

(need to do this each time you change the code - not the tests though)

    component build --dev

Run the tests:

    component test browser

### Mocha

Install the tool:

    npm i -g mocha
    
Run the tests:

    mocha
