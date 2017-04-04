# The Principles of Email Design
A repository of coding resources for anyone first dipping their toes into the waters of HTML email design. Godspeed.

Originally released as part of a [Litmus Live Workshop](https://litmus.com/email-workshops) of the same name.

## Traditional Responsive

This approach uses the three tenets of responsive design to create responsive HTML emails. It relies on media queries, fluid tables, and fluid images, all of which are now well-supported in most email clients. For those clients that don't support media queries or embedded styles, the hybrid/spongy approach below is a good alternative.

Example can be found in `Traditional Responsive Emails`.

## Hybrid/Spongy Approach

This approach, first introduced by [Fabio Carneiro](), uses fluid-by-default tables, combined with `max-width` styles and Outlook ghost tables to create responsive emails. It is an excellent approach when media queries or embedded styles aren't supported, as it works nearly everywhere. It also serves as a good base to build on, with media queries used as progressive enhancements for email clients that support them.

Example can be found in `Hybrid Emails`.

## Different Development Approaches

Below are three alternative approaches to building responsive HTML email campaigns. Each has its pros and cons, so choose wisely.

### Fab Four Technique

As pioneered by [Rémi Parmentier](https://medium.freecodecamp.com/the-fab-four-technique-to-create-responsive-emails-without-media-queries-baf11fdfa848), this approach uses an understanding of `width`, `max-width`, `min-width`, and the `calc()` function to allow for different layouts across desktop and mobile devices.

Example can be found in `Alternative Approaches/fab-four.html`.

### Mobile-First Approach

First introduced by [Stig Morten Myre](https://cm.engineering/coding-mobile-first-emails-1513ac4673e), this approach also uses `width`, `max-width`, `min-width`, and the `calc()` function, combined with Microsoft ghost tables and `display: table;` (plus a few hacks) to achieve responsive emails. This builds on the mobile version first, which is a nice way to approach email as more subscribers move towards consuming email via mobile devices. It works damned near everywhere and is a nice base to build on.

Example can be found in `Alternative Approaches/mobile-first.html`.

### Div-Based Design

This approach relies primarily on `div` elements as the containers and `display: table;` as the layout mechanism of your email. Nearly every email client, with the exception of Outlook, understands layout with `divs`. For Outlook clients, ghost tables are employed to get layouts rendering properly. Depending on the complexity of your design, this can be a great approach as it can keep your code lean and easy to maintain.

Example of a single-column, minimal approach can be found in `Alternative Approaches/nearly-table-free.html`.

Example of a complex, div-based email can be found in `Alternative Approaches/div-based.html`.
