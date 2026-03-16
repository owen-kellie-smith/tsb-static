# Thornbury Swing Band – Static Site

Plain static HTML site served via GitHub Pages.

https://owen-kellie-smith.github.io/tsb-static/

aka

https://thornburyswingband.co.uk/  [How?](#dns-info)

---

## ✏️ Stuff that goes out of date quickly (so worth editing first)

1. [Upcoming events](#-upcoming-events)
2. [Past events](#-past-events)
3. [Band members](#-band-members) and [Vacancies](#-vacancies)

## Stuff that goes out of date more slowly (but eventually ...)

4. [Repertoire](#-current-repertoire)
5. [Sound Engineer fees](#-sound-engineer-fees)
6. [Practice venue](#-practices)
7. [Music Director](#-music-director)
8. [Manager](#-manager)
9. [Email addresses and phone numbers](#-email-addresses-and-phone-numbers)
   
You can edit any page directly on GitHub — no software needed.

Once you edit the page you may make the line numbers in this README out of date i.e. wrong - but they
aren't part of the public site, so just update them if you want to help future you / some other editor.


**How to edit a file:**
1. Click the link below for the section you want to change
2. Click the **pencil icon** (✏️) in the top-right of the file view
3. Make your changes
4. Click **Commit changes**

The site updates automatically within a minute or two.

---

### 📅 Upcoming events

**File:** [`events-coming-up/index.html`](../../edit/main/events-coming-up/index.html#L36)
*(link opens at the event block, around line 36)*

Each event looks like this — copy and paste to add more:

```html
<div class="event">
  <h3>Event name and location</h3>
  <p class="date">Saturday 14 June 2025 &ndash; 7:30pm</p>
  <p>Any extra details, e.g. venue address or ticket link.</p>
</div>
```

To remove a past event, delete everything from `<div class="event">` to the matching `</div>`.

---

### 🎹 Past events

**File:** [`gigs/index.html`](../../edit/main/gigs/index.html#L32)
*(link opens at the 2024 events list, around line 32)*

- Events are listed as `<li>` items inside `<ul class="info-list">` blocks
- Each year has its own `<h2>Events in 20XX</h2>` heading
- To add a new year, copy an existing `<h2>` + `<ul>` block and update the year and events
- Paste new events at the **top** of the relevant year's list (most recent first)

A basic entry looks like:
```html
<li><strong>Saturday 1 March 2025</strong> &ndash; Event name, Venue name.</li>
```

With a quote:
```html
<li><strong>Saturday 1 March 2025</strong> &ndash; Event name, Venue.
  <blockquote>Quote from the organiser or audience.
  <cite>&mdash; Their name</cite></blockquote>
</li>
```

---

### 🎷 Band members

**File:** [`the-band/index.html`](../../edit/main/the-band/index.html#L59)
*(link opens at the Band Members section, around line 59)*

The lineup is a single paragraph — just edit the names directly:

```html
<p><strong>Trombones:</strong> Name, Name, Name<br>
<strong>Trumpets:</strong> Name, Name, Name<br>
...
</p>
```

### 🈳 Vacancies

**File:** [`the-band/index.html`](../../edit/main/the-band/index.html#L67)
*(link opens at the Band Members section, around line 67)*

```html
<p>Current Vacancies: Trombone players</p>
```

---


### 🎤 Current repertoire

**File:** [`assets/thornbury-swing-band-current-repertoire.pdf`](../../blob/main/assets/thornbury-swing-band-current-repertoire.pdf)

**Referred to by:** [`the-band/index.html line 52`](../../blob/main/your-event/index.html#l51)

---


### 💷 Sound engineer fees

**File:** [`the-band/index.html`](../../edit/main/your-event/index.html#l78)
*(link opens at the Fees section, around line 78)*

```html
  <li><strong>Fees:</strong> ... own PA system and sound engineer
  ... usually around £200 although it can be up to £500 ....</li>
```
---

### 🎵 Practices

**File:** [`the-band/index.html`](../../edit/main/the-band/index.html#L70)
*(link opens at the Band Vacancies section, around line 70*

```html
<p>... Thursday evenings, 7:30&ndash;9:30 at Almondsbury  ...</p>
```
---

### 🏊 Music director

**File:** [`the-band/index.html`](../../edit/main/the-band/index.html#L37)
*(link opens at the Band section, around line 37*

```html
<p>... now under the direction of Chris White-Horne.</p>
```
---

### 🎸 Manager

**File:** [`assets/useful_information_for_event_organisers.pdf`](../../blob/main/assets/useful_information_for_event_organisers.pdf) 
p.2 `Liaison  
     Luigi Caludi will be your lead point of contact ... `

**File:** [`your-event/index.html`](../../edit/main/your-event/index.html#L35)
*(link opens at the Your Event section, around line 35, see also line 91*

```html
<p>... Luigi will be your ... contact. Luigi will liaise with you ...</p>
...
<p>... Luigi Caludi will be your lead point of contact ...</p>
```
---

### 📧 Email addresses and phone numbers


**File:** [`contact/index.html`](../../edit/main/contact/index.html#L35)
*(link opens at the Contact section, around line 35*

```html
<p>... thornburyswingband@gmail.com (twice)...</p>
```

**File:** [`assets/music-to-make-your-wedding-e28098swingu2019.pdf`](../../blob/main/assets/music-to-make-your-wedding-e28098swingu2019.pdf) 

```
bookings@thornburyswingband.com 07749 221415
```

**File:** [`assets/thornbury-swing-band-fundraising-with-a-swing.pdf`](../../blob/main/assets/thornbury-swing-band-fundraising-with-a-swing.pdf) 

```
bookings@thornburyswingband.com 
```

---

## 🗂️ File structure

```
index.html              – Home page
the-band/               – About the band & lineup
your-event/             – Booking information
events-coming-up/       – Upcoming events  
media/                  – Audio & video
gigs/                   – Past events      
contact/                – Contact & privacy policy
assets/                 – photos and PDFs
  style.css             – Shared styles
```

---

## 🚀 GitHub Pages setup (first time only)

1. Push this folder to a GitHub repository
2. Go to **Settings → Pages**
3. Set source to **main branch / root folder**
4. Site goes live at `https://<username>.github.io/<repo>/` ie in this case at `https://owen-kellie-smith.github.io/tsb-static/`

**Notes:**
- `.nojekyll` is present so GitHub Pages skips Jekyll processing
- Contact form uses a `mailto:` link (the WordPress form doesn't work in static sites)
- Media page has placeholder text — add SoundCloud/YouTube embed links when available

## DNS info

## Domain name management (info)
As a demo, [etcb.co.uk is registered (at names.co.uk), for a year until March 2027. names.co.uk DNS settings forward to Cloudflare.](https://www.whois.com/whois/thornburyswingband.co.uk) Cloudflare [has a CNAME for thornburyswingband.co.uk which is owen-kellie-smith.github.io](https://mxtoolbox.com/SuperTool.aspx?action=mx%3athornburyswingband.co.uk)&run=toolpage).  Github fowards to etcb-website/docs via this repo > Settings > Pages (Custom Domain) which created [a CNAME in docs](docs/CNAME).

```mermaid
flowchart TB

A[User Browser]

B[thornburyswingband.co.uk)<br>Domain registered at names.co.uk]

C[names.co.uk DNS<br>Nameservers → Cloudflare]

D[Cloudflare DNS<br>CNAME www → owen-kellie-smith.github.io]

E[GitHub Pages<br>Custom domain configured]

F[Repo:  tsb-static<br>/docs directory<br>Static site]

A --> B
B --> C
C --> D
D --> E
E --> F
```
