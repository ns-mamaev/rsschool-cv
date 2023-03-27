# Nikita Mamaev

## Frontend developer

### Contact information:

* Email: palmally@gmail.com
* Telegram: [@ns_mamaev](https://t.me/ns_mamaev)
* Location: Kazan, Russia
* Ready to relocate

### About myself:
I got interested at the web development as a hobby in November 2021 and I immediately liked it. I am really impressed with modern web services and want to be a part of this industry. After more than a year of training and practice, I decided to completely move into this bussiness.
I interested to learn a new technologies and improving my skills. I've been working as a frontend developer for about six months now, but I know how important it is not to stop learning

### Technologies stack:

- Core technologies:
  - JavaScript with ES6
  - TypeScript
- Markup:
  - HTML 5
  - CSS 3
  - SCSS
- Frameworks & Libraries:
  - React
  - Redux & Redux Toolkit
- Backend:
  - NodeJS
  - ExpressJS
  - MongoDB
  - PostgreSQL
- Assembly:
  - Webpack
  - Parcel
- Testing:
  - Jest
  - Storybook


### The code example
[Task (codewars.com): ](https://www.codewars.com/kata/52742f58faf5485cae000b9a/javascript)


Need to write a function which formats a duration, given as a number of seconds, in a human-friendly way.
For example: For seconds = 3662, function should return "1 hour, 1 minute and 2 seconds"


Solution:
```
function formatDuration (time) {
  if (time === 0) {
    return 'now'
  }
  const formats = [['second', 60],['minute', 60],['hour', 24],['day', 365],['year', Infinity]];
  const res = []
  
  for (let [type, qty] of formats) {
    const value = time % qty
    time = (time - value) / qty;
  
    if (value === 0) continue;
    res.push(`${value} ${type}${value !== 1 ? 's' : ''}`)
    
    if (time === 0) break;
  }
  
  return res.reverse().join(', ').replace(/, (?!.+,)/, ' and ');
}
```

## My projects:

- Movie search (SPA with auth, which allow you to find interesting movie and save it to your collection):
  - Stack: React.js, CSS3, HTML5
  - Code: https://github.com/ns-mamaev/movies-explorer-frontend

- Simple web-store (in progress):
  - Stack: TypeScript, React.js, SCSS, Redux Toolkit
  - Code: https://github.com/ns-mamaev/react-bikes

## Courses:
- Web Developer: Yandex Practicum in 2022;
- JS / FRONT-END: RS School (2023 - now);

## Languages:
- English A2
- Russian Native