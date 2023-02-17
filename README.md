# Hackathon: Concordium Hackathon - The Future of Identity

Concordium Mainnet address: 3kKn2kz9YHrkrKUcBZF9NUJbg8LqGzcBbLwzH1VPBdEqseZH1c

The Concordium blockchain is a technologically advanced and meticulously designed blockchain that facilitates both private and public transactions, while adhering to strict regulatory standards. With its unparalleled scientific foundation, it boasts a high throughput, expedited transaction processing, and predictable fee structures, empowering businesses, developers, and traders to fully leverage the transformative power and potential of blockchain technology.

Prior to utilizing the Concordium blockchain, it is strongly recommended acquainting oneself with the fundamental principles and concepts of this distinct blockchain.

# TASK 1: Setup Development Environment

- Install Rust
- Install cargo-concordium
- Install Concordium-client
- Install the Web Wallet
- Create a Testnet account
- Acquiring testnet CCD via the CCD faucet
- Export the account from web wallet and import it into concordium client

# Install Rust and Cargo

Download and install [Rustup](https://rustup.rs/) which installs both Rust and Cargo.

If on Unix, enter the following command:

```console
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

Make sure to select the default option at the terminal (1).

<img src="./img/1.png">

# Install Wasm

```console
rustup target add wasm32-unknown-unknown
```

<img src="./img/2.png">

# Install Concordium

Download and install [Concordium 2.7.0](https://developer.concordium.software/en/mainnet/net/installation/downloads-testnet.html#cargo-concordium-testnet). Rename it to ```cargo-concordium```.

<img src="./img/3.png">

If one Unix, move the renamed file to something clear but within your PATH, such as:

```console
- mv cargo-concordium ~/.cargo/bin
```

Note, if on MacOS, chmod it like:

```console
chmod +x path/to/cargo-concordium
```

Then, test you set it up correctly by typing:

```console
cargo concordium --help
```

You should see a screen that indicates you've got it working.

# Install Concordium Client

Assigned tutorials use concordium-client as a command line tool to deploy, mint, and transfer. So, if you're on MacOS, the installer should be straightforward and be installed with the [binary](https://developer.concordium.software/en/mainnet/net/installation/downloads-testnet.html#concordium-node-and-client-download-testnet) file. Remember to rename the package to concordium-client in case it has a different version.

<img src="./img/4.png">
<img src="./img/5.png">

Check the installation (1):

```console
concordium-client --help
```
<img src="./img/6.png">
And then connect to testnet (2):

```console
concordium-client consensus status --grpc-port 10000 --grpc-ip node.testnet.concordium.com
```

<img src="./img/7.png">

# Setup a wallet and setup testnet

Get a Concordium browser-extension wallet for Chrome/Brave/Firefox [here](https://developer.concordium.software/en/mainnet/net/browser-wallet/setup-browser-wallet.html#setup-bw).

The wallet uses a 24-word secret recovery phrase to secure your wallet. Nobody will ever ask you for it, and keep it secret!

Now configure the wallet to sit on testnet, with an ID account built from the Concordium testnet IP and identity.

Follow the instructions accordingly:

<img src="./img/8.png">
<img src="./img/9.png">
<img src="./img/10.png">
<img src="./img/11.png">
<img src="./img/12.png">
<img src="./img/13.png">

# Acquiring testnet CCD via the CCD faucet

Also, request 2000 CCD from the testnet faucet:

<img src="./img/14.png">

Acquiring testnet CCD via the CCD faucet

And then, use your wallet to export the keys:

You can now use <YOUR PUBLIC ADDRESS.export> to create a
```concordium-client``` configuration and a ```wallet```.


# Export the account from web wallet and import it into concordium client

Write down the following command accurately:

```console
concordium-client config account import <YOUR PUBLIC ADDRESS.export> --name <Your-Wallet-Name>
Enter encryption password: <TYPE_A_PASSWORD>
```

<img src="./img/15.png">

Concordium Mainnet address: 3kKn2kz9YHrkrKUcBZF9NUJbg8LqGzcBbLwzH1VPBdEqseZH1c
Concordium Testnet address: 4jRDrPgWdyfecgA6USLgk9ABfHByzNVMucht96q6VYokhSu6id

Once done, all should be written to the disk and you're done!

---

<h1><img src="https://emojis.slackmojis.com/emojis/images/1643514974/10003/catjam.gif?1643514974" width="30"/> Hey there!</h1>

<p>Welcome to my GitHub!</br>

I'm 0xSilkweave, a front-end developer and Web3 enthusiast. 

---

###

<p align="left">Tools:</p>

###

<div align="left">
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"><img src="https://github.com/0xSilkweave/0xSilkweave/raw/main/logos/javascript-original.svg" width="36" height="42" alt="JavaScript" /></a>
<a href="https://reactjs.org/" target="_blank" rel="noreferrer"><img src="https://github.com/0xSilkweave/0xSilkweave/raw/main/logos/react-colored.svg" width="36" height="42" alt="React" /></a>
<a href="https://developer.mozilla.org/en-US/docs/Glossary/HTML5" target="_blank" rel="noreferrer"><img src="https://github.com/0xSilkweave/0xSilkweave/raw/main/logos/html5-original.svg" width="36" height="42" alt="HTML5" /></a>
<a href="https://www.w3.org/TR/CSS/#css" target="_blank" rel="noreferrer"><img src="https://github.com/0xSilkweave/0xSilkweave/raw/main/logos/css3-original.svg" width="36" height="42" alt="CSS3" /></a>
<a href="https://www.figma.com/" target="_blank" rel="noreferrer"><img src="https://github.com/0xSilkweave/0xSilkweave/raw/main/logos/figma-colored.svg" width="36" height="42" alt="Figma" /></a>
<a href="https://tailwindcss.com/" target="_blank" rel="noreferrer"><img src="https://github.com/0xSilkweave/0xSilkweave/raw/main/logos/tailwindcss-colored.svg" width="36" height="42" alt="TailwindCSS" /></a>
<a href="https://getbootstrap.com/" target="_blank" rel="noreferrer"><img src="https://github.com/0xSilkweave/0xSilkweave/raw/main/logos/bootstrap-original.svg" width="36" height="42" alt="Bootstrap" /></a>
<a href="https://vitejs.dev/" target="_blank" rel="noreferrer"><img src="https://github.com/0xSilkweave/0xSilkweave/raw/main/logos/vite.svg" width="36" height="42" alt="Vite" /></a>
<a href="https://nodejs.org/en/" target="_blank" rel="noreferrer"><img src="https://github.com/0xSilkweave/0xSilkweave/raw/main/logos/nodejs-colored.svg" width="36" height="42" alt="NodeJS" /></a>
<a href="https://firebase.google.com/" target="_blank" rel="noreferrer"><img src="https://github.com/0xSilkweave/0xSilkweave/raw/main/logos/firebase-colored.svg" width="36" height="42" alt="Firebase" /></a>
<a href="https://docs.alchemy.com/alchemy/documentation/alchemy-web3" target="_blank" rel="noreferrer"><img src="https://github.com/0xSilkweave/0xSilkweave/raw/main/logos/alchemy-colored.svg" width="36" height="42" alt="Alchemy" /></a>
<a href="https://hardhat.org/" target="_blank" rel="noreferrer"><img src="https://github.com/0xSilkweave/0xSilkweave/raw/main/logos/hardhat-colored.svg" width="36" height="42" alt="Hardhat" /></a>
<a href="https://ethereum.org/en/" target="_blank" rel="noreferrer"><img src="https://github.com/0xSilkweave/0xSilkweave/raw/main/logos/ethereum-colored.svg" width="36" height="42" alt="Ethereum" /></a>
</div>

<p align="left">Contact:</p>

###
<div align="left">
  <a href="https://twitter.com/0xSilkweave" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Twitter&logo=twitter&label=&color=1DA1F2&logoColor=white&labelColor=&style=for-the-badge" height="35" alt="0xSilkweave"  />
  </a>
  <a href="https://discordapp.com/users/0xSilkweave#0947" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Discord&logo=discord&label=&color=7289DA&logoColor=white&labelColor=&style=for-the-badge" height="35" alt="0xSilkweave#0947"  />
  </a>
</div>

###
