# CFDStatus
Code for Denver project sites status pages; are they up; status updates every 30 mins


Create React App advice from DD Slack

Alexander Dreith [4:55 PM]
https://reactjs.org/docs/faq-ajax.html (edited) 
But that is for simplicities sake, there are many many forms of implementation beyond that.
Alex Myers [5:09 PM]
thanks this looks like a good and simple enough start;it also helps that I decided to use an online code editor that lets me instantly see any changes I'm making;  I don't have the same luck with VS Code
Alexander Dreith [5:10 PM]
If you start with CRA you should have a pretty good browser + editor experience
Even if you don't use CRA for your final project, it can be an "all the tooling is setup for you" jumping off point for experimenting.
Alex Myers [5:19 PM]
is this the Create React App thing?  it sounds like you're saying there are definite advantages to using it?
Alexander Dreith [5:23 PM]
There are, but I mean specifically if you're just playing around/experimenting with React then using CRA means all you have to do is run `npx create-react-app my-test` and it will scaffold an entire project with tooling and everything inside `/my-test`
And out of the box `npm start` runs a local build in development mode with refresh on change/save etc.
Alex Myers [5:24 PM]
can you elaborate on how you mean by "tooling"?
Alexander Dreith [5:28 PM]
You _want_ to just worry about writing JS. But modern development has babel transpiling to ES6, env variables for whether React is running in development or production mode, live reload, opening a port where the app is running on localhost, webpack (bundling, concatenating, minifying, etc).
You need something like NPM scripts, webpack, etc. to accomplish all those automated tasks for you. You can either write your own scripts, config files, and file structure to scaffold an entire project to be ready for how modern dev is, or you can use an opinionated, pre-built, "bootstrap" project that has all of that tooling setup for you.
CRA is an "out-of-the-box" solution
Alex Myers [5:32 PM]
ah okay thanks for that
Alexander Dreith [5:33 PM]
Run `npx create-react-app my-test` checkout the folder structure and everything. Run `npm start` in `my-test` and change a few things to see it all working etc.
Then run `npm run eject` and look at all the things CRA hid from you. Config files, scripts, etc. Those are all the things that allow you to just run `npm start` and forget about it.
All the new things/files you see popup when you eject is the reason why a lot of people would rather use CRA than have to write/setup that stuff themselves.
