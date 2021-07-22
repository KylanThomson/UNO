| Fundamentals of Building a MDPS and Competitive Web Application |
- Design tokens
   - Design tokens are an agnostic way to store variables such as typography, color, and spacing so that they can be used across multiple platforms and multiple devices without all of the work
     - This is also EXTREMELY IMPORTANT AND USEFUL for when working with multiple apps WITHIN our platform - we can save these styles and spacing and replicate them within our plethora of different applications in uno
   - We store design tokens, normally in a CSS file, into a JSON file that can be transformed to different platforms
     - We can do this with AWS’s style dictionary: Style Dictionary Demo

- Cohesion - the act of making multiple platforms of a software cohesive (but not the same)
  - Layers of cohesion:
    1. Voice & Tone/Branding
      - We want our applications to be cohesive in their branding, tone, and appearance - branding is a key stepping stone to really make an impressionable and recognizable software, especially when entering an already-saturated subindustry of software development
    2. Communication
      - We need communication to be consistent and fleshed out, for example: we ask the users to sign up for email notifications, however, our app (incorrectly) also sends mobile notifications. Then, each time we attempt to send a notification over to their page, they receive an email as well as a mobile notification causing them to receive two at once.  In a large scale organization, it is much more sensible to have a singular communication system across all platforms.
  - Cohesion is great in development naming conventions, where even when components are written differently across platforms, they’re still functionally the same and named similarly creating ease for developers during transfer
    - Look at google material for something like this - reuse of buttons and components etc.
       - We can create design tokens within figma, and break up our design, as shown here: https://i0.wp.com/css-tricks.com/wp-content/uploads/2019/03/1PUtb8ARGrYql5rGLtFen5w.png?ssl=1
       - Using the same example as before, we should name the separate mobile and webapp notification functions with the same names; we don’t want to separate “banner” and “alert” or “error” and “danger”, we want these things to be named the same thing because they function the same 
     - Frequently in software development, the purpose of cohesion is incorrectly emphasized, where developers attempt to make software across platforms work in the same way
       - With our MPDS, we don’t want this to be the case - with the complexity of the application, the mobile version should not contain all the features given to us by the webApp - this would cause clutter and convolution when working on mobile
         - Instead, we should attempt to use the mobile app as a place that the user can set reminders or do menial/on-the-go tasks conveniently - when doing larger scale tasks on the application, the user should opt for the webapp
- Feature Parity - the act of making congruent and consistent features between the different platforms supported by your product
  - Difficulties:
    - Maintaining equality within multiple platforms on release
      - When creating a desktop application for UNO, we have to decide which platforms we want it to be released to, and whether or not we can release undeveloped versions of the product to our non-default platforms (iOS, MacOS, Windows, Linux, WebVersion)
    - Thinking about feature parity within a competitor sense:
      - Within the creation of a MPDS amongst many competitors, we have to separate ourselves one of two different ways (or both!)
        1. How will our individual applications and features draw a user conversion to our software?  What are we doing feature-wise to set ourselves apart from our competitor’s features?
           - Something to note: When attempting to replicate successful features of a competitor’s product, we will always be behind in development compared to them - while we’re attempting to replicate their feature, they will be improving it
             - Solution? Attempt to resolve customers unmet needs, instead of fighting a competitor to meet needs better - if two features are extremely similar, and a company already has an established relationship/subscription with your competitor, then they will likely not be willing to make the switch based on a potential minorly improved feature (especially when your competitor is working to improve that feature in the present) (make your competitors attempt to fight and replicate your features!)
        2. How will our MPDS as a whole encapsulate everything the user wants, and is missing from our competitors?  How will our system, designed to do very similar things as our competitors, be a better union of our design features?
     - When asking consumers to switch to a product, you’re asking them for faith in your product
        - Users will have to transfer data, start over on MPDS customization, and will be forced to learn a new program, all inconveniences costing a company time and money
     - When trying to get a high amount of feature parity, this increases the likelihood of having useless or generally unused features
       - Often times, it is better to build the application in a way that encourages frequent updates and user suggestions, rather than overloading time and capital spent on meaningless features
     - Important principle: 80-20 principle
       - This means that 80% of the benefit your users get using your application comes from 20% of the features
       - Take with grain of salt when creating the MPDS, considering all of the separate applications added to it - the 80-20 principle should be applied to the individual applications over the MPDS
     - For Uno:
       - This can be seen as a challenge for a heavily customizable web application
       - Speculating, it could be problematic to attempt to include customizable pages for mobile devices
         - Creating a way for users to make customizable pages while in mobile means that there has to be a heavily modified system for doing this that would likely work less efficiently than doing so on the computer
       - Mobile devices would require some level of redesign of the UI considering the average size of a customizable home page (expanding far horizontally, usually)
         - However, to gain popularity for our product, we may want to focus on releasing a version of the application along with our initial release of the web app that is underdeveloped amongst competitor multi-platform design systems
