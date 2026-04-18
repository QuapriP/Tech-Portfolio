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
![Navigate to Manage Domains](screenshots/1_Navigate_to_Manage_Domain.png)

### Step 2 - Sign into DNS console
![Sign into DNS Console](screenshots/2_Sign_into_DNS_Console.png)

### Step 3 - Choose method to activate Gmail
![Choose method to activate Gmail](screenshots/3_Chose_method_to_activate_Gmail.png)

### Step 4 - Domain setup success
![Domain setup success](screenshots/4_Domain_setup_success.png)

---

## Section 2: Split delivery setup

Configured split delivery to route inbound email for inactive and unrecognized accounts to a legacy mail platform, while active Google Workspace users continue receiving mail normally. This involved setting up a Gmail host, creating a named mail route pointing to the legacy server with TLS enforced, opening Gmail routing settings, and configuring the inbound routing rule with the appropriate account type targeting and route assignment.

### Step 1a - Open Gmail host settings
![Open Gmail Host Settings](screenshots/1a_Open_Gmail_Host_Settings.png)

### Step 2a - Add new mail route
![Add new Mail route](screenshots/2a_Add_new_Mail_route.png)

### Step 3a - Set up legacy host route and save
![Setup Legacy Host route and save](screenshots/3a_Setup_Legacy_Host_route_and_save.png)

### Step 4a - Open Gmail routing settings
![Open Gmail routing settings](screenshots/4a_Open_Gmail_rounting_settings.png)

### Step 5a - Configure inbound actions
![Configure inbound actions](screenshots/5a_Configure-inbound-actions.png)

### Step 6a - Choose route and save
![Choose route and save](screenshots/6a_Choose_route_and_save.png)

---

## Section 3: Dual delivery setup

Configured dual delivery to send a copy of inbound messages to both Google Workspace and a secondary recipient destination simultaneously. This involved modifying the inbound routing rule to add an additional delivery target, selecting the Advanced configuration mode, and enabling the "Also deliver to" option with the legacy mail platform set as the change route destination, with spam suppression and bounce suppression applied.

### Step 1b - Configure inbound modify
![Configure inbound modify](screenshots/1b_Configure-inbound-modify.png)

### Step 2b - Also deliver - add recipient
![Also deliver - add recipient](screenshots/2b_Also_deliver_-_add_recipient.png)

### Step 3b - Choose Advanced from the drop down
![Choose Advanced from the drop down](screenshots/3b_Choose_Advanced_from_the_drop_down.png)

### Step 4b - Change route to legacy and save
![Change route - legacy - save](screenshots/4b_Change_route-_legacy-_save.png)

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

*Part of an ongoing IT portfolio under QP Works LLC. Additional Google Workspace and IAM documentation in progress.*# Tech-Portfolio
Labs and examples showcasing my skills, ability, and experience.
