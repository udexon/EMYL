### Online Tipping -- Outside China -- 支外宝

Online tipping is one of the most lucrative captive markets nowadays. China and users of Chinese apps are ahead of the rest of the world in this area with their online payment systems which enables tipping down to a single cent.

Datong Token (name? Datong Tipping？) problems ....

#### Scenario 1: Datong Token with Western Union

<img src="https://github.com/udexon/DatongToken/blob/master/pay_wu.png" width="400"  />

Consider a scenario where Sender A who lives in country P wishes to send an amount X in currency K to Recipient B who lives in country Q.

Sender A requests Recipient B's public key. A encrypts message MA (Datong payment token) and sends token to B. Recipient B decrypts message using own private key. 

Sender A must include own public key in payment token, so that Recipient B can encrypt message MB and send it to Agent C, who lives in the same country Q as B.

Then Agent C can send an encrypted message to Agent D, who lives in the same country P as Sender A, to verify payment.

Once the payment chain is verified, Agent C may collect cash from Sender A physically or use the national banking system in country P to collect the payment. Agent C will pay Agent D using their own international payment method. Agent B can then pay Recipient B cash physically in person, or using the national banking system in country Q.

After Sender A sends the token to Recipient B, presumably via a mobile chat service such as WhatsApp, Sender B will use a Datong app to process then token, then send a new token to Agent C. Agent C again will use a Datong app to process the token, and send a new token to Agent D. Agent D will also use a Datong app to process the token, and send a new token to Sender A.

(We use the term "a Datong app" to imply the fact that third parties may produce apps that comply to the Datong protocols.)

All the transmissions of token can be done by sending text messages on chat apps like WhatsApp.

Finally, Sender A will use a Datong app to verify the token from Agent C, to confirm that Agent C is an authorized agent who will send money via conventional means to Agent D, and Agent D will send money via conventional means to Recipient B. After this confirmation, Sender A may send money to Agent C via conventional means, to initiate the transaction. 


#### Scenario 2: Datong Token with Cryptocurrency

Now consider this variation:

-- Agent C sends money using cryptocurrency L to Agent D.

Let's illustrate the two scenarios in diagrams:

<img src="https://github.com/udexon/DatongToken/blob/master/pay_bch.png" width="400"  />

We now have sufficient understanding to compare and analyse various fundamental issues concerning international financial transactions, cryptocurrencies and Datong Token.

From the technical perspective, what are the roles of RSA in both scenarios?


Firstly, as with Bitcoin, we use RSA cryptosystem to authenticate the users (Sender, Recipient, Agents). 

However, in Bitcoin, after the sender and recipient identities are authenticated, the programs concerned automatically carry out a series of operations to deduct the balance from the wallet of the sender and add the exact same amount in the recipient's wallet (which can be either in software or hardware).

In Datong Token, it is the human users (Sender, Recipient, Agents) who will perform the operations as specified in the token.





Just like HTML and Linux, something small and simple can replicate worldwide and become revolutionary.

Consider a simple act of tipping an Instamgrammer in a developing country like Vietnam using Datong Token.

The Sender A only has to send the Recipient B a text message M, consisting of A's public key APBK, and tip amount X in a local currency, e.g. Vietnam Dong (VND).

At this point, B does not have a Datong account yet. She (he) received the message M from A via private message, or possibly in an Instagram comment, which is publicly viewable. This might be done for promotional purposes, i.e. to show off to other followers.

B only has to download a Datong app and use it to generate her (his) own public key BPBK.

B will then send her public key BPBK to an agent C, together with message M, using the Datong app.

C would need to find an Agent D in the home country of Sender A, who would then collect the payment from A in their national currency using their national banking system. C would pass the message from B to D. D would send the message to A to verify the transaction. The chain of payments as described above will be performed to complete the transaction.

Datong network would have many agents in each country, so that they would compete with each other to lower their commission fees.

As a result, agents using cryptocurrencies will have much greater demand for international money transfer, which in turn improve the adoption of cryptocurrencies.


#### (Non)-Adoption of Cryptocurrencies

Datong Token immediately solves the adoption problem of cryptocurrencies. In order for a particular cryptocurrency to be useful, by definition, the sender and the recipient both have to create a personal account for the cryptocurrency concerned.

In Datong Token, the mechanisms involved in a cryptocurrency transaction are broken down to the bare minimum. In the scenario described above for payment using Datong Token, the sender and recipient do not need to create personal accounts on Datong system. 
