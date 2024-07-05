# JS-two-
// script.js
import styled from 'styled-components';

const Hero = styled.section`
  background-color: #f0f0f0;
  padding: 20px;
  text-align: center;
`;

const HeroText = styled.div`
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 10px;
`;

const ScrollDownButton = styled.button`
  background-color: #4CAF50;
  color: #ffffff;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
`;

// Use the styled components in your JavaScript code
const heroSection = document.createElement('section');
heroSection.className = Hero;

const heroText = document.createElement('div');
heroText.className = HeroText;
heroText.textContent = 'Welcome to my Portfolio';

const scrollDownButton = document.createElement('button');
scrollDownButton.className = ScrollDownButton;
scrollDownButton.textContent = 'Scroll Down';

heroSection.appendChild(heroText);
heroSection.appendChild(scrollDownButton);

document.body.appendChild(heroSection);
