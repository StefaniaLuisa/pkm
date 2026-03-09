No Javascript is on the Free and Flexible Engaging Networks template - that is the main difference

It is the very basic bare bones info

#4site/ENgrid

> [!WARNING]
> **Around October/November 2025** - 4Site updated the baked in GTM Events - now they are not showing, any redundancy removed. This was rolled out globally and all clients using ENgrid have been updated.
>
> Documentation is now updated as well: <https://engrid.4sitestudios.com/docs/v2/gtm-datalayer>
>
> Related Tasks in Productive: <https://app.productive.io/2650-4site-interactive-studios-inc/tasks/14646061>

# ENgrid Thank You | Call To Action

<https://act.ran.org/page/72188/donate/2>

# Remember Me | Explainers & Resources

[Remember Me - General Functionality Doc](https://docs.google.com/document/d/1UcFtl8z23MXEbfoXTc_hRDxniIXOVmbG5btCgR1qnEg/edit?usp=sharing)

- [x] Ask Bryan if this is still up-to-date

Remember me alone is just the ability to recognize and auto-fill forms. What RAN has where it shows what is saved and allows editing is a seperate additional Feature.

Listen to: <https://fathom.video/share/z-EM97WRhHA9Be5Gpxcgdt6ctYfLvsxZ>

### 2025 AIUSA - Custom Implementation

> **Overview**
>
> Recording: <https://cln.sh/jk720Zby>
>
> We will develop a new Remember Me experience that is tailored for the unique requirements of the Urgent Action Network forms. This will be developed as a client theme-side ENgrid component, and AIUSA will be able to add it to individual pages by adding a Code Block from the component library to that page.
> ****Deliverables**
>
> A Remember Me component that will:
>
> - Appear as a checkbox, which is checked by default.
>
> - Be visible on all page loads (even if the user has selected for Remember Me to be enabled already).
>
> - Unchecking the checkbox will also forget the user if they were already being remembered.
>
> - The user’s data will be stored in an encrypted cookie on the [act.amnestyusa.org](http://act.amnestyusa.org) domain.
>
> - We won’t need to use a remote URL for storing a cookie since its usage is limited to the embedded UAN page.
>
> - The cookie will be encrypted using a hard-coded seed.
>
> - To prevent conflicts with ENgrid’s main Remember Me component, it won’t run if this component is active on the page.
>
> It will have configurable options to:
>
> - Control the positioning of the checkbox.
>
> - Change the label of the checkbox.
>
> - Define which fields should be saved into and refilled by the component.
>
> Once complete, hand over to Bryan for QA in [~~#68 QA of Remember Me for UAN~~](https://app.productive.io/2650-4site-interactive-studios-inc/task/10876465) and then leave task open and move to next week. This parent task will be used for client communication.
> ****Update from Bryan:**

*&gt; *Now, be default, anyone submitting the embedded Urgent Action Network EN form will have the “Remember Me” option pre-selected. If they then submit the form, their info will be saved and re-populated on subsequent visits. If on a subsequent visit they de-select the “Remember Me” option, the moment they uncheck it the corresponding “Remember Me” cookie will be deleted.*

*&gt; *Recording: [https://cln.sh/jk720Zby](https://cln.sh/jk720Zby)*

*&gt; *I believe with that, this UAN project is wrapped. Heather is OOO this week and will follow-up when she back with any remaining next steps or close out work.*

### **Explainer from Bryan for FWW | 2025**

> [*https://app.productive.io/2650-4site-interactive-studios-inc/tasks/9109469*](https://app.productive.io/2650-4site-interactive-studios-inc/tasks/9109469)
>
> Hi [Angie Aker](https://app.productive.io/2650-4site-interactive-studios-inc/person/195516) the custom solution we've developed, called "Remember Me", allows a supporter filling out a form to opt into their personal information being "remembered". This information is stored in their browser, and can be used to re-populate any future form they visit. The solution is cookie based, and will use what's known as a first-party cookie hosted on the FWW website.
>
> The solution builds on top of your existing forms, so long as you can add Javascript to those pages. What's unique is that it also work across domains and sub-domains, normal cookies can no do this. For example someone who opts into having their information be remembered on an Engaging Networks page could then have it populated on a natively hosted WordPress page, an ActBlue page, or anywhere else it gets integrated; and vice-a-versa.
>
> Here you can see it in action on the [Rainforest Action Network Engaging Networks](https://act.ran.org/page/72188/donate/1) pages. I've previously opted into being remembered, so when I return all my information is filled out for me ( <https://cln.sh/xGqdhzpw> ). I then have the option to clear my information, and once I do I can then re-opt in while filling out the form.
>
> The look of the checkbox, it's tooltip, it's location on the page, etc.. are all customizable.
>
> There is no ability to store payment information at the moment because that would trigger a number of compliance related requirements and we think the big payment platforms are better suited for that type of task.
>
> To get a scope together, can you send me a list of example pages you would like it to be integrated on. Would it just be your Engaging Networks pages or would it extend to other forms hosted on other platforms and services? Also what info would you want to store? Most folks go with all the classic personal info and address fields, but we can customize this to be less or more based on your needs.

### Explainer to Shatterproof | 2024

<https://cln.sh/NpmPDFHZ>

Here's a before and after screenshot, showing someone opting in to "Remember Me" and visiting a page cold but having their personal info repopulated into the page: <https://cln.sh/NpmPDFHZ>

Live example: <https://act.ran.org/page/60781/donate/1>

> [*https://app.productive.io/2650-4site-interactive-studios-inc/tasks/4836415*](https://app.productive.io/2650-4site-interactive-studios-inc/tasks/4836415)
>
> “Remember Me” is a solution we build for Engaging Networks pages that a visitor to opt-into without needing to “login”. Once opted in, the supporters info will be repopulated on their subsequent visits until they choose to “clear” the prepopulation. This solution is cookie based and is already in use by several clients; and it works cross domain / cross sub-domain. This solution has less friction than requiring the user to “login” and covers scenarios the email links will not, like a supporter arriving at an EN page without coming from an email link but having previously opted into being remembered.
>
> Forms with Remember Me Added:

- <https://act.oceana.org/page/180820/donate/1?mode=DEMO>
- <https://act.ran.org/page/72188/donate/1?ea.tracking.id=w_ran&en_og_source=w_ran>
  - <https://streamable.com/b6onpj>

#### **Disclaimer Copy**

> "Check "Remember me" to complete forms on this device faster. While your financial information won't be stored, you should only check this box from a personal device. Click "Clear autofill" to remove the information from your device at any time.

### NWF Implementation | 2023

> Overview provided to NWF by Fernando | Jun 7, **2023**
>
> - [Task](https://app.productive.io/2650-4site-interactive-studios-inc/tasks/4825233) where this is explained
>
> - The purpose of this LOE/Hours Inquiry is to estimate the effort required to implement the “Remember Me” feature in NWF advocacy forms and donation pages. The feature will allow supporters to securely save their contact details using encrypted cookies, providing convenience for future engagements without storing any payment data. This overview will highlight the benefits of incorporating the “Remember Me” feature.
>
>   ### **Benefits:**
>
>   1. **Enhanced User Experience:** By implementing the “Remember Me” feature, supporters will experience a streamlined and convenient process when engaging with advocacy forms and donation pages. They will no longer need to repeatedly enter their contact information, saving time and effort, and encouraging increased participation.
>   2. **Increased Conversion Rates:** The “Remember Me” feature has the potential to improve conversion rates by simplifying the user journey. By reducing friction and eliminating the need for repetitive data entry, supporters are more likely to complete their actions, leading to higher conversion rates and increased engagement with the NWF’s cause.
>   3. **Streamlined Giving Experience:** When a supporter takes an action, such as signing a petition or joining a mailing list, and opts to “Remember Me,” their contact information will be securely stored. When they visit later to make a donation, their saved information will be pre-filled in the donation form, providing a personalized and convenient experience. This pre-filled information encourages seamless and frictionless donations, enhancing the overall supporter experience.
>   4. **Improved Data Accuracy:** With the “Remember Me” feature, NWF can ensure accurate and up-to-date contact information for your supporters. By pre-filling contact details based on stored preferences, the risk of manual data entry errors is minimized. This leads to more reliable communication, effective donor management, and a clean donor database. If any of the supporters information has changed since it was saved in the encrypted Remember Me cookie, they will be able to change it before submitting the form, and then that new information will be used to update the values stored in the cookie.
>
>   The implementation of the “Remember Me” feature is estimated to require approximately **8 hours of development time**.
>
>   Let me know if you have questions!
>
>   Best, Fernando
>
>   ### NWF Updates Since:
>
> - 2023 - [Add “Remember Me” Checkbox to forms](https://app.productive.io/2650-4site-interactive-studios-inc/projects/39172/tasks/task/5388623?filter=NjU4NjEx)
>
> - [2023 - Support Task to implementation ](https://app.productive.io/2650-4site-interactive-studios-inc/tasks/5388634):
>
>   ```plaintext
>   The rememberme scripting requires that HTML file to be hosted at the client's domain (preferably the main domain), because it will be the domain that stores the form content for autofill later.
>   
>   ie, when a site visitor visits support.nwf.org and makes a donation, we might store a cookie containing the address & phone & email, at the remote domain transmitted via JS window messages.
>   
>   Then, the site visitor may later visit the main www.nwf.org site, and encounters an embedded volunteer form.  Because they opted in on rememberme, the cookie containing that info would be read in and then autofilled on their form.
>   
>   This scenario could also work in reverse -- the visitor volunteers via the embedded form on the main www.nfw.org site (and opts in to rememberme), the form content is saved to the remote domain as a cookie, and then autofilled when they later visit a donation page at support.nwf.org.
>   
>   ```

- NWF [2024 Update](https://app.productive.io/2650-4site-interactive-studios-inc/tasks/6774323)

  - <https://github.com/4site-interactive-studios/engrid-nwf/blob/c393280f6dc86444b2f5700f6e190f22554c6600/src/index.ts#L99>

- NWF 2025 Task - In Icebox

  - *Update your pages with our "Remember Me" support so supporters can opt-in to having their info saved and populated on subsequent form visits even if they come to an EN page outside of a campaign link: [https://act.ran.org/page/72188/donate/1?ea.tracking.id=w_ran&en_og_source=w_ran](https://act.ran.org/page/72188/donate/1?ea.tracking.id=w_ran&en_og_source=w_ran)*

---