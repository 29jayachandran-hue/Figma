# Ex09 Event Registration Web Application
## Date:08.10.2025

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
globals.css
```
@import url("https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css");
* {
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
html,
body {
  margin: 0px;
  height: 100%;
}
/* a blue color as a generic focus style */
button:focus-visible {
  outline: 2px solid #4a90e2 !important;
  outline: -webkit-focus-ring-color auto 5px !important;
}
a {
  text-decoration: none;
}
```

style.css
```
/* --- Screen 1: android-compact-1.png (Initial/Default Layout) --- */
.android-compact {
  /* Common container styles */
  background-size: cover;
  background-position: 50% 50%;
  width: 100%;
  min-width: 412px;
  min-height: 820px;
}

/* Base styles for the first screen (using android-compact-1.png) */
.android-compact:nth-of-type(1) { /* Placeholder for first instance */
  background-image: url(./img/android-compact-1.png);
  position: relative;
}

.android-compact .logo {
  position: absolute;
  top: 35px;
  left: 3px;
  width: 409px;
  height: 62px;
  aspect-ratio: 6.65;
  object-fit: cover;
}

.android-compact .SPORTS-DAY-EVENT {
  position: absolute;
  top: 151px;
  left: 45px;
  font-family: "Jomhuria-Regular", Helvetica;
  font-weight: 400;
  color: #000000;
  font-size: 110px;
  text-align: center;
  letter-spacing: 0;
  line-height: 70px;
}

/* Separate positioning for two orange rectangles/buttons */
.android-compact .rectangle {
  top: 414px;
  position: absolute;
  left: 100px;
  width: 212px;
  height: 64px;
  background-color: #ffa500;
}

.android-compact .div {
  top: 543px;
  position: absolute;
  left: 100px;
  width: 212px;
  height: 64px;
  background-color: #ffa500;
}

/* Text wrappers for the two buttons/rectangles */
.android-compact .text-wrapper {
  position: absolute;
  top: 414px;
  left: 100px;
  width: 212px;
  height: 64px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: "Jaldi-Bold", Helvetica;
  font-weight: 700;
  color: #000000;
  font-size: 48px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-2 {
  position: absolute;
  top: 543px;
  left: 100px;
  width: 212px;
  height: 64px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: "Jaldi-Bold", Helvetica;
  font-weight: 700;
  color: #000000;
  font-size: 48px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

/* --- Screen 2: android-compact-2.png (Flexbox Layout) --- */
.android-compact:nth-of-type(2) { /* Placeholder for second instance */
  background-image: url(./img/android-compact-2.png);
  /* Overrides for this screen */
  display: flex;
  flex-direction: column;
  gap: 6px;
}

/* Unique text styles for Screen 2 */
.android-compact:nth-of-type(2) .text-wrapper {
  /* This overrides .android-compact .text-wrapper from screen 1 */
  display: flex;
  align-items: center;
  justify-content: center;
  margin-left: 56px;
  width: 300px;
  height: 119px;
  margin-top: 25px;
  font-family: "Instrument Sans-Bold", Helvetica;
  font-weight: 700;
  color: #ff0000;
  font-size: 40px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .cricket-football {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-left: 49px;
  width: 313px;
  height: 520px;
  font-family: "Inknut Antiqua-Bold", Helvetica;
  font-weight: 700;
  color: #000000;
  font-size: 40px;
  letter-spacing: 0;
  line-height: 65px;
}

/* --- Screen 3: android-compact-3.png (List/Menu Layout) --- */
.android-compact:nth-of-type(3) { /* Placeholder for third instance */
  background-image: url(./img/android-compact-3.png);
  position: relative;
}

/* Unique text styles for Screen 3 */
.android-compact:nth-of-type(3) .text-wrapper {
  /* This overrides all previous text-wrapper styles */
  position: absolute;
  top: 57px;
  left: 35px;
  width: 341px;
  height: 68px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: "Instrument Sans-Bold", Helvetica;
  font-weight: 700;
  color: #0033ff;
  font-size: 36px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

/* Multiple green rectangles (menu items/buttons) */
.android-compact .rectangle {
  top: 150px;
  left: calc(50.00% - 171px);
  position: absolute;
  width: 341px;
  height: 48px;
  background-color: #63bf1d;
}

.android-compact .div {
  top: 442px;
  left: 35px;
  position: absolute;
  width: 341px;
  height: 48px;
  background-color: #63bf1d;
}

.android-compact .rectangle-2 {
  top: 369px;
  left: 35px;
  position: absolute;
  width: 341px;
  height: 48px;
  background-color: #63bf1d;
}

.android-compact .rectangle-3 {
  top: 296px;
  left: 35px;
  position: absolute;
  width: 341px;
  height: 48px;
  background-color: #63bf1d;
}

.android-compact .rectangle-4 {
  top: 223px;
  left: 35px;
  position: absolute;
  width: 341px;
  height: 48px;
  background-color: #63bf1d;
}

.android-compact .rectangle-5 {
  top: 515px;
  left: 35px;
  position: absolute;
  width: 341px;
  height: 48px;
  background-color: #63bf1d;
}

.android-compact .rectangle-6 {
  top: 588px;
  left: 35px;
  position: absolute;
  width: 341px;
  height: 48px;
  background-color: #63bf1d;
}

/* Text wrappers for the menu items/buttons */
.android-compact .text-wrapper-2 {
  position: absolute;
  top: 296px;
  left: calc(50.00% - 171px);
  width: 341px;
  height: 48px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #ffffff;
  font-size: 32px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-3 {
  position: absolute;
  top: 150px;
  left: calc(50.00% - 171px);
  width: 341px;
  height: 48px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #ffffff;
  font-size: 32px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-4 {
  position: absolute;
  top: 588px;
  left: calc(50.00% - 170px);
  width: 341px;
  height: 48px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #ffffff;
  font-size: 32px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-5 {
  position: absolute;
  top: 515px;
  left: calc(50.00% - 171px);
  width: 341px;
  height: 48px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #ffffff;
  font-size: 32px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-6 {
  position: absolute;
  top: 442px;
  left: calc(50.00% - 170px);
  width: 341px;
  height: 48px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #ffffff;
  font-size: 32px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-7 {
  position: absolute;
  top: 369px;
  left: calc(50.00% - 171px);
  width: 341px;
  height: 48px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #ffffff;
  font-size: 32px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-8 {
  position: absolute;
  top: 223px;
  left: calc(50.00% - 171px);
  width: 341px;
  height: 48px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #ffffff;
  font-size: 32px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

/* --- Screen 4: android-compact-4.png (Thank You/Flex Layout) --- */
.android-compact:nth-of-type(4) { /* Placeholder for fourth instance */
  background-image: url(./img/android-compact-4.png);
  /* Overrides for this screen */
  display: flex;
  flex-direction: column;
}

/* Unique element styles for Screen 4 (Note: logo, text-wrapper, div, and text-wrapper-2/3 all overwrite previous non-absolute styles) */
.android-compact:nth-of-type(4) .logo {
  margin-left: 3px;
  width: 409px;
  height: 62px;
  margin-top: 35px;
  aspect-ratio: 6.65;
  object-fit: cover;
}

.android-compact .thank-you {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-left: 75px;
  width: 262px;
  height: 74px;
  margin-top: 67px;
  font-family: "Inknut Antiqua-Bold", Helvetica;
  font-weight: 700;
  color: #000000;
  font-size: 32px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact:nth-of-type(4) .text-wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-left: 43px;
  width: 333px;
  height: 194px;
  font-family: "Inika-Bold", Helvetica;
  font-weight: 700;
  color: #000000;
  font-size: 24px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact:nth-of-type(4) .div {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-left: 55px;
  width: 309px;
  height: 65px;
  font-family: "Inika-Bold", Helvetica;
  font-weight: 700;
  color: #000000;
  font-size: 32px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact:nth-of-type(4) .text-wrapper-2 {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-left: 81px;
  width: 258px;
  height: 48px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #000000;
  font-size: 24px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-3 {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-left: 55px;
  width: 335px;
  height: 48px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #000000;
  font-size: 24px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}
```

