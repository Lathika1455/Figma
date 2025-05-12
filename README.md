# Ex09 Event Registration Web Application
## Date:12-05-2025

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```
Home page:
<style>
  .events-container {
    display: flex;
    flex-direction: column;
    position: relative;
    min-height: 2162px;
    width: 100%;
    align-items: end;
    padding: 378px 70px 1213px;
  }
  .background-image {
    position: absolute;
    inset: 0;
    height: 100%;
    width: 100%;
    object-fit: cover;
    object-position: center;
  }
  .content-wrapper {
    position: relative;
    display: flex;
    margin-bottom: -243px;
    width: 100%;
    max-width: 1106px;
    gap: 20px;
    flex-wrap: wrap;
    justify-content: space-between;
  }
  .navigation-container {
    display: flex;
    flex-direction: column;
  }
  .event-title {
    align-self: center;
  }
  .login-button {
    background-color: rgba(155, 57, 30, 0.23);
    white-space: nowrap;
    margin: 115px 26px 0 0;
    padding: 35px 70px;
    cursor: pointer;
  }
  .register-button {
    background-color: rgba(155, 57, 30, 0.33);
    white-space: nowrap;
    margin: 107px 0 0 26px;
    padding: 15px 70px 33px;
    cursor: pointer;
  }
  .decorative-icon {
    aspect-ratio: 0.09;
    object-fit: contain;
    object-position: center;
    width: 37px;
    margin: auto 0;
  }
  @media (max-width: 991px) {
    .events-container {
      max-width: 100%;
      font-size: 40px;
      padding: 100px 0 100px 20px;
    }
    .content-wrapper {
      max-width: 100%;
      margin-bottom: 10px;
      font-size: 40px;
    }
    .navigation-container {
      max-width: 100%;
      font-size: 40px;
    }
    .event-title {
      max-width: 100%;
      font-size: 40px;
    }
    .login-button {
      font-size: 40px;
      max-width: 100%;
      white-space: initial;
      margin: 40px 10px 0 0;
      padding: 0 20px;
    }
    .register-button {
      font-size: 40px;
      max-width: 100%;
      margin-top: 40px;
      white-space: initial;
      padding: 0 20px;
    }
    .decorative-icon {
      display: none;
    }
  }
  .visually-hidden {
    position: absolute;
    width: 1px;
    height: 1px;
    padding: 0;
    margin: -1px;
    overflow: hidden;
    clip: rect(0, 0, 0, 0);
    border: 0;
  }
</style>

<div class="events-container">
  <img
    loading="lazy"
    src="https://cdn.builder.io/api/v1/image/assets/TEMP/30d6f593ef141370d80ff69b5216b9498cf1f3ca450a301a4c63afb410c3d9ce?placeholderIfAbsent=true&apiKey=cd36f702698e422ab5e3663a8839d2d4"
    class="background-image"
    alt="Cultural events background"
  />
  <div class="content-wrapper">
    <div class="navigation-container">
      <div class="event-title">CULTURAL EVENTS</div>
      <button class="login-button" tabindex="0">LOGIN</button>
      <button class="register-button" tabindex="0">REGISTER</button>
    </div>
    <img
      loading="lazy"
      src="https://cdn.builder.io/api/v1/image/assets/TEMP/d9e8d7d4f41eaba75cb475130dea3591aca148d00e5a46c721b9f0827138a093?placeholderIfAbsent=true&apiKey=cd36f702698e422ab5e3663a8839d2d4"
      class="decorative-icon"
      alt=""
    />
  </div>
</div>

Events pages:

<style>
  .cultural-events-container {
    background-color: rgba(255, 255, 255, 1);
    display: flex;
    flex-direction: column;
    overflow: hidden;
    color: rgba(0, 0, 0, 1);
    font: 400 64px Inter, sans-serif;
  }

  .events-wrapper {
    display: flex;
    flex-direction: column;
    position: relative;
    min-height: 2162px;
    width: 100%;
    align-items: center;
    padding: 343px 80px;
  }

  .background-image {
    position: absolute;
    inset: 0;
    height: 100%;
    width: 100%;
    object-fit: cover;
    object-position: center;
  }

  .main-title {
    position: relative;
  }

  .event-item {
    position: relative;
    display: flex;
    gap: 40px 47px;
    flex-wrap: wrap;
  }

  .event-icon {
    aspect-ratio: 1.07;
    object-fit: contain;
    object-position: center;
    width: 96px;
  }

  .event-title {
    align-self: start;
    margin-top: 12px;
    flex-grow: 1;
    flex-basis: auto;
  }

  .dancing-section {
    align-self: start;
    margin-top: 220px;
    white-space: nowrap;
  }

  .music-section {
    margin-top: 128px;
    width: 695px;
    max-width: 100%;
  }

  .music-title {
    width: 533px;
  }

  .photo-section {
    width: 790px;
    max-width: 100%;
    margin: 143px 0 0 18px;
  }

  .photo-title {
    width: 628px;
  }

  .art-section {
    align-self: end;
    margin-top: 146px;
    width: 100%;
    max-width: 982px;
    gap: 40px 50px;
  }

  .art-title {
    width: 817px;
  }

  .poetry-section {
    margin-top: 108px;
    width: 610px;
    max-width: 100%;
    gap: 40px 57px;
  }

  .poetry-title {
    margin-top: 13px;
    width: 437px;
  }

  .wood-section {
    width: 574px;
    max-width: 100%;
    gap: 40px 63px;
    white-space: nowrap;
    margin: 144px 0 -76px;
  }

  .wood-title {
    width: 394px;
  }

  @media (max-width: 991px) {
    .cultural-events-container {
      font-size: 40px;
    }

    .events-wrapper {
      max-width: 100%;
      padding: 100px 20px;
    }

    .main-title {
      max-width: 100%;
    }

    .dancing-section {
      margin: 40px 0 0 3px;
      white-space: initial;
    }

    .music-section {
      margin-top: 40px;
    }

    .music-title {
      max-width: 100%;
    }

    .photo-section {
      margin-top: 40px;
    }

    .photo-title {
      max-width: 100%;
    }

    .art-section {
      max-width: 100%;
      margin-top: 40px;
    }

    .art-title {
      max-width: 100%;
    }

    .poetry-section {
      margin-top: 40px;
    }

    .poetry-title {
      max-width: 100%;
    }

    .wood-section {
      white-space: initial;
      margin: 40px 0 10px;
    }
  }
</style>

<div class="cultural-events-container">
  <div class="events-wrapper">
    <img class="background-image" src="https://cdn.builder.io/api/v1/image/assets/TEMP/62b305aeb0b852f5abf138336df8bf536f5ca2a55a2f7af9baddff59d961ea43?placeholderIfAbsent=true&apiKey=cd36f702698e422ab5e3663a8839d2d4" alt="Cultural events background" loading="lazy" />
    <h1 class="main-title">Cultural Events</h1>

    <div class="event-item dancing-section">
      <img class="event-icon" src="https://cdn.builder.io/api/v1/image/assets/TEMP/00778fa76dcb237001cc6849fc44e99458b9bf9ee66b924743788d8771e71fb7?placeholderIfAbsent=true&apiKey=cd36f702698e422ab5e3663a8839d2d4" alt="Dancing event icon" loading="lazy" />
      <h2 class="event-title">Dancing</h2>
    </div>

    <div class="event-item music-section">
      <img class="event-icon" src="https://cdn.builder.io/api/v1/image/assets/TEMP/4dcc2a17b1b7eea034123ddf5b57e00979b5b4df386c0a3b25a9d082582373ad?placeholderIfAbsent=true&apiKey=cd36f702698e422ab5e3663a8839d2d4" alt="Music and singing event icon" loading="lazy" />
      <h2 class="event-title music-title">Music and Singing</h2>
    </div>

    <div class="event-item photo-section">
      <img class="event-icon" src="https://cdn.builder.io/api/v1/image/assets/TEMP/f87db3db1f8f97478bfa82019ad0f906b66ba3405bede1bb1a2d6fc2cc2b83a8?placeholderIfAbsent=true&apiKey=cd36f702698e422ab5e3663a8839d2d4" alt="Photography and film event icon" loading="lazy" />
      <h2 class="event-title photo-title">Photography and film</h2>
    </div>

    <div class="event-item art-section">
      <img class="event-icon" src="https://cdn.builder.io/api/v1/image/assets/TEMP/12f4fdd4020bb46cba69ffce4c31e0489d6a7a2454d4a617175ea452627391b3?placeholderIfAbsent=true&apiKey=cd36f702698e422ab5e3663a8839d2d4" alt="Art and crafts event icon" loading="lazy" />
      <h2 class="event-title art-title">Drawing,Painting,and crafts</h2>
    </div>

    <div class="event-item poetry-section">
      <img class="event-icon" src="https://cdn.builder.io/api/v1/image/assets/TEMP/b1da57b0a4d77c55e94fa4ec3cbe5cae01693faa0ee20b077c8b6b752f040247?placeholderIfAbsent=true&apiKey=cd36f702698e422ab5e3663a8839d2d4" alt="Poetry event icon" loading="lazy" />
      <h2 class="event-title poetry-title">Poetry in parks</h2>
    </div>

    <div class="event-item wood-section">
      <img class="event-icon" src="https://cdn.builder.io/api/v1/image/assets/TEMP/dc98b645c0e94ba439887e0531c94249e0ce3d7e4f8d55ba7aca0d7ca73a944d?placeholderIfAbsent=true&apiKey=cd36f702698e422ab5e3663a8839d2d4" alt="Woodworking event icon" loading="lazy" />
      <h2 class="event-title wood-title">Woodworking</h2>
    </div>
  </div>
</div>

Events Registration:

<style>
.registration-container {
  background-color: #fff;
  display: flex;
  flex-direction: column;
  overflow: hidden;
}

.registration-wrapper {
  display: flex;
  flex-direction: column;
  min-height: 2162px;
  width: 100%;
  align-items: center;
  padding: 290px 70px 99px;
}

.background-image {
  position: absolute;
  inset: 0;
  height: 100%;
  width: 100%;
  object-fit: cover;
  object-position: center;
}

.form-container {
  position: relative;
  margin-left: 18px;
  width: 100%;
  max-width: 1121px;
}

.form-layout {
  gap: 20px;
  display: flex;
}

.divider-column {
  display: flex;
  flex-direction: column;
  line-height: normal;
  width: 50%;
  margin-left: 0;
}

.divider-line {
  background-color: #d9d9d9;
  position: relative;
  display: flex;
  width: 1109px;
  max-width: 100%;
  height: 1px;
  align-self: stretch;
  margin: auto -1098px auto 0;
}

.form-fields-column {
  display: flex;
  flex-direction: column;
  line-height: normal;
  width: 50%;
  margin-left: 20px;
}

.form-content {
  position: relative;
  display: flex;
  flex-grow: 1;
  flex-direction: column;
  color: #000;
  font: 400 64px Inter, sans-serif;
}

.form-title {
  align-self: center;
}

.form-field {
  background-color: #d9d9d9;
  margin-top: 82px;
  padding: 18px 70px;
}

.form-field-name {
  margin-top: 153px;
  padding: 29px 70px 6px;
}

.form-field-register {
  padding: 9px 70px 26px;
}

.form-field-department {
  white-space: nowrap;
}

.form-field-contact {
  padding: 12px 70px 23px;
  margin-top: 77px;
}

.form-field-email {
  margin-top: 73px;
}

.form-field-events {
  margin-top: 84px;
  padding: 0 70px 35px;
}

.submit-button {
  background-color: #d9d9d9;
  white-space: nowrap;
  margin: 101px 36px 0 18px;
  padding: 60px 70px;
}

.visually-hidden {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}

@media (max-width: 991px) {
  .registration-wrapper {
    max-width: 100%;
    padding: 100px 20px 0;
  }

  .form-container {
    max-width: 100%;
  }

  .form-layout {
    flex-direction: column;
    align-items: stretch;
    gap: 0;
  }

  .divider-column {
    width: 100%;
  }

  .divider-line {
    margin-top: 40px;
  }

  .form-fields-column {
    width: 100%;
  }

  .form-content {
    max-width: 100%;
    font-size: 40px;
  }

  .form-title {
    max-width: 100%;
    font-size: 40px;
  }

  .form-field {
    font-size: 40px;
    max-width: 100%;
    margin-top: 40px;
    padding: 0 20px;
  }

  .form-field-name {
    margin-top: 40px;
  }

  .form-field-department {
    white-space: initial;
  }

  .submit-button {
    font-size: 40px;
    max-width: 100%;
    white-space: initial;
    margin: 40px 10px 0 0;
    padding: 0 20px;
  }
}
</style>

<div class="registration-container">
  <div class="registration-wrapper">
    <img
      loading="lazy"
      src="https://cdn.builder.io/api/v1/image/assets/TEMP/b0f20f733a72ba5f64be5b226ce9d26004a7ed9c5ba99cf424fabde76a899b98?placeholderIfAbsent=true&apiKey=cd36f702698e422ab5e3663a8839d2d4"
      class="background-image"
      alt=""
    />
    <form class="form-container">
      <div class="form-layout">
        <div class="divider-column">
          <div class="divider-line"></div>
        </div>
        <div class="form-fields-column">
          <div class="form-content">
            <h1 class="form-title">Event Registration Form</h1>
            
            <label for="fullName" class="visually-hidden">Full Name</label>
            <input type="text" id="fullName" class="form-field form-field-name" aria-label="Full Name" required />
            
            <label for="genderAge" class="visually-hidden">Gender and Age</label>
            <input type="text" id="genderAge" class="form-field" aria-label="Gender and Age" required />
            
            <label for="regNumber" class="visually-hidden">Register Number</label>
            <input type="text" id="regNumber" class="form-field form-field-register" aria-label="Register Number" required />
            
            <label for="department" class="visually-hidden">Department</label>
            <input type="text" id="department" class="form-field form-field-department" aria-label="Department" required />
            
            <label for="mobile" class="visually-hidden">Mobile Number</label>
            <input type="tel" id="mobile" class="form-field form-field-contact" aria-label="Mobile Number" required />
            
            <label for="email" class="visually-hidden">Email ID</label>
            <input type="email" id="email" class="form-field form-field-email form-field-contact" aria-label="Email ID" required />
            
            <label for="events" class="visually-hidden">Events to Register</label>
            <select id="events" class="form-field form-field-events" aria-label="Events to Register" required>
              <option value="">Select Events</option>
            </select>
            
            <button type="submit" class="submit-button">REGISTER</button>
          </div>
        </div>
      </div>
    </form>
  </div>
</div>

Contact page:

<style>
.thank-you-container {
  background-color: #fff;
  display: flex;
  flex-direction: column;
  overflow: hidden;
  color: #000;
  font: 400 64px Inter, sans-serif;
}

.content-wrapper {
  display: flex;
  flex-direction: column;
  position: relative;
  min-height: 2162px;
  width: 100%;
  align-items: center;
  padding: 444px 80px 757px;
}

.background-image {
  position: absolute;
  inset: 0;
  height: 100%;
  width: 100%;
  object-fit: cover;
  object-position: center;
}

.text-content {
  position: relative;
  display: flex;
  margin-bottom: -151px;
  width: 100%;
  max-width: 1225px;
  flex-direction: column;
  align-items: center;
}

.heading {
  font-size: 64px;
  font-weight: 400;
}

.message {
  align-self: stretch;
  margin: 66px 22px 0;
}

.contact-heading {
  margin-top: 127px;
}

.email-label {
  margin-top: 32px;
}

.email-address {
  align-self: stretch;
  margin-top: 27px;
}

.phone-label {
  margin: 27px 0 0 18px;
}

.phone-number {
  margin-top: 66px;
}

@media (max-width: 991px) {
  .thank-you-container {
    font-size: 40px;
  }

  .content-wrapper {
    max-width: 100%;
    padding: 100px 20px;
  }

  .text-content {
    max-width: 100%;
    margin-bottom: 10px;
  }

  .heading,
  .message,
  .contact-heading,
  .email-label,
  .email-address,
  .phone-label,
  .phone-number {
    font-size: 40px;
  }

  .message {
    margin: 40px 10px 0 0;
  }

  .contact-heading {
    margin-top: 40px;
  }

  .phone-number {
    margin-top: 40px;
  }
}

.visually-hidden {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
</style>

<div class="thank-you-container">
  <div class="content-wrapper">
    <img
      loading="lazy"
      src="https://cdn.builder.io/api/v1/image/assets/TEMP/9bb2bd29fef28781394ac399e3cf8f194aff39d2ff36c951c2f0760bcad573a2?placeholderIfAbsent=true&apiKey=cd36f702698e422ab5e3663a8839d2d4"
      alt=""
      class="background-image"
    />
    <div class="text-content">
      <h1 class="heading">THANK YOU</h1>
      <p class="message">
        We are all waiting for your participation
        <br />
        in the cultural Events.
      </p>
      <h2 class="contact-heading">Contact us:</h2>
      <h3 class="email-label">Email ID:</h3>
      <p class="email-address">Saveethaengineeringcollege@gmail.com</p>
      <h3 class="phone-label">Mobile Number:</h3>
      <p class="phone-number">7010637084</p>
    </div>
  </div>
</div>
```

## OUTPUT:

![Screenshot 2025-05-12 213837](https://github.com/user-attachments/assets/7f9aad6d-a5ec-4c84-8768-ee792405a251)

## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
