# Responsive-css-framework
Responsive from design. You only need 2 layouts. Portrait and Landscape. Scale the rest. 

## Idea
I got tired of writing complicated media queries, optimizing for mobile, web, to find out that by finishing optimization on tablet I am breaking either mobile or desktop view. Where is large desktop ? Where are future devices ? I decided to siplify it for myself. Design two views, and scale everything else. Root font-size manipulation takes very far. I decided to create this simple framework of most of the stuff I use in my projects. 


## Pick what you like
For simplicity and customizability I am leaving it as simple css files and js scripts.

If you don't like something copy and remove the parts you don't like. Is it missing something ? add it to your code. Do you think anybody can benefit from your changes ? Make a pull request. 

## How it works
Everything is build based on 2 specific views. Orientation Landscape or Portrait. That is why every style has generic version, portrait version and landscape version.

The root font size changes based on the tic, if it is too small it is too lagy(it re-renders too much), so after some testing 100px seems like reasonable tic. Check two views and calculate the rest. Let's say you have mobile 500px width portrait view -> you can build it with 10px root font size. you can check 1500px width portrait and find what is reasonable. for example 20px. Now you have middle and bottom. 

((top - bottom) x 1 + bottom. -> that would be your high. and you would select 20px. 

if you want to scale it higher. you can do same thing but x 2 that would be 30px and top would be 2500px. so the middle would still be 1500px and 20px.  

you can go as high as you want. 10x -> 100px 10500px. you got the point.





