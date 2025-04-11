# Instructions for Creating Task Cards

## Card Dimensions
- Each card should have the following dimensions:
  - Width: 60mm
  - Height: 85mm
- The corners should be rounded with a radius of 5mm.

## SVG Structure
- Use the `<svg>` element with the following attributes:
  ```xml
  <svg xmlns="http://www.w3.org/2000/svg" width="60mm" height="85mm" viewBox="0 0 60 85">
  ```
- Add a `<rect>` element for the card background:
  ```xml
  <rect x="1" y="1" width="58" height="83" rx="5" ry="5" fill="white" stroke="black" stroke-width="0.5"/>
  ```

## Text Layout
- Use `<text>` elements for the card content.
- Font settings:
  - Font family: Arial
  - Font size: 3mm to 3.5mm
  - Font weight: Bold for headings
- Example text layout:
  ```xml
  <text x="5" y="15" font-family="Arial" font-size="3.5" font-weight="bold" fill="black">[Card Title]</text>
  <text x="5" y="30" font-family="Arial" font-size="3" fill="black"><tspan font-weight="bold">Required Check:</tspan> [Skill]</text>
  <text x="5" y="35" font-family="Arial" font-size="3" fill="black"><tspan font-weight="bold">Dice Roll:</tspan> [Value]</text>
  <text x="5" y="45" font-family="Arial" font-size="3" fill="black"><tspan font-weight="bold">Success:</tspan> [Outcome]</text>
  <text x="5" y="55" font-family="Arial" font-size="3" fill="black"><tspan font-weight="bold">Failure:</tspan> [Consequence]</text>
  <text x="5" y="65" font-family="Arial" font-size="3" fill="black"><tspan font-weight="bold">Alt:</tspan> [Alternative]</text>
  ```

## Example Card
- Below is an example of a complete card:
  ```xml
  <svg xmlns="http://www.w3.org/2000/svg" width="60mm" height="85mm" viewBox="0 0 60 85">
    <rect x="1" y="1" width="58" height="83" rx="5" ry="5" fill="white" stroke="black" stroke-width="0.5"/>
    <text x="5" y="15" font-family="Arial" font-size="3.5" font-weight="bold" fill="black">Build Initial Prototype</text>
    <text x="5" y="30" font-family="Arial" font-size="3" fill="black"><tspan font-weight="bold">Required Check:</tspan> Technical Expertise</text>
    <text x="5" y="35" font-family="Arial" font-size="3" fill="black"><tspan font-weight="bold">Dice Roll:</tspan> 4+</text>
    <text x="5" y="45" font-family="Arial" font-size="3" fill="black"><tspan font-weight="bold">Success:</tspan> Gain 1 Innovation</text>
    <text x="5" y="55" font-family="Arial" font-size="3" fill="black"><tspan font-weight="bold">Failure:</tspan> Lose 1 Time Token</text>
    <text x="5" y="65" font-family="Arial" font-size="3" fill="black"><tspan font-weight="bold">Alt:</tspan> Spend 1 Innovation</text>
    <text x="5" y="70" font-family="Arial" font-size="3" fill="black">Token to retry</text>
  </svg>
  ```

## Notes
- Ensure all cards follow the same structure and layout for consistency.
- Use descriptive titles and clear instructions for each card.
- Save each card as an individual SVG file with a unique filename (e.g., `PR001.svg`, `VV001.svg`, etc.).
