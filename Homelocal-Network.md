


Yes — you can **create your own domain name locally** without buying one, but it will only work **on your own network** (or for your own testing), not on the public Internet.

## Short version
- **FQDN** = the full name of a machine, like `server01.home.local`
- **DNS** = the system that translates names to IP addresses
- You can make your own local names **without buying a real domain**

## Example
You could use something like:

- `server01.local`
- `lab.home`
- `nas.internal`

These are not public Internet domains, but they can work on your LAN if you configure DNS or your hosts file.

## Important difference
If you do **not** buy a real domain, then:
- your name is not globally reachable on the Internet
- it is only usable inside your network or for local testing

## “Without buying it” options
You can use:
- a **private/local domain** such as `home.arpa` or `lan`
- a **custom internal name** like `server01.local`
- your own DNS server on the network

## So, is it the same as FQDN?
Not exactly.

- A **FQDN** is just the full hostname format
- A **DNS name** is what the DNS system resolves
- You can have a FQDN that is **not** publicly registered, and that is totally fine for private use

> A good practical rule:
> - If it’s for your home/lab network, use something like `server01.local` or `server01.home.lan`
> - If you want it to work publicly on the Internet, then you need to buy/register a real domain

If you want, I can also explain the difference between:
- `server01.local`
- `server01.home.arpa`
- `server01.example.com`



==========================================================================================================================
==========================================================================================================================

question first can i create my own domain name with-out buying it and would that be the same as FQDN or DNS?

Absolutely — here’s the cleanest way to think about it.

## 1) `server01.local`

This is a **hostname + local domain suffix**.

- `server01` = the machine name
- `.local` = a common private/local suffix

So:

- `server01.local` is a **full name** (an FQDN-like name for local use)
- It is **not** automatically a real public Internet domain
- It is often used for **home/lab/private networks**

### Why people use `.local`
It’s convenient because many systems treat `.local` as a “this is for local networking” kind of name.

### Example
If your machine is named `server01` and you use:

- `server01.local`

then that is a readable local network name.

---

## 2) Difference between `server01.local` and a real domain

A real domain would look like:

- `server01.example.com`

That is different because:

- `example.com` is a registered domain name
- it can be used publicly on the Internet if DNS is set up correctly

But:

- `server01.local` is usually just for local/private use

---

## 3) Fedora hostname values: `static`, `transient`, and `pretty`

Fedora uses three different hostname fields. They are stored separately.

### `static`
This is the **main permanent hostname**.

- It is the one that should normally be used for system identity
- It is usually what you set with:
  ```bash
  sudo hostnamectl set-hostname server01
  ```
- It is the “real” hostname value the system tries to keep

### `transient`
This is a **temporary runtime hostname**.

- It may be set automatically by DHCP or network tools
- It can change while the system is running
- It is often used if the network gives the machine a different name temporarily

### `pretty`
This is the **human-friendly display name**.

- It can contain spaces and punctuation
- Example:
  - `My Home Server`
- It is mainly for display, not for strict networking rules

---

## 4) Simple example

If you run:

```bash
hostnamectl
```

you might see something like:

- Static hostname: `server01`
- Transient hostname: `server01`
- Pretty hostname: `Server 01`

Or maybe:

- Static: `server01`
- Transient: `server01.local`
- Pretty: `Server 01`

---

## 5) Why this matters

- `static` is the “real” configured hostname
- `transient` may be changed by the network
- `pretty` is just for showing nicely

A common setup is:

- `static` = `server01`
- `transient` = `server01`
- `pretty` = `Server 01`

---

## 6) Very short summary

- `server01.local` = a usable local network name
- `static` = permanent hostname
- `transient` = temporary/managed hostname
- `pretty` = friendly display label




# Check or change each one on Fedora with simple commands

I’m pulling together the exact commands now so you can see how to check and change each hostname value on Fedora.

Absolutely — here are the exact commands you can run on Fedora.

## 1) Check everything
```bash
hostnamectl
```

You’ll usually see:

- `Static hostname`
- `Transient hostname`
- `Pretty hostname`

---

## 2) Check the short hostname only
```bash
hostname
```

This shows the current hostname value the shell is using.

---

## 3) Check the full name / FQDN-like value
```bash
hostname -f
```

This may or may not work depending on your DNS setup.

---

## 4) Set the static hostname
If you want to set the permanent hostname:

```bash
sudo hostnamectl set-hostname server01
```

That sets the static hostname to:

- `server01`

---

## 5) Set the pretty hostname
This is just the friendly display name:

```bash
sudo hostnamectl set-hostname "Server 01" --pretty
```

That gives you a human-friendly name.

---

## 6) Set a transient hostname
You can also set a temporary one:

```bash
sudo hostnamectl set-hostname server01.local --transient
```

This is usually not what you want for permanent setup, but it’s useful to know.

---

## 7) Set the static hostname to a full local name
If you want the permanent hostname to be:

```bash
server01.local
```

you can do:

```bash
sudo hostnamectl set-hostname server01.local
```

---

## 8) Verify after changing
Run:

```bash
hostnamectl
```

again to confirm what changed.

---

## Quick example
If you want a clean local setup, a common choice is:

- Static: `server01`
- Pretty: `Server 01`

and then use `server01.local` only as a local network name if needed.

> If you want, I can next show you the exact difference between using `hostnamectl` and editing hostname manually.

-------

Yes — exactly. If you changed it to `moonlabs.local`, that means you are using a **custom local hostname/FQDN-style name** for your machine, and you can absolutely change it later if you want.

## What that means
- `moonlabs` = the short machine name
- `.local` = a local/private suffix
- Together, `moonlabs.local` is just a readable name for your network

## So yes, you can change it
You can change it anytime with:

```bash
sudo hostnamectl set-hostname newname
```

or, if you want a full local style name:

```bash
sudo hostnamectl set-hostname newname.local
```

## A good way to think about it
- `hostname` = system name
- `moonlabs.local` = a full name you chose for local use

## Important note
This does **not** mean you automatically own a real public Internet domain.  
It just means your machine has a name you chose for your network.

> So your understanding is correct: you can change the hostname whenever needed, as long as the name is suitable for your setup.
