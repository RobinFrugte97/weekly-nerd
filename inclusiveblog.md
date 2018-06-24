# Awesome, but inclusive

Often times, while I'm busy fighting the good fight against pesky deadlines, too caught up in code, I forget something important. Inclusiveness.

When I'm busy working on my project, desperately getting something new to work, I forget about semantics. I forget about a large group of users dependent on assistance tools like screen readers. Things turn out to be awesome, but not inclusive.

During the Meesterproef project our group made the decision to work component-based. Meaning every part of the website we were working on was divided in smaller components. As I took on a couple of components, I ignorantly put the same `div` around each of them. Because, you know, it makes styling so easy!

Unfortunately, the next coaching appointment I was diagnosed with a bad case of Diveritus. However will he survive this, I hear you wonder. Fret not, for I can positively say I have been cured! All it takes for you to be cured of Diveritus, is for you to think twice about what you (and your project team) code!

I took the time to remove all the 'convenient' styling `div`'s, and made sure to do a double check on semantics on my code.

Later on in the project, the exact same happened to my project group mate! He used and implemented an awesome api which allowed all of our components do all sort of fancy animations when the appeared on the viewport. It's called [Intersection Observer](https://developer.mozilla.org/en-US/docs/Web/API/Intersection_Observer_API), by the way. Really cool api that lets you animate elements as they scroll into your viewport. It's not a real lazy-loader, as it indeed does load all elements, it just doesn't display everything. Screen readers like that kind of stuff.

This awesome piece of code was, like my old components, wrapped in all kinds of non-inclusive things, like `div`'s and `article`'s at the same time. I, again, took the time to make sure everything was inclusive again, while making sure the awesome api my group mate got to work still did its job.

Awesome AND inclusive.
