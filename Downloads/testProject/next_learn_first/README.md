## introduction to nextJS
# why next over react.js
__ SSR is enable along with CSR __
__ CSR require on useState, button, inputpage.(or when error occur) __
__ "use client" for CSR else default is SSr __
__ CDN is not possible in nextJs but in react. __
__ SEO Optimised product in nextJS : by solveing waterfalling problem and fast rendering through SSR __
__ Waterfalling problem is solved first broswer as for request and the script.js got and then build by user so SEO bot didn't got what is web page about and what's on page. while in nextJs request call and dirct html css and js given to enduser __
__ Routing is enabled by next but rect router is lib that also solve the problem in react and also SEO optimizing libraries also there but no one is near to nextJS. __
# installation steps and understanding.
__ src directry no installation reastion src/app if yes no /app there just one folder difference only and App Routher is introduce in next13.js where u do create folder inside that page.tsx and layout.jsx all that wonders of filebase routhing is done due to yes in App Router. and then @ as import alias No mean default Yes mean custom (prefferd default and no with src and yes with app roter)  __
__ @ mean root of project to locate app folder then @/app __
__ every folder on created with name is going to route and insde that folder with layout or page.tsx is must. page.tsx is react code that render on that route page. __
__ global.css is going to apply entire project with tailwind.css so tune as per project __
__ @/app/page.tsx is render code on root route __
__ layout.tsx is require when repeattion of layout for upcomming allroutes. Like when banner is require for all signin, signout, login and logout like this https://domain/auth/sign.... or https://domain/auth/login... then mention in auth folder and then layout.tsx banner code do mention child by passing props otherwise page.tsx will not work. __
__ problem when u want layout but not tweek the route then make auth folder hidden in route by name schema like (auth) (_folder_name_) part of mergin routes __
__ next.config.mjs is config file of next js project require to tweek on deployment. __
__ .next folder is similar .dist folder in react project where dev build is created. __
__ tweek the tialwind config file if ur folder has is consider as tailwind classes to apply css genrally root pages, app and components folder are by default__
