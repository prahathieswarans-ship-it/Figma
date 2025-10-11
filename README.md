# Ex09 Event Registration Web Application
## Date:11.10.2025

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
```html
page 1

import React from "react";
import logo1 from "./logo-1.png";
import rectangle1 from "./rectangle-1.svg";

export const AndroidCompact = () => {
  return (
    <div className="bg-[#c65555] w-full min-w-[412px] min-h-[843px] relative">
      <img
        className="absolute top-[9px] left-3 w-[388px] h-[59px] aspect-[6.58] object-cover"
        alt="Logo"
        src={logo1}
      />

      <div className="absolute top-[251px] left-[33px] [font-family:'Irish_Grover-Regular',Helvetica] font-normal text-white text-5xl tracking-[0] leading-[normal]">
        SEC Dance Club
      </div>

      <img
        className="top-[492px] h-[58px] absolute left-[82px] w-[249px]"
        alt="Rectangle"
        src={rectangle1}
      />

      <div className="top-[396px] h-[52px] bg-[#d9d9d9] absolute left-[82px] w-[249px]" />

      <div className="absolute top-[399px] left-[136px] [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-[#1d0202] text-4xl tracking-[0] leading-[normal]">
        Login
      </div>

      <div className="absolute top-[505px] left-[104px] [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-[#1e1717] text-4xl tracking-[0] leading-[normal]">
        Register
      </div>
    </div>
  );
};

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src//*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

page 2

import React from "react";

export const AndroidCompact = () => {
  return (
    <div className="bg-[#6834b1] w-full min-w-[412px] min-h-[843px] flex flex-col gap-14">
      <div className="ml-11 w-[323px] h-[58px] mt-[150px] [font-family:'Irish_Grover-Regular',Helvetica] font-normal text-white text-5xl tracking-[0] leading-[normal]">
        Cultural Events
      </div>

      <p className="ml-[107px] w-[197px] h-[315px] [font-family:'Gluten-Regular',Helvetica] font-normal text-white text-2xl tracking-[0] leading-[normal]">
        *solo Dance
        <br />
        <br />
        *Group Dance
        <br />
        <br />
        *Western Dance
        <br />
        <br />
        *Folk Dance
        <br />
        <br />
        *Classical Dance
        <br />
        <br />
        *Adaptune <br />
        <br />
        *Duo <br />
        <br />
        *Gymnastics
      </p>
    </div>
  );
};

import React from "react";

export const AndroidCompact = () => {
  return (
    <div className="bg-[#6834b1] w-full min-w-[412px] min-h-[843px] flex flex-col gap-14">
      <div className="ml-11 w-[323px] h-[58px] mt-[150px] [font-family:'Irish_Grover-Regular',Helvetica] font-normal text-white text-5xl tracking-[0] leading-[normal]">
        Cultural Events
      </div>

      <p className="ml-[107px] w-[197px] h-[315px] [font-family:'Gluten-Regular',Helvetica] font-normal text-white text-2xl tracking-[0] leading-[normal]">
        *solo Dance
        <br />
        <br />
        *Group Dance
        <br />
        <br />
        *Western Dance
        <br />
        <br />
        *Folk Dance
        <br />
        <br />
        *Classical Dance
        <br />
        <br />
        *Adaptune <br />
        <br />
        *Duo <br />
        <br />
        *Gymnastics
      </p>
    </div>
  );
};

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src//*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

page 3

import React from "react";
import logo2 from "./logo-2.png";

export const AndroidCompact = () => {
  return (
    <div className="bg-[#8e9d4c] w-full min-w-[412px] min-h-[843px] flex flex-col">
      <img
        className="ml-0.5 w-[407px] h-[61px] mt-[18px] aspect-[6.65] object-cover"
        alt="Logo"
        src={logo2}
      />

      <div className="ml-3 w-[388px] h-[103px] mt-[111px] [font-family:'Irish_Grover-Regular',Helvetica] font-normal text-white text-[85px] tracking-[0] leading-[normal]">
        Thank You
      </div>

      <p className="ml-3 w-[353px] h-[173px] mt-[129px] [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-white text-[32px] tracking-[0] leading-[normal]">
        <span className="[font-family:'Gravitas_One-Regular',Helvetica] font-normal text-white text-[32px] tracking-[0]">
          CONTACT US:
          <br />
          <br />
        </span>

        <span className="text-2xl">
          Phone:1234 1234
          <br />
          <br />
          mail:sec@gmail.com
        </span>
      </p>
    </div>
  );
};

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src//*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}


## output:
<img width="923" height="604" alt="Screenshot 2025-10-11 112012" src="https://github.com/user-attachments/assets/e103ba22-d974-4a9f-a16f-beb55784752e" />


## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
