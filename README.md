# Nostr Answers

People tend to have the same questions when they first join Nostr, so here are
the answers.

## How do I tag someone with the `@`?

Tagging another user is a bit different that other social media platforms.
Instead of typing `@` and then the person's handle you need to get their public
key. Do this by going to their profile, copying the public key, and then
creating a post that includes `@` and then the public key.

## How do I change my Profile pic?

Another slight difference from other platforms is that you can't directly upload
a profile picture. Instead you have to use a URL to the profile picture. To
achieve this use an image hosting service like [imagebb](https://imgbb.com/).
Upload the photo and then copy the URL to the image and paste that into your
profile.

## What's this Lightning Network thing?

You may have noticed those invoices being sent around Nostr or the lightning
bolt icons on people's profiles. These are links to their Lightning Network
address. The Lightning Network is a layer two protocol built on top of Bitcoin
which provides instantaneous transactions at an extremely low fee.

You can get in on the action by getting a Lightning Network wallet. The simplest
to use is the [Wallet of Satoshi](https://www.walletofsatoshi.com/). Once you
download and install that, you're ready to start zapping people satoshis (a
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
