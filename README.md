# Netflix Landing Page

A Netflix-inspired landing page created using **HTML and CSS**. The project recreates the main sections of a Netflix-style homepage, including the navigation bar, hero section, trending movies, reasons to join, FAQ section, email signup forms, and footer.

## Features

* Netflix-style navigation bar
* Netflix logo with language selection
* Sign In button
* Hero section with background image
* Main heading and membership information
* Email signup form
* Trending movies section
* Movie ranking numbers
* Movie hover effect
* Next button for the movie slider
* "More reasons to join" feature cards
* Frequently Asked Questions section
* Expandable FAQ items using HTML `<details>` and `<summary>`
* FAQ `+` and `×` indicators
* Bottom email signup section
* Footer with useful links
* English and Hindi language options
* Responsive-friendly CSS structure

## Technologies Used

* HTML5
* CSS3

No JavaScript or external frameworks are required for the basic page structure and interactions.

## Project Structure

```text
Netflix/
│
├── index.html
├── styless.css
├── hero.jpg
├── j1.webp
└── README.md
```

## Main Sections

### 1. Navigation Bar

The navigation bar contains:

* Netflix logo
* Language selection
* Sign In button

The navigation is positioned over the hero section so that the background image continues behind the navbar.

### 2. Hero Section

The hero section contains:

* Main heading: "Unlimited movies, shows, and more"
* Starting price information
* Membership message
* Email input
* Get Started button

The section uses a background image with a dark gradient overlay to make the text easier to read.

### 3. Trending Now

The Trending Now section displays movie cards with ranking numbers.

Each movie card contains:

* Ranking number
* Movie poster
* Hover effect

The movie cards are arranged using CSS Flexbox.

### 4. More Reasons to Join

This section contains four feature cards:

* Enjoy on your TV
* Download your shows to watch offline
* Watch everywhere
* Create profiles for kids

CSS Grid is used to arrange the cards into four columns.

```css
grid-template-columns: repeat(4, 1fr);
```

### 5. FAQ Section

The FAQ section contains frequently asked questions using the HTML `<details>` and `<summary>` elements.

Users can click a question to expand or collapse the answer.

The CSS changes the indicator from `+` to `×` when an FAQ is open.

```css
.faq-item summary::after {
    content: "+";
}

.faq-item details[open] summary::after {
    content: "×";
}
```

### 6. Bottom Signup

Another email signup form is provided near the bottom of the page so users can enter their email address.

### 7. Footer

The footer contains:

* Contact information
* FAQ
* Help Centre
* Account
* Media Centre
* Investor Relations
* Jobs
* Ways to Watch
* Terms of Use
* Privacy
* Contact Us
* Speed Test
* Legal Notices
* Only on Netflix
* Language selection
* Country information
* reCAPTCHA information

## CSS Concepts Used

This project demonstrates several important CSS concepts:

### Flexbox

Used for navigation, forms, and movie cards.
css
display: flex;
align-items: center;
justify-content: space-between;


### CSS Grid

Used for the feature cards and footer links.

css
display: grid;
grid-template-columns: repeat(4, 1fr);
### Positioning

The navbar uses absolute positioning so it can appear over the hero background.

css
position: absolute;
top: 0;
left: 0;


### Background Images

The hero section uses a background image combined with a gradient overlay.

css
background-image:
    linear-gradient(...),
    url("./hero.jpg");

### Hover Effects

Buttons and movie posters change appearance when the user moves the mouse over them.

css
.movie-card img:hover {
    transform: scale(1.03);
}
```

### HTML Details Element

The FAQ uses native HTML functionality without JavaScript.

```html
<details>
    <summary>What is Netflix?</summary>
    <p>Netflix is a streaming service...</p>
</details>
```

## How to Run

1. Download or clone the project.
2. Keep `index.html` and `styless.css` in the same folder.
3. Place the hero background image in the same folder if using a local image.
4. Open `index.html` in a web browser.

You can also use **VS Code with the Live Server extension** to run the project locally.

## Notes

This is a **Netflix-inspired frontend project** created for learning and practice. It does not provide actual Netflix streaming, membership, authentication, or account functionality.

The email forms are frontend-only and do not currently submit user information to a backend.

## Future Improvements

Possible improvements include:

* Add responsive layouts for mobile and tablet screens
* Add JavaScript functionality to the movie slider
* Add working Sign In functionality
* Add form validation
* Add a backend for user registration
* Add more movie cards
* Add animations and transitions
* Improve accessibility
* Add a mobile navigation menu
* Make the language selector functional

## Author

Created as a frontend development practice project using HTML and CSS.
