# MinimaCSS

MinimaCSS is not intended to be treated as a library or framework.
MinimaCSS's goal is to be a launching point for your CSS. It's a 
skeleton of styles designed to provide a simple start where basic 
decisions have already been made.

MinimaCSS's guiding philosophy is to be an anti-dependency. It is 
closer to a reference resource than it is to a library or framework. 
I encourage you to consider every MinimaCSS to be a fork of the 
original project. Once forked, it's yours, build it up and modify it 
according to your own app's unique needs.


## Getting Started

MinimaCSS provides default styles with customizable variables (located 
in [minima.config.css]()) to get your design up and running quickly.

Duplicate the repo and start changing anything you want.

MinimaCSS uses `rem` size values. Given the default values in 
[minima.reset.css](), `1.6rem` will be equivalent to `16px`.


## Variable Naming Conventions

> Naming is an exercise in philosophy, rather than an exercise in science.

MinimaCSS's philosophy for variable has two parts: 

1. Start with specifics for the smallest piece, then get more descriptive by appending the next biggest context.
2. Don't bike shed names

For example, if you want a variable for the color, use `--color`. If it's 
for a border, then use `--color-border`. Then, suppose you need the color of a 
border for a form input, look for `--color-border-input`. Then, suppose you 
need the color of a border for an input element that is in an error state, look 
for `--color-border-input-error`.

- The concept of color is smaller than the context of border since the variable 
holds a color value, not a border value.
- Border < input since inputs have more attributes than just borders.
- Input < error because input is an html concept while error is a wider user interface concept.


## Configuration

- `--gutter` Used to set the gap between layout boxes.


## Todo

- [x] grid/masonry styles and demo (multi column example)
- [x] flex styles supporting multi 'columns'
- [x] mobile styles using media queries and/or contaienr queries
- [x] error message block style
- [ ] error message list style
- [ ] table style
- [ ] scrollbar style
- [ ] dynamic call-to-action button styles and demo
- [ ] refine configuration variable names for clarity
- [ ] document configuration values

