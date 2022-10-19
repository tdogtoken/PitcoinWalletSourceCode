**1. Clone wallet sources**

```
git clone https://github.com/tdogtoken/PitcoinWalletSourceCode.git
```

**2. Modify `CryptoNoteWallet.cmake`**
 
```
set(CN_PROJECT_NAME "pitcoin")
set(CN_CURRENCY_DISPLAY_NAME "Pitcoin")
set(CN_CURRENCY_TICKER "PBTC")
```

**3. Set symbolic link to coin sources at the same level as `src`. For example:**

Create git submodule:

```
git submodule add https://github.com/tdogtoken/PitcoinSourceCode.git cryptonote
```

Replace URL with git remote repository of your coin.

**4. Build**

```
mkdir build && cd build && cmake .. && make
```
