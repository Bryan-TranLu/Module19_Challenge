## Module 19 Challenge
Submission for Bryan Tran Lu. 

## Note to Grader
* The `def generate_account()` function modified to create a new mnemonic each time. It is understood that this is method is not advised or secure but was added to ensure that the script runs.
* Since a new account is created each time, there is a balance of zero ether and thus an error of 'insufficient funds for gas' occurs when a transaction is made. However, when another ganache address is used the transaction works.

## Instructions
The application script is in `fintech_finder.py` and the required functions are in `crypto_wallet.py`.

1) To launch the Streamlit application, type `streamlit run fintech_finder.py`

2) On the resulting webpage, select a candidate that you would like to hire from the appropriate drop-down menu. Then, enter the number of hours that you would like to hire them for.

3) Click the Send Transaction button to sign and send the transaction with your Ethereum account information. If the transaction is successfully communicated to Ganache, validated, and added to a block, a resulting transaction hash code will be written to the Streamlit application sidebar.

## Installation Requirements
Imports for Crypto Wallet functions:
```python
import os
import requests
from mnemonic import Mnemonic
from dotenv import load_dotenv
load_dotenv()
from bip44 import Wallet
from web3 import Account
from web3 import middleware
from web3.gas_strategies.time_based import medium_gas_price_strategy
```
Imports for Steamlit and Fintech Finder app:
```python
import streamlit as st
from dataclasses import dataclass
from typing import Any, List
from web3 import Web3
w3 = Web3(Web3.HTTPProvider('HTTP://127.0.0.1:7545'))
from crypto_wallet import generate_account, get_balance, send_transaction
```

## Images
Input areas for the user interface of the Streamlit application.

<a href="" target="_blank" rel="noreferrer"><img src="Images/Fintech_Finder.png" width="" height="300" alt="" /></a>

## Authors and Support
If there are any questions regarding the assignment, please reach out via email.
