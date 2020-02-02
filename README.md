# todoist
A Todo list built with Firebase for realtime updates, React hooks, Sass, Accessibility and unit testing.

This is a following a very insightful tutorial that I found on Youtube - https://www.youtube.com/watch?v=HgfA4W_VjmI&t=1506s

# Programmer Diary
Because this is such an immense project, I decided to document my personal thoughts as I was following along. These can be discoveries, frustrations, and insights that I can look back on to reflect what it is that I truly learnt from this.

## Part 1:
- Basic setup of the project structure - realizing that it's very good practice to separate hooks, helpers from your App.js. This cleans up a lot of logic within App.js! Seeing custom hooks makes me realize that our final project could have been a lot cleaner instead of creating multiple unnamed useEffects.
-Intro to firebase - not a relational database like SQL. This is more of a documented database which is saved on the cloud for realtime updates. Slightly different syntax - it's basically an object that has methods on it where you can do .find or .where, for example.
- Seeing the basic process of instantiating the HTML document and separting the sidebar, nav, header in the Layout folder.

- Frustrations and discoveries: Seeing nested ternary operators was very challenging - I'm not sure if I will ever try to use them as he did in the tutorial to be honest. Long lines of if statements is always confusing and unreadable. Still trying to see why he called unsubscribe() as a method because I think it's a variable... maybe I'm wrong.

## Part 2:
- SCSS setup along with context as well as firebase indexing for unique IDs.
Reflection: it's comforting to see that such an easy task such as deleting is actually complicated, and that things that may seem hard to me, are actually hard to others as well! Basic logistic for deleting -> delete project off firebase -> that will run the context of getProject -> which will fire off the hook that it imports -> which will send back to the local state. Not so easy anymore eh?
- Apart from that, I will probably have to revisit context in the react docs to get a more solid understanding of Provider and Taker.

## Part 3:
- Building major functionality finally using the hooks that we built in part 1 & 2. There was a lot of logic separating each category, adding each task to the correct category, etc. It was nice to see that even a simple feature could take hours to do implement properly. There were also lots of conditional rendering, raw JSX templating and a nice design perspective to see how a typical programmer would solve things.
