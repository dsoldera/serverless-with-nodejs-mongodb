# USING NODEJS AND SERVERLESS

- tutorial: https://dev.to/bnevilleoneill/going-serverless-with-your-node-js-apps-3f8i

## Installing serverless tool

```
npm install serverless -g
```

> Should be installed in every node version

## Definitions

```
const handlerFunction = (event, context, callback) => {
    callback(error, result)
}
module.exports = handlerFunction;
```

Let’s review how the above serverless function is executed. The **handleFunction** const is the name of our serverless function.

The **event** object, which is one of our function arguments, represents the information about the kind of event that would trigger our function and cause it to start executing a piece of our code.

The **context** object contains information about the environment our function is to be executed on (note that this is usually handled by cloud providers on our behalf).

Lastly, the **callback** function takes care of returning a response or an error object, usually based on the request made by user events.
