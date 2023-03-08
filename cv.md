
# Hey! I'm Nikolai Komarov and this is my CV :)

### My contacts:

1. Telegram: +77054144973
2. email: k_k_007@mail.ru
3. discord: Nikkez#8081 (for rs-school channel: Nikolay (@Sancekez))

*********

### About my self

Good day! I'm Nikolai. I'm a 3rd year student at the International University of Information Technology (IITU) in Almaty city. I really want to try to work at large projects and learn new technologies in a team of cool and strong developers.


My work experience is about 1.5 years. I had little experience in team development of small websites and online stores. After I mastered the layout of projects well, I realized that I want to develop as a React JS developer and now I am taking mega cool courses from rs-school.


I set myself the goal of getting a job at EPAM because I believe that this company employs some of the strongest developers in the CIS. I will make every effort to achieve this.


### My skills:

1. HTML
2. JS
3. CSS (SCSS / SASS)
4. BEM Methodology
5. Rest API
6. React JS
7. GIT
8. Webpack
9. npm
10. Vue JS
11. English level B1

*********

### Example of code:

```
function formatDuration (seconds) {
  var time = { year: 31536000, day: 86400, hour: 3600, minute: 60, second: 1 },
      res = [];

  if (seconds === 0) return 'now';
  
  for (var key in time) {
    if (seconds >= time[key]) {
      var val = Math.floor(seconds/time[key]);
      res.push(val += val > 1 ? ' ' + key + 's' : ' ' + key);
      seconds = seconds % time[key];
    }
  }
 
  return res.length > 1 ? res.join(', ').replace(/,([^,]*)$/,' and'+'$1') : res[0]
}
``` 
