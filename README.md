Create a new JavaScript file in your project directory, for example index.js . Then, copy the code below into this file:

        const wallet = {
            address: address,
            privateKey: privateKey
        };

        const walletJSON = JSON.stringify(wallet, null, 4);

        fs.writeFileSync('wallet.json', walletJSON);

        console.log(`Wallet created and saved to wallet.json`);
    } catch (error) {
        console.log(error)
    }
}

createP2PKHwallet();
