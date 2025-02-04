# **ASDA Webmaxter's Guide to Affordable, Fast, and Customizable Websites**

## **Introduction**

Welcome to the ASDA Webmaster’s repository! This project is dedicated to helping ASDA members set up their own **WordPress websites** at a fraction of the cost of platforms like Wix or Squarespace.

Many dental students and future dentists will eventually manage their own practice websites. Understanding website infrastructure now will prepare us to make informed decisions later.

My name is Max \([\[Insta\]](https://www.instagram.com/maxterr12/) [\[LinkedIn\]](https://www.linkedin.com/in/maxwellmendelson/)\), and I serve as the WebMaxter for the University of Maryland School of Dentistry ASDA chapter. Over the past year, I migrated our chapter’s website from Wix to WordPress, hosting it on a DigitalOcean server. This transition has significantly reduced our costs, and I’d love to share the process with other chapters! Check out the site [here](https://umbasda.org/).

## **Why WordPress?**

Most website builders charge around **\$30/month** for hosting and an additional **\$27/year** for a domain—totaling **\$370/year**. By switching to **WordPress + DigitalOcean + Namecheap**, costs are reduced to:

- **\$6/month** for hosting (\~\$72/year)
- **\$14/year** for a domain (via Namecheap)
- **Total: \~\$86/year**

This setup gives you a **faster, more customizable, and cost-effective** website.

---

## **Understanding Website Basics**

A website consists of two key components:

### **1. The Computer (Server) Running WordPress**

Any computer can technically host a website. If you wanted, you could run a website from a computer at home, and people could access it using your **IP address** (e.g., `192.168.1.1`).

However, home hosting has downsides:

- **Your internet speed may not be fast enough.**
- **If your computer turns off, your site goes down.**
- **You may need to configure security and updates manually.**

To solve this, we rent a **cloud server** (a "Droplet") from **DigitalOcean**, ensuring **24/7 uptime and high speeds**.

### **2. The Domain Name (Your Website Address)**

A domain name (e.g., `umbasda.org`) acts as your website’s virtual real estate. Instead of users typing in an IP address, they type a domain name that points to your server.

Domain names are purchased from **domain registrars** like Namecheap.

- **Simple, short, and well-known domains** are expensive (e.g., `asda.org` would cost thousands).
- **Basic domains (.com, .org, .net)** typically cost **\$12-\$14/year**.
- **Some extensions (.xyz, .info, .club) are cheaper but may appear less professional.**

It's crucial to **renew your domain every year**—if it expires, someone else can buy it, and you might lose access to your site.

---

## **Step-by-Step: Setting Up a WordPress Website on DigitalOcean**

### **1. Set Up a DigitalOcean Droplet for WordPress**

[How to Set Up WordPress on DigitalOcean](https://www.youtube.com/watch?v=HJ46hjXl3uY)

1. **Create a DigitalOcean Account** ([Sign up here - use this link for free credits (\$200 for 60 days)](https://m.do.co/c/1fb519dbd266))
2. **Create a "Droplet" (Cloud Server)**
   - Choose **Ubuntu 22.04**
   - Select the **\$6/month** plan - **Make sure someone is accountable for keeping up with the payments** - not the end of the world if a payment is missed, unlike domains...
   - Choose a data center near your users
3. **Access Your Droplet**
   - In the video, he uses the app 'Putty'. However, putty is not necessary. You can access the console from the WordPress site.

---

### **2. Purchase a Domain from Namecheap**

[How to Register a Domain on Namecheap](https://www.namecheap.com/support/knowledgebase/article.aspx/9776/6/how-to-register-a-domain-name/)

1. Go to [Namecheap](https://www.namecheap.com/)
2. Search for your desired domain
3. Purchase and **enable auto-renewal**   - **MAKE SURE SOMEONE IS ACCOUNTABLE FOR KEEPING UP WITH PAYMENTS. IF YOU FORGET, YOU ARE AT RISK FOR LOSING THE DOMAIN. I HAVE SEEN THIS HAPPEN TO PLENTY OF ASDA SITES!!**

---

### **3. Restore the Website Backup (Optional, but recommended)**
- _FYI: You will be using your ip address to access your website_
- Click [here](https://umbasda.org/?page_id=425) for umbsod ASDA download link to serve as a template for your chapter's site.
1. Install the **All-in-One WP Migration by ServMask** plugin.
2. Use it to **import the ************`umbasda-org.wpress`************ file**.
   - This resets the WordPress server but may interfere with domain settings, so do this **before setting up the domain**.
3. Go to **WordPress Settings** and update the site URL so that WordPress recognizes the new domain.
4. Login at `xxx.xxx.xx.xx/wp-login.php` using:
   - **Username:** WebMaster
   - **Password:** WebMaster\$Password
   - **Change this password immediately upon logging in.**

---

### **4. Set Up Email Forwarding**

1. Go to [ImprovMX](https://app.improvmx.com/) and create an account.
2. Forward the **predental email** (e.g., `predental@umbasda.org`) to the **webmaster's email**.
3. Inside **Outlook**, set up an automatic forward from the **webmaster's email** to the **predental chair**.
   - This way, the webmaster handles email forwarding, and the predental chair doesn’t have to deal with it.

---

### **5. Connect Your Domain to DigitalOcean**

[Step 1. Linking it from NameCheap](https://www.namecheap.com/support/knowledgebase/article.aspx/767/10/how-to-change-dns-for-a-domain/)\
[Step 2. Linking it to DigitalOcean](https://docs.digitalocean.com/products/networking/dns/how-to/add-domains/#add-a-domain-using-the-control-panel)  <- Follow the instructions under 'Add a Domain Using the Control Panel'

---

## **Installed Plugins**

- **All-in-One WP Migration** (Backup & Migration Tool)
- **Block Visibility** (Controls block visibility)
- **Elementor** (Drag & drop page builder)
- **Kadence Blocks** (Advanced Gutenberg blocks)
- **Kadence Starter Templates** (Prebuilt site templates)
- **Disable Admin Email Verification Prompt** (Removes WordPress admin verification popups)
- **RSS Importer** (Imports RSS feed posts)
- **Specific Content for Mobile** (Creates mobile-specific content)
- **WP fail2ban** (Enhances security via logs)
- **WP File Manager** (Manage website files)
- **WP Maximum Upload File Size** (Increases upload limit)

---

## **Future Development & Contributions**

This repository will be updated as the project evolves. If you have **suggestions, improvements, or additional resources**, feel free to:

- Create a **pull request**
- Open an **issue**
- Reach out with ideas

By working together, we can build a **cost-effective, fast, and reliable** website solution for ASDA chapters and future dental practices.

**Trust me, if you can do a filling, you can make a website... probably... feel free to reach out :^D 🚀**
