# Redux Discussion Question

1. Run `npm install`
2. Run `npm start`
3. Review the files in this repository
4. Use the `useSubscription` hook in `DisneyStockChart.js` to subscribe to the stock data for DIS: 
> `useSubscription` Example Usage:
```javascript
   useSubscription(`http://localhost:5001/stock-data`, newPrice => {
      // Your Code Here
   })
```
5. Send the stock data from the subscription to the redux store and save the data in state.
6. Ensure that this works using the redux devtools
7. Over time, are more and more duplicate values being added to state? Make sure your `useSubscription` hook is only called **once**, when the component mounts...
8. Use `useSelector` to get the stock data from the redux state
9. Feed the data from the redux state into the `Line` to create a realtime graph of disney stock prices
