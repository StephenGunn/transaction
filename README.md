# Transaction, A resource for rendering and sending transactional emails with Svelte

Transaction is a resource for learning how to render [
https://svelte.dev
](Svelte) components as email friendly markup on the server along with best practices and integrations with the top email sending clients.

The goal of this project is not to provide an opaque library for rendering emails but to provide a resource for learning how to render emails with Svelte and send them with the top email sending clients.

## Svelte Ready Templates

Along with tutorials on how to render emails with Svelte, this project will also provide a collection of ready to use Svelte templates for common transactional emails based on [Postmark Transactional Email Templates](https://github.com/ActiveCampaign/postmark-templates).

The templates we use will feature their styles not inlined but in their `<style>` tag for ease of maintenance and readability. We will programatically inline their styles before sending them with the email sending clients.

## The Templates

These are all sourced from the [Postmark Transactional Email Templates](https://github.com/ActiveCampaign/postmark-templates) and used under the MIT license.

Each template comes in three different generic layout variations: Basic, Basic full, and Plain. This gives you a starting point so that you can customize your templates to match your brand.

<img src="https://github.com/activecampaign/postmark-templates/raw/main/media/starter-templates@2x.png" max-width="100%" alt="Starter templates side-by-side: Basic, basic full, and plain">
<img src="https://github.com/activecampaign/postmark-templates/raw/main/media/dark-mode@2x.png" max-width="100%" alt="Dark mode compatibility">

### Welcome

Send a welcome email to users after they sign up.

- 💌 Preview with layout: [Basic](https://newsletter.postmarkapp.com/assets/templates/dist/basic/welcome/content.html), [Basic full](https://newsletter.postmarkapp.com/assets/templates/dist/basic-full/welcome/content.html), [Plain](https://newsletter.postmarkapp.com/assets/templates/dist/plain/welcome/content.html)
- 📔 [Welcome email best practices guide](https://postmarkapp.com/guides/welcome-email-best-practices)

### Reset Password

Send users a link to reset their password.

- 💌 Preview with layout: [Basic](https://newsletter.postmarkapp.com/assets/templates/dist/basic/password-reset/content.html), [Basic full](https://newsletter.postmarkapp.com/assets/templates/dist/basic-full/password-reset/content.html), [Plain](https://newsletter.postmarkapp.com/assets/templates/dist/plain/password-reset/content.html)
- 📔 [Reset password best practices guide](https://postmarkapp.com/guides/password-reset-email-best-practices)

### Reset Password Help

Help users reset their password if they can’t remember their email.

- 💌 Preview with layout: [Basic](https://newsletter.postmarkapp.com/assets/templates/dist/basic/password-reset-help/content.html), [Basic full](https://newsletter.postmarkapp.com/assets/templates/dist/basic-full/password-reset-help/content.html), [Plain](https://newsletter.postmarkapp.com/assets/templates/dist/plain/password-reset-help/content.html)
- 📔 [Reset password best practices guide](https://postmarkapp.com/guides/password-reset-email-best-practices)

### Receipt

Send a receipt to users after they made a purchase.

- 💌 Preview with layout: [Basic](https://newsletter.postmarkapp.com/assets/templates/dist/basic/receipt/content.html), [Basic full](https://newsletter.postmarkapp.com/assets/templates/dist/basic-full/receipt/content.html), [Plain](https://newsletter.postmarkapp.com/assets/templates/dist/plain/receipt/content.html)
- 📔 [Receipt and invoices best practices guide](https://postmarkapp.com/guides/receipt-and-invoice-email-best-practices)

### Invoice

Request payment from a user.

- 💌 Preview with layout: [Basic](https://newsletter.postmarkapp.com/assets/templates/dist/basic/invoice/content.html), [Basic full](https://newsletter.postmarkapp.com/assets/templates/dist/basic-full/invoice/content.html), [Plain](https://newsletter.postmarkapp.com/assets/templates/dist/plain/invoice/content.html)
- 📔 [Receipt and invoices best practices guide](https://postmarkapp.com/guides/receipt-and-invoice-email-best-practices)

### Dunning

Let users know about a failed payment

- 💌 Preview with layout: [Basic](https://newsletter.postmarkapp.com/assets/templates/dist/basic/dunning/content.html), [Basic full](https://newsletter.postmarkapp.com/assets/templates/dist/basic-full/dunning/content.html), [Plain](https://newsletter.postmarkapp.com/assets/templates/dist/plain/dunning/content.html)
- 📔 [Dunning best practices guide](https://postmarkapp.com/guides/dunning)

### Comment notification

Notify users of new comments by other users.

**Note:** Comment notification isn't the prettiest preview because it's just [Mustachio](https://github.com/activecampaign/mustachio). Since almost all content in this email is dynamic, it won't look good without real content. Don't worry though, that's how it's supposed to look.

- 💌 Preview with layout: [Basic](https://newsletter.postmarkapp.com/assets/templates/dist/basic/comment-notification/content.html), [Basic full](https://newsletter.postmarkapp.com/assets/templates/dist/basic-full/comment-notification/content.html), [Plain](https://newsletter.postmarkapp.com/assets/templates/dist/plain/comment-notification/content.html)
- 📔 [Comment notification best practices guide](https://postmarkapp.com/guides/comment-notification-email-best-practices)

### Trial Expiring

Let users know when their trial is about to expire.

- 💌 Preview with layout: [Basic](https://newsletter.postmarkapp.com/assets/templates/dist/basic/trial-expiring/content.html), [Basic full](https://newsletter.postmarkapp.com/assets/templates/dist/basic-full/trial-expiring/content.html), [Plain](https://newsletter.postmarkapp.com/assets/templates/dist/plain/trial-expiring/content.html)
- 📔 [Trial expiration email best practices](https://postmarkapp.com/guides/trial-expiration-email-best-practices)

### Trial Expired

Let users know when their expired trial.

- 💌 Preview with layout: [Basic](https://newsletter.postmarkapp.com/assets/templates/dist/basic/trial-expired/content.html), [Basic full](https://newsletter.postmarkapp.com/assets/templates/dist/basic-full/trial-expired/content.html), [Plain](https://newsletter.postmarkapp.com/assets/templates/dist/plain/trial-expired/content.html)
- 📔 [Trial expiration email best practices](https://postmarkapp.com/guides/trial-expiration-email-best-practices)

### User Invitation

Help users invite others to use your software.

- 💌 Preview with layout: [Basic](https://newsletter.postmarkapp.com/assets/templates/dist/basic/user-invitation/content.html), [Basic full](https://newsletter.postmarkapp.com/assets/templates/dist/basic-full/user-invitation/content.html), [Plain](https://newsletter.postmarkapp.com/assets/templates/dist/plain/user-invitation/content.html)
- 📔 [User invitation email best practices](https://postmarkapp.com/guides/user-invitation-email-best-practices)

We've also made sure that these have been tested for consistency in the following email clients:

- Desktop
  - Apple Mail 9, 10, 11
  - Outlook 2007, 2010, 2011, 2013, 2016
  - Windows 10 Mail
- Mobile
  - Gmail App (Android)
  - iPhones 6, 7, 8, SE, X
  - iPad (Retina)
  - iPad Mini
  - iPad Pro
- Web
  - AOL
  - Gmail
  - Outlook.com
  - Yahoo
