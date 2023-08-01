## Module 19 Challenge
Submission for Bryan Tran Lu. 

## Description


## Instructions


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
