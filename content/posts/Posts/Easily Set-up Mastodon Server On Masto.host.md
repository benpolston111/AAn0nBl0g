---
title: Easily Set-up Mastodon Server On Masto.host
date: 2025-02-01
draft: false
tags:
  - AAn0nAAr0n
  - blog
  - tech
  - Mastodon
---
# Host Mastodon on Masto.host

## Down With Elon

I was never a huge bird app user, mostly because I've never really been a social media person. Seeing the owner's recent actions has made me want to get involved somehow. I figure what a better way than aiming for his pockets via promotion of the Fediverse against traditional social media networks.

I know...I know... "Why don't you just self-host? You'd save yourself a little money". First, I was running on zero sleep when I did this and wanted something a little easier. Second, I live in West Virginia and my ISP's up-time is atrocious. Sue me! (Don't actually, I have no moneys for you or attorneys)

## Here's The Process

We're gonna need a small investment (all under $20):

- Domain - I bought mine from [namecheap.com](https://namecheap.com)
- Cloudflare Free Account - Just go to [cloudflare.com](https://cloudflare.com) and sign up
- Masto.host Server - Plans start at $6/month, that's what I went with and we can upgrade later
- Time and Patience - Some of this just takes time, be patient and this should work just fine

### Step 1
#### Buying your domain

![](https://i.ibb.co/sdPTJPB1/namecheap.png)

This is where we search for domains on Namecheap. Not a sponsor, just cheaper than buying directly from Cloudflare. 
From what I can tell with my limited experience of the platform so far, common tld's are .social, .chat, and other social-centric names, but you should be safe to pick anything.

![](https://i.ibb.co/7tNTxpGp/namecheap-select.png)

Find one at a decent price, and checkout like you would normally on any other platform.

### Step 2
#### Starting domain transfer

![](https://i.ibb.co/bjhBr9wm/cloudflare-main.png)

After you've bought your domain, log into cloudflare and click "Add a domain" (if you haven't made an account yet, do it now).

![](https://i.ibb.co/46vfMbC/cloudflare-adddomain.png)

Enter your domain and click continue.

![](https://i.ibb.co/rRJdGfTx/cloudflare-plan.png)

Select Free Plan and click continue.

![](https://i.ibb.co/Mkw2342Z/cloudflare-activation.png)

Click "Continue to activation".

![](https://i.ibb.co/ccsmKZPR/cloudflare-confirm.png)

Click "Confirm". We'll handle the DNS records in a minute.

### Step 3
#### Changing nameservers

![](https://i.ibb.co/G3PwTQ6D/cloudflare-nameservers.png)

We're gonna copy these nameserver addresses to namecheap so we can get the transfer underway.

![](https://i.ibb.co/fWjP1rg/namecheap-transfer.png)

Go back to namecheap, click domain list, and scroll down to nameservers. Here we select Custom DNS and paste our nameserver addresses.

Now here's where the time and patience comes in. Nameservers can take up to 48 hours to complete transfer. This can be a frustrating waiting process, but I promise it almost never takes that long. Cloudflare should send you an email when this process is over so you don't have to stare at your screen (though I always do). As soon as it's transferred, you're ready for the next step! 

### Step 4
#### Finally getting to Mastodon

![](https://i.ibb.co/0VRZ5QJ8/mastohost-start.png)

Next, let's go to Masto.host. You can feel free to start on a larger server, but for my current needs this one works.

![](https://i.ibb.co/tTWrQFTN/mastohost-domain.png)

Click "Your domain".

![](https://i.ibb.co/Lh9zCnVF/mastohost-input.png)

Enter your domain and click "Continue".

![](https://i.ibb.co/Cyg1RRn/mastohost-notice.png)

Make sure you don't have anything else currently hosted on your domain, or just use a subdomain. Click "Use your.domain".

![](https://i.ibb.co/Ld0cW15K/mastohost-subscribe.png)

Click "Subscribe" and go through the payment process.

![](https://i.ibb.co/r2vC68rK/mastohost-dns.png)

After payment is completed, you should see the DNS record we're gonna input over in Cloudflare. So let's hop back over there.

![](https://i.ibb.co/x8BddYGk/cloudflare-finalsteps.png)

On your account dashboard, click your domain.

![](https://i.ibb.co/3mhC7Zx2/cloudflare-dns.png)

Click "DNS Records".

![](https://i.ibb.co/23gDsm1z/cloudflare-dnsman.png)

Enter the DNS record details from Masto.host here, then click "Save". This may take 15-30 minutes, but you should then be able to access your domain in the browser. That's what we'll do next.

### Step 5
#### Finishing steps

![](https://i.ibb.co/9mzdHzHR/masto-accountcreation.png)

Go to your domain in the browser and click "Create Account". Fill in these details and click "Request an account". Then back to Masto.host to make the new account an owner/admin.

![](https://i.ibb.co/p61wXsv7/mastohost-portal.png)

On Masto.host, click "Change User Role".

![](https://i.ibb.co/cS2LF5wC/mastohost-admin.png)

Enter the account username you just created, then click "Change User Role". 

That's it! Log in, administrate a little bit, follow some people and hashtags, and of course have fun! I've been enjoying my time on Mastodon, and it may take some time to get "Federated" and build your platform, but I think it is well worth it.

### Bonus

#### Relays

When you first spawn a Mastodon Instance, it may seem like a very lonely place. With Mastodon you have to build your own community, and it's not a quick process. Relays make your job easier by federating with collections of other servers. Here are some tools I found useful for relays:

[relaylist.com](https://relaylist.com/) - List of relays

[relay.fedi.buzz](https://relay.fedi.buzz/) - Relays from hashtag or by instance

#### Blocklist

Help keep your users safe.

[Garden Fence](https://github.com/gardenfence/blocklist) - Github hosted csv files to block known Nazis, Trolls, Conspiracy Theorists and alike.

#### Themes

Give your instance a unique look.

[TangerineUI-for-Mastodon](https://github.com/nileane/TangerineUI-for-Mastodon) - I use the purple one!

[Mastodon-Bird-UI](https://github.com/ronilaukkarinen/mastodon-bird-ui) - Resembles Twitter (yuck, but to each their own)

#### RSS

RSS tools for Mastodon.

[RSS-Parrot](https://rss-parrot.net/) - Turn Mastodon into your feed reader

#### Learn More

Learning resources for Mastodon and the Fediverse.

[Fedi.tips](https://fedi.tips/) - Best resource I know of for getting started on Mastodon




