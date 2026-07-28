
# Ubuntu Landscape Server

LTS & PPA
LTS (Long Term Support)
PPA (Personal Package Archive)
Refer to two different (but related) parts of how Canonical distributes and supports Landscape.

In Landscape, an **LTS release** means: Long Term Support

* A **stable, production-focused version** of Landscape Server
* Released every ~2 years
* Supported for a **long period (about 10 years total support lifecycle)**
* Receives:

  * Security fixes
  * Bug fixes
  * Point releases (updates within the same LTS line)

👉 Example:

* `Landscape 24.04 LTS`
* `Landscape 26.04 LTS`

📌 In practice:

* You use LTS when you want **stability and minimal upgrades**
* It is the recommended choice for **production systems**


## PPA 
A **PPA is an Ubuntu software repository** used with `apt`. APT = Advanced Package Tool
Used in Ubuntu's Terminal like: `sudo apt update`

For Landscape, Canonical provides different PPAs depending on the release channel you want.

Examples:

| Channel       | PPA                                                          |
| ------------- | ------------------------------------------------------------ |
| LTS           | `ppa:landscape/self-hosted-24.04` (or similar versioned LTS) |
| Latest stable | `ppa:landscape/latest-stable`                                |
| Beta          | `ppa:landscape/self-hosted-beta`                             |

---

## 🔗 So what does “LTS PPA” mean together?

When you see something like:

> **“LTS PPA” in Landscape Server**

It means:

👉 You are using the **PPA channel that delivers the Long Term Support (LTS) version of Landscape**

So:

* **LTS = the type of release (stable, long-term supported version)**
* **PPA = the repository source you add to install or update it**

---

## 🧠 Simple way to think about it

* **LTS = “what version strategy am I on?”**
* **PPA = “where do I download updates from?”**

So an “LTS PPA” is basically:

> “the Ubuntu package repository that gives you the long-term supported version of Landscape Server”



## ⚙️ Why this matters in Landscape

In practice, choosing the LTS PPA means:

* fewer upgrades
* more predictable changes
* safer for production environments
* longer security maintenance window


