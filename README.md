# Google Workspace Administration

![Google Workspace](https://img.shields.io/badge/Google%20Workspace-Admin-green)
![Email Routing](https://img.shields.io/badge/Email%20Routing-blue)
![DNS%20/%20Domain%20Setup](https://img.shields.io/badge/DNS%20%2F%20Domain%20Setup-gray)

Hands-on documentation of Google Workspace admin tasks completed as part of IT administration work under QP Works LLC. Covers domain configuration with DNS setup, split delivery routing, and dual delivery configuration. Screenshots are provided for each step to demonstrate practical execution in the Google Admin Console.

**Skills:** Google Admin Console | DNS configuration | MX records | Gmail host settings | Split delivery | Dual delivery | Email routing | Domain verification | TLS/secure transport

---

## Section 1: Domain setup

Configured a custom domain within Google Workspace, including navigating to the domain management console, signing into the DNS provider, choosing the Gmail activation method via MX record setup, and confirming successful domain verification with DKIM activation.

### Step 1 - Navigate to Manage Domains
![Navigate to Manage Domains](screenshots/1%20Navigate%20to%20Manage%20Domain.png)

### Step 2 - Sign into DNS console
![Sign into DNS Console](screenshots/2%20Sign%20into%20DNS%20Console.png)

### Step 3 - Choose method to activate Gmail
![Choose method to activate Gmail](screenshots/3%20Chose%20method%20to%20activate%20Gmail.png)

### Step 4 - Domain setup success
![Domain setup success](screenshots/4%20Domain%20setup%20success.png)

---

## Section 2: Split delivery setup

Configured split delivery to route inbound email for inactive and unrecognized accounts to a legacy mail platform, while active Google Workspace users continue receiving mail normally. This involved setting up a Gmail host, creating a named mail route pointing to the legacy server with TLS enforced, opening Gmail routing settings, and configuring the inbound routing rule with the appropriate account type targeting and route assignment.

### Step 1a - Open Gmail host settings
![Open Gmail Host Settings](screenshots/1a%20Open%20Gmail%20Host%20Settings.png)

### Step 2a - Add new mail route
![Add new Mail route](screenshots/2a%20Add%20new%20Mail%20route.png)

### Step 3a - Set up legacy host route and save
![Setup Legacy Host route and save](screenshots/3a%20Setup%20Legacy%20Host%20route%20and%20save.png)

### Step 4a - Open Gmail routing settings
![Open Gmail routing settings](screenshots/4a%20Open%20Gmail%20rounting%20settings.png)

### Step 5a - Configure inbound actions
![Configure inbound actions](screenshots/5a%20Configure-inbound-actions.png)

### Step 6a - Choose route and save
![Choose route and save](screenshots/6a%20Choose%20route%20and%20save.png)

---

## Section 3: Dual delivery setup

Configured dual delivery to send a copy of inbound messages to both Google Workspace and a secondary recipient destination simultaneously. This involved modifying the inbound routing rule to add an additional delivery target, selecting the Advanced configuration mode, and enabling the "Also deliver to" option with the legacy mail platform set as the change route destination, with spam suppression and bounce suppression applied.

### Step 1b - Configure inbound modify
![Configure inbound modify](screenshots/1b%20Configure-inbound-modify.png)

### Step 2b - Also deliver - add recipient
![Also deliver - add recipient](screenshots/2b%20Also%20deliver%20-%20add%20recipient.png)

### Step 3b - Choose Advanced from the drop down
![Choose Advanced from the drop down](screenshots/3b%20Choose%20Advanced%20from%20the%20drop%20down.png)

### Step 4b - Change route to legacy and save
![Change route - legacy - save](screenshots/4b%20Change%20route-%20legacy-%20save.png)

---

## Skills demonstrated

- Navigating the Google Admin Console at an administrative level across Domains, Gmail, and Routing settings
- DNS record management and MX record configuration for domain verification and Gmail activation
- DKIM activation for email authentication and spoofing protection
- Configuring Gmail host settings and named mail routes with TLS and CA certificate validation enforced
- Building inbound routing rules targeting specific account types (active vs. inactive/unrecognized)
- Distinguishing between and implementing both split delivery and dual delivery architectures
- Understanding of email delivery flow in hybrid and migration environments

---

*Part of an ongoing IT portfolio under QP Works LLC. Additional Google Workspace and IAM documentation in progress.*
