PaperWallet
===========
Fork of 2.8.1 release of bitaddress (https://github.com/pointbiz/bitaddress.org/releases/tag/v2.8.1), modified to work with Groestlcoin.

If you want to see the history of changes, get 2.8.1 from https://github.com/pointbiz/bitaddress.org/releases/tag/v2.8.1 and get original checkin from this repo. Compare them. They will match. After this, it'll be easy to track changes.

PS: bitaddress.org.html is generated from individual .js files using "grunt" tool

If you would like to help with translating for a particular language use this template:

			// javascript alerts or messages                        
			"testneteditionactivated": "TESTNET EDITION ACTIVATED",
			"paperlabelbitcoinaddress": "Groestlcoin Address:",
			"paperlabelprivatekey": "Private Key (Wallet Import Format):",
			"paperlabelencryptedkey": "Encrypted Private Key (Password required)",
			"bulkgeneratingaddresses": "Generating addresses... ",
			"brainalertpassphrasetooshort": "The passphrase you entered is too short.\n\n",
			"brainalertpassphrasewarning": "Warning: Choosing a strong passphrase is important to avoid brute force attempts to guess your passphrase and steal your groestlcoins.",
			"brainalertpassphrasedoesnotmatch": "The passphrase does not match the confirm passphrase.",
			"detailalertnotvalidprivatekey": "The text you entered is not a valid Private Key",
			"detailconfirmsha256": "The text you entered is not a valid Private Key!\n\nWould you like to use the entered text as a passphrase and create a Private Key using a SHA256 hash of the passphrase?\n\nWarning: Choosing a strong passphrase is important to avoid brute force attempts to guess your passphrase and steal your groestlcoins.",
			"bip38alertincorrectpassphrase": "Incorrect passphrase for this encrypted private key.",
			"bip38alertpassphraserequired": "Passphrase required for BIP38 key",
			"vanityinvalidinputcouldnotcombinekeys": "Invalid input. Could not combine keys.",
			"vanityalertinvalidinputpublickeysmatch": "Invalid input. The Public Key of both entries match. You must input two different keys.",
			"vanityalertinvalidinputcannotmultiple": "Invalid input. Cannot multiply two public keys. Select 'Add' to add two public keys to get a groestlcoin address.",
			"vanityprivatekeyonlyavailable": "Only available when combining two private keys",
			"vanityalertinvalidinputprivatekeysmatch": "Invalid input. The Private Key of both entries match. You must input two different keys."     

			// header and menu html
			"tagline": "Open Source JavaScript Client-Side Groestlcoin Wallet Generator",
			"generatelabelbitcoinaddress": "Generating Groestlcoin Address...",
			"generatelabelmovemouse": "MOVE your mouse around to add some extra randomness...",
			"generatelabelkeypress": "OR type some random characters into this textbox",
			"singlewallet": "Single wallet",
			"paperwallet": "Paper wallet",
			"bulkwallet": "Bulk wallet",
			"brainwallet": "Brain wallet",
			"vanitywallet": "Vanity wallet",
			"detailwallet": "Wallet Details",
			
			// footer html
			"footerlabeldonations": "Donations to bitaddress.org developer",
			"footerlabeltranslatedby": "Translated by Groestlcoin",
			"footerlabelpgp": "PGP",
			"footerlabelversion": "Based on bitaddress.org v2.8.1",
			"footerlabelgithub": "GitHub Repository",
			"footerlabelcopyright1": "Copyright bitaddress.org, Groestlcoin developers.",
			"footerlabelcopyright2": "JavaScript copyrights are included in the source.",
			"footerlabelnowarranty": "No warranty.",
			
			// single wallet html
			"newaddress": "Generate New Address",
			"singleprint": "Print",
			"singlelabelbitcoinaddress": "Groestlcoin Address",
			"singlelabelprivatekey": "Private Key (Wallet Import Format)",
			"singletip1": "<b>A Groestlcoin wallet</b> is as simple as a single pairing of a Groestlcoin address with its corresponding Groestlcoin private key. Such a wallet has been generated for you in your web browser and is displayed above.",
			"singletip2": "<b>To safeguard this wallet</b> you must print or otherwise record the Groestlcoin address and private key. It is important to make a backup copy of the private key and store it in a safe location. This site does not have knowledge of your private key. If you are familiar with PGP you can download this all-in-one HTML page and check that you have an authentic version from the author of this site by matching the SHA1 hash of this HTML with the SHA1 hash available in the signed version history document linked on the footer of this site. If you leave/refresh the site or press the "Generate New Address" button then a new private key will be generated and the previously displayed private key will not be retrievable. Your Groestlcoin private key should be kept a secret. Whomever you share the private key with has access to spend all the groestlcoins associated with that address. If you print your wallet then store it in a zip lock bag to keep it safe from water. Treat a paper wallet like cash.",
			"singletip3": "<b>Add funds</b> to this wallet by instructing others to send groestlcoins to your Groestlcoin address.", 
			"singletip4": "Check your balance</b> by going to https://chainz.cryptoid.info/grs and entering your Groestlcoin address.",
			"singletip5": "<b>Spend your groestlcoins</b> by going to one of the exchanges and sweep the full balance of your private key into your account at their website. You can also spend your funds by downloading one of the popular groestlcoin p2p clients and importing your private key to the p2p client wallet. Keep in mind when you import your single key to a groestlcoin p2p client and spend funds your key will be bundled with other private keys in the p2p client wallet. When you perform a transaction your change will be sent to another groestlcoin address within the p2p client wallet. You must then backup the p2p client wallet and keep it safe as your remaining groestlcoins will be stored there. Satoshi advised that one should never delete a wallet.",
			
			// paper wallet html
			"paperlabelhideart": "Hide Art?",
			"paperlabeladdressesperpage": "Addresses per page:",
			"paperlabeladdressestogenerate": "Addresses to generate:",
			"papergenerate": "Generate",
			"paperprint": "Print",
			"paperlabelBIPpassphrase": "Passphrase:",
			"paperlabelencrypt": "BIP38 Encrypt?",
			
			// bulk wallet html
			"bulklabelstartindex": "Start index:",
			"bulklabelrowstogenerate": "Rows to generate:",
			"bulklabelcompressed": "Compressed addresses?",
			"bulkgenerate": "Generate",
			"bulkprint": "Print",
			"bulklabelcsv": "Comma Separated Values:",
			"bulklabelformat": "Index,Address,Private Key (WIF)",
			"bulklabelq1": "Why should I use a Bulk Wallet to accept groestlcoins on my website?",
			"bulka1": "The traditional approach to accepting groestlcoins on your website requires that you install the official groestlcoin client daemon ("groestlcoind"). Many website hosting packages don't support installing the groestlcoin daemon. Also, running the groestlcoin daemon on your web server means your private keys are hosted on the server and could get stolen if your web server is hacked. When using a Bulk Wallet you can upload only the groestlcoin addresses and not the private keys to your web server. Then you don't have to worry about your groestlcoin wallet being stolen if your web server is hacked.",
			"bulklabelq2": "How do I use a Bulk Wallet to accept groestlcoins on my website?",
			"bulklabela2li1": "Use the Bulk Wallet tab to pre-generate a large number of groestlcoin addresses (10,000+). Copy and paste the generated comma separated values (CSV) list to a secure text file on your computer. Backup the file you just created to a secure location.",
			"bulklabela2li2": "Import the groestlcoin addresses into a database table on your web server. (Don't put the wallet/private keys on your web server, otherwise you risk hackers stealing your coins. Just the groestlcoin addresses as they will be shown to customers.)",
			"bulklabela2li3": "Provide an option on your website's shopping cart for your customer to pay in Groestlcoin. When the customer chooses to pay in Groestlcoin you will then display one of the addresses from your database to the customer as his "payment address" and save it with his shopping cart order.",
			"bulklabela2li4": "You now need to be notified when the payment arrives. Google "groestlcoin payment notification" and subscribe to at least one groestlcoin payment notification service. There are various services that will notify you via Web Services, API, SMS, Email, etc. Once you receive this notification, which could be programmatically automated, you can process the customer's order. To manually check if a payment has arrived you can use Block Explorer. Replace THEADDRESSGOESHERE with the groestlcoin address you are checking. It could take between 1 minute to 10 min for the transaction to be confirmed.<br/> http://www.blockexplorer.com/address/THEADDRESSGOESHERE<br/><br/>Unconfirmed transactions can be viewed at: https://chainz.cryptoid.info/grs <br/>You should see the transaction there within 30 seconds.",
			"bulklabela2li5": "Groestlcoins will safely pile up on the block chain. Use the original wallet file you generated in step 1 to spend them.",
			
			// brain wallet html
			"brainlabelenterpassphrase": "Enter Passphrase:",
			"brainlabelshow": "Show?",
			"brainprint": "Print",
			"brainlabelconfirm": "Confirm Passphrase:",
			"brainview": "View",
			"brainalgorithm": "Algorithm: SHA256(passphrase)",
			"brainlabelbitcoinaddress": "Groestlcoin Address:",
			"brainlabelprivatekey": "Private Key (Wallet Import Format):",
			
			// vanity wallet html
			"vanitylabelstep1": "Step 1 - Generate your "Step1 Key Pair",
			"vanitynewkeypair": "Generate",
			"vanitylabelstep1publickey": "Step 1 Public Key:",
			"vanitylabelstep1pubnotes": "Copy and paste the above into the Your-Part-Public-Key field in the Vanity Pool Website.",
			"vanitylabelstep1privatekey": "Step 1 Private Key:",
			"vanitylabelstep1privnotes": "Copy and paste the above Private Key field into a text file. Ideally save to an encrypted drive. You will need this to retrieve the Groestlcoin Private Key once the Pool has found your prefix.",
			"vanitylabelstep2calculateyourvanitywallet": "Step 2 - Calculate your Vanity Wallet",
			"vanitylabelenteryourpart": "Enter Your Part Private Key (generated in Step 1 above and previously saved)",
			"vanitylabelenteryourpoolpart": "Enter Pool Part Private Key (from Vanity Pool):",
			"vanitylabelnote1": "[NOTE: this input box can accept a public key or private key]",
			"vanitylabelnote2": "[NOTE: this input box can accept a public key or private key]",
			"vanitylabelradioadd": "Add",
			"vanitylabelradiomultiply": "Multiply",
			"vanitycalc": "Calculate Vanity Wallet",
			"vanitylabelbitcoinaddress": "Vanity Groestlcoin Address:",
			"vanitylabelnotesbitcoinaddress": "The above is your new address that should include your required prefix.",
			"vanitylabelpublickeyhex": "Vanity Public Key (HEX):",
			"vanitylabelnotespublickeyhex": "The above is the Public Key in hexadecimal format.",
			"vanitylabelprivatekey": "Vanity Private Key (WIF):",
			"vanitylabelnotesprivatekey": "The above is the Private Key to load into your wallet.",
	
			// detail wallet html
			"detaillabelenterprivatekey": "Enter Private Key",
			"detailkeyformats": "Key Formats: WIF, WIFC, HEX, B64, B6, MINI, BIP38",
			"detailview": "View Details",
			"detailprint": "Print",
			"detaillabelnote1": "Your Groestlcoin Private Key is a unique secret number that only you know. It can be encoded in a number of different formats. Below we show the Groestlcoin Address and Public Key that corresponds to your Private Key as well as your Private Key in the most popular encoding formats (WIF, WIFC, HEX, B64, MINI).",
			"detaillabelnote2": "Groestlcoin Core stores public keys in compressed format. The client now also supports import and export of private keys with importprivkey/dumpprivkey. The format of the exported private key is determined by whether the address was generated in an old or new wallet.",
			"detaillabelbitcoinaddress": "Groestlcoin Address",
			"detaillabelbitcoinaddresscomp": "Groestlcoin Address Compressed",
			"detaillabelpublickey": "Public Key (130 characters [0-9A-F]):",
			"detaillabelpublickeycomp": "Public Key (compressed, 66 characters [0-9A-F]):",
			"detaillabelprivwif": "Private Key WIF (51 characters base58) starts with a",
			"detaillabelprivwifcomp": "Private Key WIF Compressed (52 characters base58) starts with a,
			"detailcompwifprefix": "'K' o 'L'",
			"detaillabelprivhex": "Private Key Hexadecimal Format (64 characters [0-9A-F]):",
			"detaillabelprivb64": "Private Key Base64 (44 characters):",
			"detaillabelprivmini": "Private Key Mini Format (22, 26 or 30 characters, starts with an 'S'):",
			"detaillabelpassphrase": "BIP38 Passphrase",
			"detaildecrypt": "Decrypt BIP38",
			"detaillabelq1": "How do I make a wallet using dice? What is B6?",
			"detaila1": "An important part of creating a Groestlcoin wallet is ensuring the random numbers used to create the wallet are truly random. Physical randomness is better than computer generated pseudo-randomness. The easiest way to generate physical randomness is with dice. To create a Groestlcoin private key you only need one six sided die which you roll 99 times. Stopping each time to record the value of the die. When recording the values follow these rules: 1=1, 2=2, 3=3, 4=4, 5=5, 6=0. By doing this you are recording the big random number, your private key, in B6 or base 6 format. You can then enter the 99 character base 6 private key into the text field above and click View Details. You will then see the Groestlcoin address associated with your private key. You should also make note of your private key in WIF format since it is more widely used."
