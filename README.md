<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
  <img alt="Ömer Can Başboğa, full-stack developer in Istanbul. Java and Spring Boot, React, and data that shows up messy from five places at once." src="assets/banner-light.svg" width="100%">
</picture>

Most of what I've built at work is internal tooling other teams end up relying on: a sea-level monitoring service that pulls from five outside networks, the admin side of an ISO 27001 single sign-on system, a student club system with a two-signature approval flow, and a matching pipeline where a local LLM only gets the cases the rules can't decide.

The repos here are my own rewrites of that work with made-up data, so they can be public. Four of them run in your browser.

**[Website](https://omercanbasboga.github.io)**, **[CV](https://omercanbasboga.github.io/assets/OmerCanBasboga_CV.pdf)**, **[LinkedIn](https://www.linkedin.com/in/%C3%B6mer-can-ba%C5%9Fbo%C4%9Fa-b7940223a)**, or write to omercan.basboga@gmail.com. Open to roles in Istanbul or remote.

## Try these in your browser

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://omercanbasboga.github.io/campus-portal/"><img src="https://omercanbasboga.github.io/assets/shots/campus-portal.webp" alt="campus-portal landing page"></a>
      <p><b><a href="https://omercanbasboga.github.io/campus-portal/">campus-portal</a></b><br>
      Three React apps, built and deployed on their own, joined in the browser with Module Federation: login analytics, staff and student records, an org chart.<br>
      <sub><a href="https://github.com/Omercanbasboga/campus-portal">code</a>, React, Module Federation, MUI, Highcharts</sub></p>
    </td>
    <td width="50%" valign="top">
      <a href="https://omercanbasboga.github.io/monitoring-hub/"><img src="https://omercanbasboga.github.io/assets/shots/monitoring-hub.webp" alt="monitoring-hub dashboard"></a>
      <p><b><a href="https://omercanbasboga.github.io/monitoring-hub/">monitoring-hub</a></b><br>
      Eight gauges, two feeds each. When the primary goes quiet the backup fills the hole and every missed slot is logged.<br>
      <sub><a href="https://github.com/Omercanbasboga/monitoring-hub">code</a>, Java, Spring Boot, Redis, PostgreSQL, React</sub></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <a href="https://omercanbasboga.github.io/org-management-console/"><img src="https://omercanbasboga.github.io/assets/shots/club-office.webp" alt="Club Office approval queue"></a>
      <p><b><a href="https://omercanbasboga.github.io/org-management-console/">Club Office</a></b><br>
      Student clubs with a two-step approval. Sign a request as the club's advisor, switch to the admin, approve it.<br>
      <sub><a href="https://github.com/Omercanbasboga/org-management-console">console</a> and <a href="https://github.com/Omercanbasboga/org-management-service">service</a>, Spring Boot, Spring Security, React</sub></p>
    </td>
    <td width="50%" valign="top">
      <a href="https://omercanbasboga.github.io/hollowmere/"><img src="https://omercanbasboga.github.io/assets/shots/hollowmere.webp" alt="Hollowmere title screen"></a>
      <p><b><a href="https://omercanbasboga.github.io/hollowmere/">Hollowmere</a></b><br>
      A match-3 in a dark-fantasy world I made up. Fill a creature's ward meter to seal it for the rest of the run.<br>
      <sub><a href="https://github.com/Omercanbasboga/hollowmere">code</a>, JavaScript, with a <a href="https://github.com/Omercanbasboga/hollowmere-liveops">Spring Boot config service</a></sub></p>
    </td>
  </tr>
</table>

## More code

**Backend and data**

- [unit-matcher](https://github.com/Omercanbasboga/unit-matcher): messy unit names from several HR systems matched to one org tree. Rules first, a local LLM (Qwen on Ollama) for the unsure cases, a person for the rest, and it learns from their answers.
- [sso-gateway-bff](https://github.com/Omercanbasboga/sso-gateway-bff): reactive OAuth2/OIDC backend-for-frontend. Tokens stay on the server.
- [minmax-lttb-downsampler](https://github.com/Omercanbasboga/minmax-lttb-downsampler): 30,000 points down to 300 without losing the one spike that matters.
- [installment-scheduler](https://github.com/Omercanbasboga/installment-scheduler): buy-now-pay-later plans that don't lose a cent to rounding.
- [tallyup](https://github.com/Omercanbasboga/tallyup): group expenses settled in as few transfers as possible.

**Frontend**

- [iam-admin-console](https://github.com/Omercanbasboga/iam-admin-console): clients, users, roles and scopes for the gateway; five near-identical screens became one component.
- [monitoring-hub-dashboard](https://github.com/Omercanbasboga/monitoring-hub-dashboard): the first, standalone version of the monitoring-hub charts.

**Games**

- [hollowmere-vigil](https://omercanbasboga.github.io/hollowmere-vigil/): a branching text RPG in the same world, where most choices are real d20 checks. English and Turkish.

<sub>Java, Spring Boot, Spring Security, Python, PostgreSQL, Redis, MongoDB, React, MUI, Node.js, Docker, Ollama</sub>
