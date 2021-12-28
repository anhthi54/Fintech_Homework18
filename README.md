# Fintech_Homework18
### Setup the custom out-of-the-box blockchain

* Create accounts for two nodes andi1 & andi2 for the network with a separate `datadir` for each using `geth`.

* Run `puppeth`, name my netwrks as 'andid54', and select the option to configure a new genesis block.

* Choose the `Clique (Proof of Authority)` consensus algorithm.

* Paste both account addresses from the first step one at a time into the list of accounts to seal.

![](https://github.com/anhthi54/Fintech_Homework18/blob/7811daddf1b68dd7ca7eda06747fd7e8a36dc4b8/Screenshot/1.1.PNG)


* Paste them again in the list of accounts to pre-fund. There are no block rewards in PoA, so you'll need to pre-fund.

* You can choose `no` for pre-funding the pre-compiled accounts (0x1 .. 0xff) with wei. This keeps the genesis cleaner.

* Complete the rest of the prompts, and when you are back at the main menu, choose the "Manage existing genesis" option.

* Export genesis configurations.

![](https://github.com/anhthi54/Fintech_Homework18/blob/7811daddf1b68dd7ca7eda06747fd7e8a36dc4b8/Screenshot/2.2.PNG)

* Initialize each node with the new `andid54.json` with `geth`.
![](https://github.com/anhthi54/Fintech_Homework18/blob/7811daddf1b68dd7ca7eda06747fd7e8a36dc4b8/Screenshot/3.3.PNG)
![](https://github.com/anhthi54/Fintech_Homework18/blob/7811daddf1b68dd7ca7eda06747fd7e8a36dc4b8/Screenshot/4.4.PNG)

* Run the first node, unlock the account, enable mining, and the RPC flag. Only one node needs RPC enabled.
![](https://github.com/anhthi54/Fintech_Homework18/blob/7811daddf1b68dd7ca7eda06747fd7e8a36dc4b8/Screenshot/8.8.PNG)

* Set a different peer port for the second node and use the first node's `enode` address as the `bootnode` flag.
![](https://github.com/anhthi54/Fintech_Homework18/blob/7811daddf1b68dd7ca7eda06747fd7e8a36dc4b8/Screenshot/7.7.PNG)

### Send a test transaction

* Use metamask to send coins from account andi1 to andi2.

* You will need to use Localhost8545, and include the chain ID, and use ETH as the currency.

* Send a transaction from the `andi1` account to the `andi2' account.
![](https://github.com/anhthi54/Fintech_Homework18/blob/7811daddf1b68dd7ca7eda06747fd7e8a36dc4b8/Screenshot/6.6.PNG)