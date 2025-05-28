Frosty Delights Website
**Overview**
Frosty Delights is a static website for a delightful snowball dessert business based in Leesburg, VA. The site serves as a digital storefront, showcasing the menu, location, and story of Frosty Delights while providing an easy way for customers to get in touch.
Designed with a clean, responsive layout, the website ensures a seamless experience across devices, inviting users to explore frosty treats and connect with the team.

**Features**

Responsive Design: Fully responsive pages using Tailwind CSS, with a mobile-friendly hamburger menu for navigation on smaller screens.
Navigation: Fixed white navigation bar with links to Home, Menu, About Us, Contact, Location, and Careers pages.
Contact Form: A user-friendly contact form integrated with Formspree, allowing customers to send inquiries to ScapegoatsSnowballs@gmail.com. Upon submission, users are redirected to a custom thanks.html page with an engaging message: “Thank You for Reaching Out! Your message has landed with us, and our team is thrilled to connect with you soon! While you wait, dive into the cool world of our frosty delights!”
Informative Sections: Dedicated pages for menu, location (22025 Evergreen Mills Road, Leesburg, VA), about us, careers, and a contact page with quick contact details, social media links, catering info, and FAQs.
Footer: Consistent black footer across all pages with quick links, contact info (ScapegoatsSnowballs@gmail.com, (703) 957-9523), social media (X, Instagram, Facebook), and hours (Mon-Sat 11 AM-8 PM, Sun 12 PM-6 PM, with Summer Hours on location page: 12 PM-9 PM daily).
Styling: Modern design with Tailwind CSS and Font Awesome icons for a polished, professional look.

**Technologies Used**

HTML5: Static page structure for all pages (index.html, menu.html, about.html, contact.html, location.html, careers.html, thanks.html).
Tailwind CSS: Utility-first CSS framework for responsive, customizable styling.
Font Awesome: Icons for navigation (hamburger menu) and social media links.
jQuery: Handles AJAX form submission for the contact form to ensure smooth redirection to thanks.html.
Formspree: Backend service for processing contact form submissions, sending emails to ScapegoatsSnowballs@gmail.com, and redirecting to thanks.html.
JavaScript: Custom scripts for hamburger menu toggle and Formspree AJAX submission.

**Contact Form Integration**
The contact form on contact.html is integrated with Formspree to handle submissions without a custom backend:

Form Fields: Name, Email, and Message, all required.
Submission: Data is sent to Formspree’s endpoint (https://formspree.io/f/{form_id}), which emails the submission to ScapegoatsSnowballs@gmail.com with the user’s email as the reply-to address.
Redirect: Uses AJAX to prevent Formspree’s default thank-you page, redirecting users to thanks.html with a custom, exciting message.
Spam Protection: Includes a _gotcha honeypot field and Formspree’s Formshield for spam filtering.

**Setup Instructions**

Clone the Repository:git clone https://github.com/your-repo/frosty-delights.git


Install Dependencies: No installation needed, as Tailwind CSS and Font Awesome are loaded via CDNs, and jQuery is included for AJAX.
Formspree Setup:
Sign up at formspree.io and create a new form.
Set the recipient email to ScapegoatsSnowballs@gmail.com.
Copy the form’s endpoint ID (e.g., xabc1234) and replace {form_id} in contact.html’s form action.
Set the redirect URL in Formspree’s dashboard to thanks.html or your hosted absolute URL (e.g., https://yourdomain.com/thanks.html).


Local Testing:
Run a local server (e.g., python -m http.server).
Open contact.html, submit the form, and verify email delivery and redirect to thanks.html.


Deployment:
Host on a platform like Netlify, GitHub Pages, or Cloudflare Pages.
Update _next and AJAX redirect in contact.html to absolute URLs (e.g., https://yourdomain.com/thanks.html).
Test the live form to confirm functionality.



Future Improvements

Backend Enhancements: Integrate additional Formspree plugins (e.g., Google Sheets, Mailchimp) for submission tracking.
Consistency: Update footer hours to match Summer Hours (12 PM-9 PM daily) and standardize phone number to (703) 957-9523 across all pages.
User Experience: Add reCAPTCHA for extra spam protection, a loading state for form submission, or an auto-redirect from thanks.html to index.html after 5 seconds.
Accessibility: Improve ARIA labels and keyboard navigation for better accessibility.

License
© 2025 Frosty Delights. All rights reserved.
Contact
For inquiries, reach out to ScapegoatsSnowballs@gmail.com or submit a message via the contact form.
