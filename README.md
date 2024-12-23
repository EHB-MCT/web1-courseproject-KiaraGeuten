# Alexander Hamilton's CV

## Project Overview

Welcome to Alexander Hamilton's CV! A project I built for school. In here you can find everything you need for hiring him.
From debating and writing essays to public speaking he can do it all.

## Features

- Short description
- Skills
- Hire page
- Contact form

## Technologies Used

- HTML
- CSS

## Acknowledgments

Thanks to Lukas Van Heddegem for the navigation and contact form:

- HTML:

````<nav>
      <a href="index.html">
        <img src="images/Hamilton-Logo.png" alt: "logo Hamilton"/>
      </a>
      <h1>Alexander Hamilton</h1>
      <input id="header-collapsible" class="toggle" type="checkbox" />
      <label for="header-collapsible" class="lbl-toggle">
        <div class="l1 line"></div>
        <div class="l2 line"></div>
        <div class="l3 line"></div>
      </label>
      <div class="nav-buttons collapsible-content">
        <ul>
          <li><a href="#">Experience</a></li>
          <li><a href="skills.html">Skills</a></li>
          <li><a href="hire.html">Hire me</a></li>
        </ul>
        <img src="images/Hamilton-Logo.png" alt="logo Hamilton" />
      </div>
    </nav> ```

    ```<form id="ContactForm" class="isolate">
          <div class="contact_fields">
            <div class="field">
              <input class="field_input" type="text" placeholder="Name" />
              <label class="field_label">Name</label>
            </div>
            <div class="field">
              <input type="email" class="field_input" placeholder="E-mail" />
              <label class="field_label">E-mail</label>
            </div>
          </div>
          <div class="field">
            <input type="tel" class="field_input" placeholder="Phone number" />
            <label class="field_label">Phone number</label>
          </div>
          <div class="field">
            <textarea
              rows="10"
              class="field_input"
              placeholder="Comment"
            ></textarea>
            <label class="form_label field_label">Comment</label>
          </div>
          <div class="contact_button">
            <button type="submit" class="button">Send</button>
          </div>
        </form>```

- CSS:

nav {
display: flex;
flex-direction: row;
justify-content: space-between;
background-color: #8b641f;
align-items: center;
padding: 10px 20px 10px;
box-sizing: border-box;
position: sticky;
top: 0;
z-index: 1;

a {
img {
width: 100px;
}
}
h1 {
font-size: 50px;
margin: 0;
width: 100%;
text-align: center;
padding-left: 100px;
}
.toggle {
display: none;
}
.nav-buttons {
ul {
display: flex;
flex-direction: row;
gap: 30px;
padding-right: 12px;

      li {
        display: inline;

        a {
          text-decoration: none;
          color: white;
          font-size: 20px;
          text-wrap: nowrap;
        }
      }
    }
    img {
      display: none;
    }

}
}

.contact {
display: grid;
grid-template-columns: 6fr 8fr;
grid-template-rows: repeat(2, minmax(100px, auto));
padding: 30px;
margin-top: 0;
box-sizing: border-box;

.contacttext {
grid-column: 1/3;
}
.imagecontact {
grid-column: 1/2;
img {
width: 700px;
}
}
.contacttext h2 {
margin-bottom: 10px;
}
gap: 1rem;
.imagecontact {
width: 100%;

    img {
      width: 100%;
    }

}

form {
display: flex;
flex-direction: column;
grid-column: 2/3;
gap: 0.8rem;
max-width: 700px;
margin-bottom: 0;

    .contact_fields {
      display: flex;
      flex-direction: row;
      gap: 0.8rem;
    }
    .field {
      position: relative;
      flex: 1 1 50%;
    }

    label {
      position: absolute;
      left: 8px;
      top: 8px;
      color: grey;
      pointer-events: none;
    }
    textarea,
    input {
      padding: 8px;
      width: 100%;
      box-sizing: border-box;
      border-radius: 6px;
      border: 0;
      appearance: none;
      &::placeholder {
        color: transparent;
      }
    }
    textarea:not(:placeholder-shown) + label,
    input:not(:placeholder-shown) + label {
      font-size: 8px;
      top: 4px;
      left: 10px;
    }

    textarea:not(:placeholder-shown),
    input:not(:placeholder-shown) {
      border-color: black;
      padding: 12px 6px 4px 10px;
    }

    textarea:focus-visible,
    input:focus-visible {
      border-color: black;
      padding: 12px 6px 4px 10px;

      & + label {
        font-size: 8px;
        top: 4px;
        left: 10px;
      }
    }

}
}
````
