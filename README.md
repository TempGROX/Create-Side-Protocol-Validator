
<div align=center>
  <img src="https://github.com/TempGROX/TempGROX/blob/main/src/photos/images.png">
  <h1>Create-Side-Protocol-Validator</h1>
  <p>In this small repository there is an instruction with which you can create a Side Protocol project validator</p>
  <br>
</div>

# Creating Validator
Creating a validator always starts with this action, namely, you need to touch the faucet and get your first wallet balance. In order to make it more convenient for you, I will leave you a link to the official faucet of the Side Protocol project: [FAUCET](https://station-test.side.one/faucet)

**Check balances:**
```bash
sided query bank balances <your_wallet_address>
```

**Create Validator:**
After your node has been synchronized and when executing the previous command, you have a non-zero wallet balance displayed, you can start creating a validator, this happens using the following command:
```bash
sided tx staking create-validator \
--from=alice \
--amount=400000000uside \
--pubkey=$(sided tendermint show-validator)  \
--moniker="side_node" \
--security-contact="contact@side.one" \
--chain-id="grimoria-testnet-1" \
--commission-rate="0.1" \
--commission-max-rate="0.2" \
--commission-max-change-rate="0.05" \
--min-self-delegation="400000000" \
--fees="50000uside"
```
To see the value of each flag, first just run this command with the **--help** flag


# The end!
If you liked this guide, please go to all my social networks)

<br>
<div id="badges" align="center">
  <a href="https://discord.com/users/961408999411048461">
    <img src="https://img.shields.io/badge/Discord-blue?style=for-the-badge&logo=https%3A%2F%2Fimg.icons8.com%2Fios%2F50%2Fmedium-logo.png&logoColor=white" alt="LinkedIn Badge"/>
  </a>
  <a href="https://medium.com/@James_Brandon">
    <img src="https://img.shields.io/badge/Medium-black?style=for-the-badge&logo=https%3A%2F%2Fimg.icons8.com%2Fios%2F50%2Fmedium-logo.png&logoColor=white" alt="Youtube Badge"/>
  </a>
  <a href="https://keybase.io/jamesbrandon">
    <img src="https://img.shields.io/badge/Keybase-orange?style=for-the-badge&logo=https%3A%2F%2Fimg.icons8.com%2Fios%2F50%2Fmedium-logo.png&logoColor=white">
  </a>
  <a href="https://x.com/JBTGrox">
    <img src="https://img.shields.io/badge/Twitter-blue?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter Badge"/>
  </a>
  <a href="https://linktr.ee/JBrandon_?utm_source=linktree_admin_share">
    <img src="https://img.shields.io/badge/Linktree-green?style=for-the-badge&logo=https%3A%2F%2Fimg.icons8.com%2Fios%2F50%2Fmedium-logo.png&logoColor=white">
  </a>
</div>