page 1
```
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="android-compact">
      <img class="logo" src="img/logo.png" />
      <div class="SPORTS-DAY-EVENT">SPORTS DAY<br />EVENT</div>
      <div class="rectangle"></div>
      <div class="div"></div>
      <div class="text-wrapper">LOGIN</div>
      <div class="text-wrapper-2">REGISTER</div>
    </div>
  </body>
</html>
```

page 2
```
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="android-compact">
      <div class="text-wrapper">EVENTS</div>
      <div class="cricket-football">
        Cricket<br />Football<br />Badminton<br />Volleyball<br />Basketball<br />100 mtr<br />400mtr<br />Sprints
      </div>
    </div>
  </body>
</html>
```

page 3
```
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="android-compact">
      <div class="text-wrapper">Registration Form</div>
      <div class="rectangle"></div>
      <div class="div"></div>
      <div class="rectangle-2"></div>
      <div class="rectangle-3"></div>
      <div class="rectangle-4"></div>
      <div class="rectangle-5"></div>
      <div class="rectangle-6"></div>
      <div class="text-wrapper-2">Gender</div>
      <div class="text-wrapper-3">Full Name</div>
      <div class="text-wrapper-4">Mail</div>
      <div class="text-wrapper-5">Mobile</div>
      <div class="text-wrapper-6">Department</div>
      <div class="text-wrapper-7">Register No</div>
      <div class="text-wrapper-8">Age</div>
    </div>
  </body>
</html>
```

page 4
```
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="android-compact">
      <img class="logo" src="img/logo.png" />
      <div class="thank-you">THANK YOU</div>
      <p class="text-wrapper">Your registration was successful, we are eagerly waiting for your participation</p>
      <div class="div">CONTACT US</div>
      <div class="text-wrapper-2">Phone : 987654321</div>
      <div class="text-wrapper-2">Phone : 789456321</div>
      <div class="text-wrapper-3">Mail : saveetha@gmail.com</div>
    </div>
  </body>
</html>
```

## OUTPUT:
![alt text](<Screenshot 2025-10-08 210748.png>)

## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
