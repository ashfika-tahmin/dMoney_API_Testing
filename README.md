# dMoney API Testing

## What is dMoney?

dMoney is a digital financial service API for common wallet operations.  
It supports user accounts and transactions such as deposits, money transfers, withdrawals, and payments.

## Technologies used

- **Postman Collection** - defines the API requests, test data, and assertions in `collection/assignment_on_API_testing.postman_collection.json`.
- **Newman** - runs the Postman collection from the command line.
- **newman-reporter-htmlextra** - generates a detailed HTML test report.
- **Node.js and npm** - provide the runtime and manage the project dependencies.

## How to run

1. Make sure Node.js and npm are installed.
2. Start the dMoney API server. The collection's default `baseUrl` is `http://localhost:5000`; update it in the collection if your server uses a different URL.
3. From the project root, install the dependencies:

   ```powershell
   npm install
   ```

4. Run the collection and generate the HTML report:

   ```powershell
   node report.js
   ```

5. Open `Reports/report.html` in a browser to view the results.

To run the collection directly with Newman without generating the HTML Extra report:

```powershell
npx newman run .\collection\assignment_on_API_testing.postman_collection.json
```


## Documentation
https://documenter.getpostman.com/view/59433845/2sBYHYuJ16
