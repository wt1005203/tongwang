# SIM Lab site revision notes

This ZIP contains the revised Hugo source for the Systems and Interactions of Microbiomes Lab (SIM Lab) website.

## Latest changes in this version

- Updated individual member pages so they now use a single visible section heading: `Profile`.
- Removed the old visible `Profile Details` heading.
- Removed duplicate placeholder Markdown `## Profile` sections from student and Marble pages.
- Replaced the visible label `Current Research Projects` with `Research Interests`.
- Added optional member fields for `Contact` and `Contact me about`.
- Updated Fei Wang’s profile so her structured profile information appears on the profile page.
- Kept Marble’s photo fix from the previous version: `static/img/Marble_profile.jpg` is a square crop, and circular thumbnails use `object-fit: cover`.
- Kept the sidebar/profile logo replacement: `static/img/SIM_Lab_logo.png`.

## Where to edit common parts later

- Sidebar logo: replace `static/img/SIM_Lab_logo.png` with a new image using the same filename, or change `profileImage` in `config.toml`.
- Lab name, email, subtitle, and main site settings: edit `config.toml`.
- Homepage About text: edit `content/_index.md`.
- Research page: edit `content/research/_index.md`.
- Members page intro: edit `content/members/_index.md`.
- Member list card layout: edit `layouts/partials/membersSummary.html`.
- Individual member page layout: edit `layouts/members/single.html`.
- Website styling: edit `static/css/resume-override.css`.

## Individual member files

Edit these Markdown files to revise each member’s profile:

```text
content/members/tong-wang.md
content/members/fei-wang.md
content/members/qiwen-ena-chen.md
content/members/jocelyn-yang.md
content/members/marble.md
```

## Suggested member-profile editing pattern

Each member file begins with front matter between two `---` lines. To update a member, edit values such as:

```yaml
title: "Name"
role: "Role"
image: "img/photo-file.jpg"
department_program: "Department or program"
research_interests: "Research interest 1; research interest 2"
joined: "Fall 2026"
email: "name@purdue.edu"
contact: "Alternative non-email contact text"
contact_me_about: "Topics this member welcomes questions about"
hobbies: "Hobby 1, hobby 2, and hobby 3"
description: "Short one-sentence summary for the Members page card."
```

Use `email` for an email address. Use `contact` only when the contact information is not an email address. The profile-page template displays `email` as `Contact` with a mailto link.

The current structured profile fields are displayed by:

```text
layouts/members/single.html
```

## Build note

I verified file references and ZIP integrity in the sandbox. Hugo is not installed in the sandbox, so I could not run a full local Hugo build here.

## Sidebar logo scaling fix

The sidebar logo display is controlled by CSS in:

```text
static/css/resume-override.css
```

The latest override removes the original resume theme's extra portrait border and padding around the sidebar image and scales the logo to `14rem`, so the circular SIM Lab logo fills the sidebar image area more fully.

To adjust the logo size later, edit these values in `static/css/resume-override.css`:

```css
#sideNav .navbar-brand .img-profile {
  width: 14rem !important;
  height: 14rem !important;
  max-width: 14rem !important;
  max-height: 14rem !important;
}
```

For a slightly smaller logo, try `13rem`; for a larger logo, try `14.5rem` or `15rem`, but keep it below the sidebar width of about `17rem`.

## 2026-07-30 update: Former members link

- The homepage Members section now shows a simple gold text link labeled **Former members** instead of a blue button.
- The link points to `members/#former-members`, where the full former-members table is shown.
- The standalone Members page heading now uses **Former members** instead of **Alumni**.
- Main files changed:
  - `layouts/partials/sectionSummary.html`
  - `layouts/_default/section.html`
  - `static/css/resume-override.css`
- Former-member data are still edited in `content/members/_index.md` under the `alumni:` front matter field.
