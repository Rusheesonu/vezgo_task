# vezgo_task

Language Used : Python 

Modules Used :

  Requests : For getting the data from web.
  Regex : Json - For data processing

Functions :
  
  bitquery_api_request(query, variables)
    
      - Bitquery provides a DB of real time crypto data.
      - We are querying their DB using an api to get the data 
      - api - "https://graphql.bitquery.io/"
      - This function takes 2 arguments as inputs query you want to execute and variables you want to pass with the query.
      - This function returns the queried output in the form of json block.
      

get_current_ether_price_in_usd():

      - This function gets the real time USD price of ETH.
      

getting_Account_balance(each_address, ether_price_usd):

      - This function takes any address as input and returns current balance of the account in ETH and USD.

getting_current_holdings(each_address):

      - This function takes any address as input and return all the holdings for that particular account.

get_transactions(each_address):

      - This function takes any address as input and returns latest 15 transactions for that particular account.

Command to run the script : 

      - python test.py ETH
      - Currenlt only configured to ETH walletss.

Sample output json block from the latest run:

{"address": "0x6e9d79ebbc9e75d656ff933e4a1850dd2283c58e", "balance": 609.47587384, "balance_USD": "$ 657037.7244", "positions": [{"symbol": "ETH", "tokenType": "", "name": "Ether", "value": 609.47587384}], "transactions": [{"from": "0xe319e5537a4b2eaba175cc5c0cb5e1b953bc83de", "to": "0x6e9d79ebbc9e75d656ff933e4a1850dd2283c58e", "value": "109282497560000000000", "timeStamp": "1614474363", "hash": "0xab4ff6179373275aa3da4417565b9c85fc7d1148975ba74ef4457a1515b75094"}, {"from": "0x3e5dd458a07a7ca37b48ab7e67bf5d371280d279", "to": "0x6e9d79ebbc9e75d656ff933e4a1850dd2283c58e", "value": "131258540630000000000", "timeStamp": "1614836981", "hash": "0xf52e6b937283f0efa620b47ce5874911def92193695d9094d4aebab89c4fa54a"}, {"from": "0x0ebcb7b353949edef5e302f1fb3a5aeb1813618c", "to": "0x6e9d79ebbc9e75d656ff933e4a1850dd2283c58e", "value": "125514874870000000000", "timeStamp": "1614863234", "hash": "0x12f7de58563fccb7b50ad0f8bdb6bbe398a1ad2a9625f4de419d05d68062da3a"}, {"from": "0xc4798efea6469d6afcdae160ec3fda2b24806231", "to": "0x6e9d79ebbc9e75d656ff933e4a1850dd2283c58e", "value": "243419960780000000000", "timeStamp": "1617938110", "hash": "0x2c520311c670fd22e3663a1e1e7efff37228358b8ca7cf7d136bee4b23bcc681"}]}


