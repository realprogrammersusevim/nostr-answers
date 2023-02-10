# Nostr Answers

![Header](https://raw.githubusercontent.com/realprogrammersusevim/nostr-answers/main/images/header.jpeg)

People tend to have the same questions when they first join Nostr, so here are
the answers.

## How do I tag someone with the `@`?

Many clients now have an autocomplete menu that will pop up when you start
typing the person's name after the `@` symbol. Click on the name and the user's
public key will be inserted into the message.

## How do I change my Profile picture?

Another slight difference from other platforms is that you can't directly upload
a profile picture. Instead you have to use a URL to the profile picture. To
achieve this use an image hosting service like
[nostr.build](https://nostr.build/). Upload the photo and then copy the URL to
the image and paste that into your profile.

## How do I upload an image?

Just like changing your profile picture, Nostr does not support uploading an
image file. Simply upload your image to [nostr.build](https://nostr.build) and
then paste the link into your note. Many clients will automatically get the link
and display the image.

## How do I mention or quote a post?

Mentioning or quoting a note is similar to tagging a user. Copy the ID of the
note and then put `@` and then the ID of the note you wish to reference.

## What's this Lightning Network thing?

You may have noticed those invoices being sent around Nostr or the lightning
bolt icons on people's profiles. These are links to their Lightning Network
address. The Lightning Network is a layer two protocol built on top of Bitcoin
which provides instantaneous transactions at an extremely low fee.

You can get in on the action by getting a Lightning Network wallet. The simplest
to use is the [Wallet of Satoshi](https://www.walletofsatoshi.com/). Once you
download and install the app, you're ready to start zapping people satoshis (a
denominator of Bitcoin).

## How do I find and follow others?

Go to [nostr.directory](https://nostr.directory) to find all the Twitter
accounts you know and love on Nostr. Post `#plebchain` to get followed and find
others to follow.

If you find someone that appears to know what they're doing and probably has a
good feed then copy their public key and log in with it. You'll be able to see
their feed and then log back into your own account to follow the people you
like. Note that you won't be able to see anything personal if you log in with a
public key, only publicly available information like who they follow, and by
extension what posts they receive.

## What's the difference between a public and private key?

A public key is generated from your private key. It's a unique identifier that
allows other users to find, follow, and tag you. Your private key however is the
key to your account. If someone else gets your private key they will have
complete access to your account. **Don't post your private key publicly.** There
is a reason it's called a _private_ key.

## What's the difference between my client and Nostr?

There is an important distinction to be made when talking about Nostr. When you
are using your client such as Damus or Astral the software or website is not
Nostr itself. Nostr is a protocol that specifies a way for computers to talk to
each other like the TCP/IP protocol that's used whenever you visit a website. A
client is a piece of software that implements the Nostr protocol and follows the
rules to talk correctly to the other computers, get the information, and display
it for you.

## How do I get verified?

NIP-05 verification is used to fight impersonation. Handles on Nostr like
`@jack` are not special. Anyone can create an account with that handle. The only
thing that identifies you is your public key. The problem with a public key is
that it's difficult for humans to remember a long random string of letters and
numbers. What NIP-05 does is make sure you can tell which person is the real
one. To be verified your public key needs to be listed on a website. This makes
sure there can be only one `@jack` at a certain domain, in the case of Jack
Dorsey he's verified himself [here](https://cash.app/.well-known/nostr.json).
This makes it easy to tell that you're talking to the real Jack Dorsey because
only he can be `jack@cash.app`. Services like
[nostrplebs.com](https://nostrplebs.com) will verify you or you can use a custom
domain.

## How can I keep my private key secure?

A private key can be thought of as the password to your account. Store it in a
secure location like a password manager as you would any other password. In the
future multi-signature setups my be available, but currently only single key
setups are allowed.

## How do I set up my own relay?

TODO

## Is there a Nostr token?

Nostr is simply a protocol for computers talking with one another. This is like
asking if there is an HTTPS token. No, a token has not been built into the
protocol. If you would like to send people money or fund developers working on
the network many, if not most, of the main clients support tipping through the
Lightning Network.

If you see a Nostr or Damus token it's a scam.

## Do relays talk to each other?

Currently no. When you post your client contacts each of the relays in your list
individually and sends the message. Only the clients you send the message to
will have your message and other relays will never have or store it. Some people
have set up personal relays to pull events from many relays and then only
connect to their personal relay. This can help with data usage as your phone
only has to connect and receive messages from one computer instead of many
different ones often sending identical messages.

## Is Nostr Peer to Peer?

Nostr not peer to peer. Clients only connect to relays, not to each other.

## How do I find the best relays?

TODO

## How many relays should I connect to?

At least 5 is recommended. Any lower than that and you might miss messages from
others or others might not see your messages. The maximum number of relays you
should connect to is more personal. The more relays you have, the more data will
be required contact each relay and download all the new messages. If you don't
have much data on your phone you might want to stick to a lower number. If you
only access Nostr from a desktop and have fast WiFi you could connect to many
more relays

## How can other people find and follow me on Nostr?

The best identifier is your public key. Other people can copy and paste your
public key into their client and find your profile.

## Is my handle unique?

No. Anyone can choose any handle. People are distinguished by their public keys.

## Is Nostr a blockchain?

Nostr is not a blockchain. There is absolutely no blockchain component to the
protocol. Clients send notes to relays which then store them and can retrieve
them if other connected clients wish to have them.
