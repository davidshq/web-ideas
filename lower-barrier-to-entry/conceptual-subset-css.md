# Introduction
This subset assumes we have some very fundamental knowledge of CSS that we aren't going to jump into in detail here. For example, the basic (not advanced) tutorials from [W3Schools on CSS](https://www.w3schools.com/css/) or [Learn X in Y Minutes](https://learnxinyminutes.com/docs/css/).

The subset recommended here for CSS is initially based on the results of the [State of CSS 2019 survey](https://2019.stateofcss.com/). As time progresses additional features may be added as core concepts and some removed, this is just a very basic example of what such a subset might look like.

# Someone Else Said Something
- "For much of CSS, you don’t need to worry about learning properties and values by heart. You can look them up when you need them. However, there are some key underpinnings of the language, without which you will struggle to make sense of it." - Rachel Andrew, [Smashing Magazine](https://css-tricks.com/the-secret-weapon-to-learning-css/).
- " I couldn’t stop thinking about the advice that I would give to a fledgling developer who's interested in web design and CSS—where would I recommend that they start? There’s so much to cover that merely thinking about it gives me a headache." - Robin Rendle, [CSS Tricks](https://css-tricks.com/the-secret-weapon-to-learning-css/).

# Features
## Layout
- Include: Grid, Flexbox
- Exclude: Multi-column Layout, Writing Modes, Exclusions
## Shapes & Graphics
- Include: Filters & Effects
- Exclude: Shapes, object-fit, clip-path, Masking, blend-mode 
## Interactions
- Exclude: Scroll Snap, overscroll-behavior, overflow-anchor
## Typography
- Include: @font-face, Variable Fonts[1], Line Breaking Properties[2]
- Exclude: font-variant, initial-letter
## Animations & Transformations
- Include: Transitions, Transforms, Animations
## Other
- Include: Variables, calc()
- Exclude: @supports[1], Contain, will-change

# Units & Selectors
## Units
- Include: px, %, em, vh, vw, rem
- Exclude: pt, vmin, vmax, cm, ch, mm, in, ex
## Pseudo-Elements
- Include: ::before, ::after, ::placeholder
- Exclude: ::selection, ::first-letter, ::first-line
## Combinators
- Include: div span, div > span, div + div, div ~ div
## Tree & Document Structures
- Include: :first-child, :nth-child(), :last-child, :not(), :nth-of-type(), :nth-last-child(), :first-of-type, :last-of-type
- Exclude: :root, nth-last-of-type(), :empty, :only-child, :only-of-type, :lang()
## Attributes 
- Include: Equality, Presence, Starts With, Constains Substring
- Exclude: Contains Word, Ends With
## Links & URLs
- Include: :link, :visited
- Exclude: :target, :any-link, :local-link
## Interaction
- Include: :hover, :focus, :active
- Exclude: :focus-within, :focus-visible
## Form Controls
- Include: :checked, :enabled, :disabled, :required, :optional
- Exclude: :valid, :invalid, :default, :read-only, :read-write, :placeholder-show, :indeterminate, :in-range, :out-of-range, :user-invalid

# Technologies
## Pre & Post Processors
- Include: SASS, PostCSS
- Mention: LESS
- Exclude: Stylus
## Frameworks
- Mention: Bootstrap, Semantic UI, Bulma, Tailwind, Tachyons, Ant Design, PureCSS
- Exclude: Foundation, UIKit, Primer, Materialize CSS
## Methodologies
- Include: BEM
- Mention: Atomic CSS, OOCSS, SMACSS
- Exclude: ITCSS
## CSS-in-JS
- Include: CSS Modules
- Touch Upon: Style Components, Styled JSX, Emotion
- Exclude: JSS, Glamor, Aphrodite, Radium
# Other Tools
## Text Editors
- Include: VS Code
- Touch Upon: Sublime Text
- Exclude: Atom, WebStorm, Vim, Emacs, PHPStorm, Notepad++, Brackets., IntelliJ, Coda, Visual Studio, Nano, Dreamweaver, Textmate, BBEdit
## Browsers
- Include: Chrome, Firefox
- Touch Upon: Safari, IE
- Exclude: Edge, Vivaldi, Chromium, Yandex, UC Browser, Firefox Quantum, Samsung Internet, Opera, Brave
# Environments
## Testing Browsers
- Include: Chrome, Firefox, Safari, Edge, Safari iOS, Chrome Android
- Touch Upon: IE
- Exclude: Chrome iOS, Firefox Android, Opera, Samsung Internet, Brave, Vivaldi, Opera Mini, UC Browser
## Form Factors
- Include: Desktop, Smartphone, Tablet
- Touch Upon: Print, Screen Reader, Email
- Exclude: Feature Phone, TV, Smart Watch, Gaming Console

# Footnotes
[1] May be worth educating due to future value.
[2] Surprised this is so widely used.
