# monero_wallet_cli
Conteinerized Monero CLI Wallet
<b>:: Container Deployment</b>

<i>docker volume create wallets</i>

<i>docker run -d --restart unless-stopped --name xmr-wallet-cli -w /wallets -v wallets:/wallets -it deewhy/monero_wallet_cli</i>

Your MONERO WALLETS will be stored to the persistent volume <i>wallets</i> 

<b>:: Command line</b>

JUST if you aren't planning to deploy and sync your own MONERO NODE, consider to TRUST your favourite node and <i>exec</i> the application as follows:

<i>docker exec -it xmr-wallet-cli /cli/monero-wallet-cli --daemon-address xmr.support:18081 --trusted-daemon</i>

Some online nodes: https://monero.fail/

To restore an EXISTING WALLET from SEED: 

<i>docker exec -it xmr-wallet-cli /cli/monero-wallet-cli --restore-deterministic-wallet --daemon-address xmr.support:18081 --trusted-daemon</i>

Done, ENJOY!

If you like my job PLEASE buy to me a coffee sometime :: <b>Donate</b> to [MONERO]:<br>
48X8E9cm8eigtMfWqZo68K3D6ideqfxn4R56Jzi1duC8jTX3LCD9nd4RyPyLinwaqwdukDxd6BEYFP63RvAAd8NRDGypQGN
